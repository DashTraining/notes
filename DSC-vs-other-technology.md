---
title: DSC vs Other technology
tags: [DSC, Azure, PowerShell, deployment]
category: deployment
---

Comparison of some deployment and configuration management technologies, reflecting the modern state of things as of 2025.

### GPOs

* Fancy way of setting registry entries / user & OS-policy settings (user experience, desktops)
* Requires on-premise AD / Group Policy infrastructure
* Good at configuring user experience, desktop policies; not designed for software installation or server provisioning
* OU / AD-structure becomes a limitation if not planned well
* Easy to circumvent (if user has admin rights or does not want to apply it)

### SCCM

* Will perform deployment you want on the systems you want at the time you want — OS deployment, software, patches, bare-metal, server or workstation imaging
* Flexibility with Collections for targeting groups of machines
* Good for bare-metal, OS roll-out, large homogeneous fleets
* Requires substantial infrastructure and an agent on clients/servers
* Task sequences and configurations can get complex, heavy overhead for maintenance

### MDM

* No on-premise infrastructure — it’s cloud / device-management oriented; useful for mobile OS / modern device management
* Can apply settings and deploy apps in a mobile / cloud / managed-device context
* Doesn’t target traditional Windows-server workloads or deep server configuration; not ideal for complex server or infrastructure management
* Limited scope for fine-grained Windows server role configuration, registry tweaking, or cross-platform server setups

### DSC (classic / PS-DSC)

* Declarative configuration tool integrated with PowerShell — infrastructure-as-code approach to define system state declaratively, not as imperative scripts.
* Helps avoid configuration drift: ensures all machines stay in the declared desired state; scalable across machines.
* Works well for server roles, service configuration, registry settings, baseline configuration, compliance across Windows (and to some degree Linux) nodes.
* Configurations (MOF-based) + Local Configuration Manager (agent / LCM) model — some management overhead; older syntax (PowerShell DSL + MOF) can be rigid.
* Less suited for user-experience or desktop-policy management compared to GPO; better for infrastructure/server configuration

### DSC v3 (modern)

* Fully modernized version of DSC: standalone tool (not dependent on PowerShell), works cross-platform (Windows, Linux, macOS).
* Configurations are defined in JSON or YAML (not MOF); resources can be authored in *any* language (PowerShell, Python, Go, C#, Bash, etc.), making the system language-agnostic.
* Declarative + idempotent: DSC v3 ensures the system reaches and stays in the desired state, without re-applying unnecessary changes.
* Easier integration with modern DevOps / infrastructure-as-code workflows: JSON/YAML fits CI/CD pipelines, version control, automation toolchains nicely.
* Works for mixed / hybrid environments, and supports reusing existing PS-DSC resources via adapters — easing migration from classic DSC.
* More flexible tooling: because it’s not PowerShell-only, DSC v3 is lightweight, simpler (no LCM, no Windows-only dependencies), easier to scale and adopt in polyglot environments.
* Good for server / infrastructure configuration across OSes, automation of services, baseline configuration, reproducible deployments, and as part of IaC pipelines

## Where Each Shines

* **GPOs** remain best when your focus is *user-experience / desktop / client policy / registry-based user or workstation settings*. They are simple and well-suited for desktop/user management.
* **SCCM** remains relevant when you need powerful deployment and software/OS management (bare-metal imaging, large server/workstation fleets, patching, complex rollouts).
* **MDM** works when dealing with mobile devices, modern device management scenarios, cloud-managed workstations/mobile OS — but isn’t ideal for infrastructure or detailed server config.
* **DSC "classic" (PS-DSC)** is a good fit for server configuration, baseline management, Windows-server estates — particularly useful to enforce configuration drift prevention.
* **DSC v3** is the most forward-looking: ideal for modern infrastructure-as-code, hybrid/multi-OS environments, cloud + on-premises, automation pipelines — especially when you want reproducible, declarative, cross-platform infrastructure config, leveraging flexible resource authoring and integration.

## Tooling

### AMDXtoDSC

**Description:** [https://4sysops.com/archives/convert-group-policy-to-powershell-dsc-with-admxtodsc/](https://4sysops.com/archives/convert-group-policy-to-powershell-dsc-with-admxtodsc/)

**Download:** [https://github.com/gpoguy/ADMXToDSC](https://github.com/gpoguy/ADMXToDSC)

### MSIPackage DSC Resource
Can be used to install MSI files.

## Further Reading

* [Announcing DSC v3.0.0](https://devblogs.microsoft.com/powershell/announcing-dsc-v3/) — official release blog by the PowerShell Team introducing modern DSC v3.
* [See what’s new in Desired State Configuration v3](https://www.techtarget.com/searchWindowsServer/tip/See-whats-new-in-Desired-State-Configuration-v3) — summary of differences, features & cross-platform support at TechTarget.
* [Official repo for DSC v3](https://github.com/PowerShell/DSC) (open-source) — you can browse code, samples, resource model, and see how to author resources.
* [What Direction Should We Go?](http://stevenmurawski.com/powershell/2016/02/what-direction-should-we-go/?utm_content=buffer7ef46&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer) - a blog from back in 2016
* [The Case for Each](https://foxdeploy.com/2016/02/25/dsc-vs-gpo-vs-sccm-the-case-for-each/)
*	[Clear Simple Guide](https://cloudblogs.microsoft.com/enterprisemobility/2016/03/23/clear-simple-guidance-when-configmgr-and-intune-should-be-used-with-windows-10/) when these should be used
* [Compare Group Policy GPO and PowerShell DSC](https://blogs.technet.microsoft.com/ashleymcglone/2017/02/27/compare-group-policy-gpo-and-powershell-desired-state-configuration-dsc/)
* [Why Group Policy IS NOT DEAD](https://www.gpanswers.com/the-why-group-policy-is-not-dead-manifesto) 
