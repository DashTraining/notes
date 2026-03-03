# PowerShell Script Publishing Best Practices

## Creating Modules

 #TO-DO: 

## Documenting

[PowerShell style guide](https://learn.microsoft.com/en-us/powershell/scripting/community/contributing/powershell-style-guide)

## Linting

- [Best Practices and Style Guide](https://poshcode.gitbook.io/powershell-practice-and-style/style-guide/introduction)
- [also here](https://github.com/PoshCode/PowerShellPracticeAndStyle)

In VS Code:

    {
        "powershell.codeFormatting.preset": "OTBS",
        "editor.formatOnSave": true
    }

## Versioning

- [Semantic versioning](https://semver.org/)
- [A discussion on BUILD and REVISION](https://softwareengineering.stackexchange.com/questions/24987/what-exactly-is-the-build-number-in-major-minor-buildnumber-revision)
- [Microsoft's take from the Engineering Fundamentals Playbook](https://microsoft.github.io/code-with-engineering-playbook/source-control/component-versioning/)

## Changelog

- [How to create a good changelog](https://keepachangelog.com/)
- [PowerShell module to do it](https://github.com/natescherer/ChangelogManagement)
- [Description of how to use the module](https://www.scriptrunner.com/blog-admin-architect/what-is-a-changelog-and-how-to-manage-it)

## Licensing

[Choose a License](https://choosealicense.com/)

## Putting it together

Think of using a scaffolding tool such as Plaster… [available here](https://github.com/PowerShellOrg/Plaster) ...which is now undergoing changes to make it up-to-date with PowerShell 7
Good guides on how to use it:

- [1](https://overpoweredshell.com/Working-with-Plaster/#the-default-plaster-template)
- [2](https://poshsecurity.com/blog/levelling-up-your-powershell-modules-with-plaster)
