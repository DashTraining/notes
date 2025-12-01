---
title: PKI Fundamentals Link List
tags: [PKI]
categories: PKI
---

Links from my 'PKI Fundamentals' training, available for delivery as corporate training or for individuals at authorized Microsoft Learning partners.

Please report broken links.

## Introduction to Cryptography

- [Cryptanalysis on Wikipedia](https://en.wikipedia.org/wiki/Cryptanalysis)

### Algorithms

- [Sunsetting SHA-1](https://security.googleblog.com/2014/09/gradually-sunsetting-sha-1.html) (kind of an old already in 2024)
- [SHA-256 Compatibility — SHA-256 Compatibility](https://support.globalsign.com/customer/portal/articles/1499561-sha-256-compatibility)
- [Disk encryption theory - Wikipedia](https://en.wikipedia.org/wiki/Disk_encryption_theory)
- [Good example of ECB (Electronic Codebook) encryption](https://upload.wikimedia.org/wikipedia/commons/f/f0/Tux_ecb.jpg), more on it here [The ECB Penguin](https://blog.filippo.io/the-ecb-penguin/)
- [Tweakable Block Ciphers](https://people.eecs.berkeley.edu/~daw/papers/tweak-joc.pdf)
- [Bitlocker: AES-XTS (new encryption type)](https://blogs.technet.microsoft.com/dubaisec/2016/03/04/bitlocker-aes-xts-new-encryption-type/)
- [You Don't Want XTS](https://sockpuppet.org/blog/2014/04/30/you-dont-want-xts/)

### OIDs

- [Show an OID at IANA](https://oid-base.com/get/1.3.6.1.4.1) then type 53698
- [IANA | Request Private Enterprise Numbers](http://pen.iana.org/pen/PenApplication.page)
- [OIDs for Microsoft Cryptography](https://support.microsoft.com/en-us/help/287547/object-ids-associated-with-microsoft-cryptography)

### ASN.1

- [ASN.1 Editor | PKI Solutions](https://www.pkisolutions.com/tools/asn1editor/)

## Getting Started with CAs

### External CAs

- [SSL certificates at Comodo](https://ssl.comodo.com/free-ssl-certificate.php)
- [Microsoft Trusted Root Certificate Program Audit Requirements | Microsoft Learn — Microsoft Trusted Root Certificate Program](https://social.technet.microsoft.com/wiki/contents/articles/31635.microsoft-trusted-root-certificate-program-audit-requirements.aspx)
- [Example of terminated trust](https://blog.qualys.com/ssllabs/2017/04/05/ssl-labs-distrusts-wosign-and-startcom-certificates)
- [Example of terminated trust](https://blog.qualys.com/ssllabs/2017/09/26/google-and-mozilla-deprecating-existing-symantec-certificates)

### Active Directory Certificate Services

- [Active Directory Certificate Services (AD CS) Public Key Infrastructure (PKI) Design Guide](https://social.technet.microsoft.com/wiki/contents/articles/7421.active-directory-certificate-services-ad-cs-public-key-infrastructure-pki-design-guide.aspx)
kb5005413-mitigating-ntlm-relay-attacks-on-active-directory-certificate-services-ad-cs-3612b773-4043-4aa9-b23d-b87910cd3429)
- [Commands for AD CS setup on Windows Server Core](https://learn.microsoft.com/en-us/windows-server/identity/ad-cs/)
- [Lab Guide: Installing a Two-Tier AD CS](https://michaelpoore.com/2016/03/howto-publishing-offline-root-ca-certs-and-crls/)
- [Lab Guide: Deploying an AD CS Two-Tier PKI Hierarchy](https://technet.microsoft.com/library/hh831348.aspx)
- [AD CS common issues](https://posts.specterops.io/certified-pre-owned-d95910965cd2)
- [KB5005413: Mitigating NTLM Relay Attacks on AD CS](https://support.microsoft.com/en-us/topic/)
- [What is a strong key protection in Windows? - Sysadmins LV — Much more about this:](https://www.sysadmins.lv/retired-msft-blogs/pki/what-is-a-strong-key-protection-in-windows.aspx)
- [Activating the Strong Private Key Protection](https://adelnadjarantoosi.wordpress.com/2017/04/12/how-to-activate-the-enable-strong-private-key-protection-option/)
- [Force strong key protection for user keys stored on the computer](https://technet.microsoft.com/en-us/library/jj852211(v=ws.11).aspx)
- [Windows FIPS 140 validation](https://support.microsoft.com/en-us/help/811833/system-cryptography-use-fips-compliant-algorithms-for-encryption-hashi) FIPS compliant algorithms for encryption, hashing, and signing Federal Information Processing Standard (FIPS) 140-2 is a security implementation that is designed for certifying cryptographic software. This setting has a lot of impact, not all of it good.
- [AD CS Security Guidance](https://social.technet.microsoft.com/wiki/contents/articles/10942.ad-cs-security-guidance.aspx)
- [Install and Configure Certificate Enrolment Policy Web Service](https://www.petenetlive.com/KB/Article/0001250)
- [TameMyCerts policy module for Microsoft Active Directory Certificate Services](https://docs.tamemycerts.com/)
- [Sleepw4lker/TameMyCerts: Policy Module for Microsoft Active Directory Certificate Services](https://github.com/Sleepw4lker/TameMyCerts) on GitHub
- [GhostPack/PSPKIAudit: PowerShell toolkit for AD CS auditing based on the PSPKI toolkit. — PSPKIAudit](https://github.com/GhostPack/PSPKIAudit) on GitHub
- [certutil — PKI Health Tool, Certutil](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/certutil)

### PowerShell automation

- [PSPKI | PKI Solutions — PSPKI](https://www.pkisolutions.com/tools/pspki/)
- [Approve-CertificateRequest with PSPKI](https://www.sysadmins.lv/projects/pspki/Approve-CertificateRequest.aspx)
- [Backup-CARoleService](https://technet.microsoft.com/library/dn440704(v=wps.630).aspx)

### HSMs

- [Certification Authority Guidance](https://technet.microsoft.com/en-us/library/hh831574(v=ws.11).aspx) Planning Key Storage, Hardware Security Module (HSM)
- [Azure Cloud HSM Onboarding Guide](https://github.com/microsoft/MicrosoftAzureCloudHSM/blob/main/OnboardingGuides/Azure%20Cloud%20HSM%20Onboarding.pdf)
- [Azure Cloud HSM Integration Guide](https://learn.microsoft.com/en-us/azure/cloud-hsm/integration-guides)
- [Key storage provider (KSP) for AWS CloudHSM Client SDK 5 - AWS CloudHSM — AWS CloudHSM](https://docs.aws.amazon.com/cloudhsm/latest/userguide/ksp-library.html)
- [SoftHSM v2 for Windows](https://github.com/disig/SoftHSM2-for-Windows)

### Online Responders

- [Manually verify a certificate against an OCSP](https://raymii.org/s/articles/OpenSSL_Manually_Verify_a_certificate_against_an_OCSP.html) with OpenSSL

### NDES

- [Linuz Certificate Enrollment and Automated Renewal Using NDES](https://blogs.technet.microsoft.com/jeffbutte/2016/12/16/236/)

### OpenSSL

- [Download and install OpenSSL Light with winget](https://winget.run/pkg/ShiningLight/OpenSSL.Light)

## Practical Applications

### Web Servers

- [Nartac Software IIS Crypto](https://www.nartac.com/Products/IISCrypto) for setting cipher suites on IIS
- [SSL Server Test](https://www.ssllabs.com/ssltest/index.html) test which cipher suite is being used(Powered by Qualys SSL Labs)
- [Hardenize](https://www.hardenize.com/) comprehensive web site configuration test
- [CAA Records](https://support.dnsimple.com/articles/caa-record/) devined by DNS Simple
- [CAA Records](https://letsencrypt.org/docs/caa/) Certificate Authority Authentication defined by Let's Encrypt
- [CAA Record Generator](https://sslmate.com/caa/) Construct a CAA record
- [DNS Propagation Checker](https://www.whatsmydns.net/) Global DNS Testing Tool — Check proppegation of your DNS records to troubleshoot CAA visibility
- [HSTS Preload List Submission](https://hstspreload.org/)
- [Certificate and Public Key Pinning](https://owasp.org/www-community/controls/Certificate_and_Public_Key_Pinning)
- [Red Sift](https://redsift.com/)  Proactive certificate expiry notification

### Smart Cards

- [Drivers for the Gemalto cards](http://download.windowsupdate.com/d/msdownload/update/driver/drvs/2016/06/20886167_c141b07eec3171d843702d148abec1903f4e5e16.cab)
- [Setting up Certificate Templates to Enroll on behalf of other Users](https://pivkey.zendesk.com/hc/en-us/articles/203128059-Setting-up-Certificate-Templates-to-Enroll-on-behalf-of-other-Users-Server-2008-R2-)
- [Enabling smart card logon - Windows Server | Microsoft Learn — Logon with certs from 3rd-party Cas](https://support.microsoft.com/en-us/help/281245/guidelines-for-enabling-smart-card-logon-with-third-party-certificatio)
- [Virtual Smart Cards](https://techcommunity.microsoft.com/t5/ask-the-directory-services-team/setting-up-virtual-smart-card-logon-using-virtual-tpm-for/ba-p/400409)
- [Get Started with Virtual Smart Cards - Walkthrough Guide](https://docs.microsoft.com/en-us/windows/security/identity-protection/virtual-smart-cards/virtual-smart-card-get-started)

### PowerShell Remoting

- [Enable secure Windows/Powershell Remoting over https](https://michlstechblog.info/blog/powershell-enable-secure-windows-powershell-remoting-over-https/)

### Disk encryption

- [How to Make BitLocker Use 256-bit AES Encryption Instead of 128-bit AES](https://www.howtogeek.com/193649/how-to-make-bitlocker-use-256-bit-aes-encryption-instead-of-128-bit-aes/)

### Code signing

- [SignTool - Win32 apps | Microsoft Learn — Sign Tool documentation here:](https://docs.microsoft.com/en-us/windows/win32/seccrypto/signtool)
- [SSL certificates inside Java apps](https://medium.com/@codebyamir/the-java-developers-guide-to-ssl-certificates-b78142b3a0fc)
- [Java Code Signer](https://docs.oracle.com/javase/tutorial/security/toolsign/signer.html)

### DNS SEC

- [DNSViz](https://dnsviz.net/d/lab.graydaycafe.com/dnssec/) visualization for "lab.graydaycafe.com"
- [DNSSEC Debugger](https://dnssec-debugger.verisignlabs.com/lab.graydaycafe.com)

### Timestamps

- [Time Stamp Server & Stamping Protocols](https://www.sectigo.com/resource-library/time-stamping-server)
- [Free Time Stamp Authority](https://www.freetsa.org/index_en.php)

### Other applications

- [What is Strict KDC Validation? by Ammar Hasayen](https://blog.ahasayen.com/what-is-strict-kdc-validation/)
- [Enabling Strict KDC Validation in Windows Kerberos](https://www.microsoft.com/en-us/download/details.aspx?id=6382)
- [Authenticate with X.509 certificates — Azure IoT](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-x509ca-overview)
- [Device Guard](https://docs.microsoft.com/en-us/windows/device-security/device-guard/deploy-device-guard-deploy-code-integrity-policies)
- [Encrypted SQL Server Connections](https://techcommunity.microsoft.com/t5/azure-sql-database/certificate-based-authentication-for-azure-sql-db-using-azure/ba-p/386135)
- [Using Certificates in Azure SQL Database](https://techcommunity.microsoft.com/t5/azure-database-support-blog/using-certificates-in-azure-sql-database-import/ba-p/368949)

## Further reading

- [Trustless transaction verification](https://youtu.be/bBC-nXj3Ng4?si=l7akw-9R3o8q53HK&t=131) (watch on YouTube)
- [Post-quantum Cryptography](https://www.techrepublic.com/blog/it-security/how-quantum-cryptography-works-and-by-the-way-its-breakable/)
