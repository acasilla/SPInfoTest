# Introduction 
Welcome to the new home of the SPFarmInfo Script

# Getting Started
1.	Copy the Get-SPFarmInfo.PS1 script to a SharePoint Server
2.	Launch the script .\Get-SPFarmInfo.ps1
3.	Collect and review the HTML report

# Extras
## -PatchInfo
You can get additional Patch Information with the -PatchInfo swtich, however this requires two things that your customer should be aware of. 
1. A Nuget Provider is required
2. MSI Powershell Module will be installed. 

Customers will receive the following prompt when using the PatchInfo switch:

    PatchInfo Warning
    PatchInfo requires a Nuget Provider and Microsoft's MSI Module to be installed. You may be prompted for this. Continue with PatchInfo?
    [Y] Yes  [N] No  [?] Help (default is "N"): 

If they answer Yes, they'll also be greeted with the following prompts during the execution of the script:

    NuGet provider is required to continue
    PowerShellGet requires NuGet provider version '2.8.5.201' or newer to interact with NuGet-based repositories. The NuGet provider must be available in 'C:\Program Files\PackageManagement\ProviderAssemblies' or
    'C:\Users\stuartpadmin.CONTOSO\AppData\Local\PackageManagement\ProviderAssemblies'. You can also install the NuGet provider by running 'Install-PackageProvider -Name NuGet -MinimumVersion 2.8.5.201 -Force'. Do you want
    PowerShellGet to install and import the NuGet provider now?

and

    Untrusted repository
    You are installing the modules from an untrusted repository. If you trust this repository, change its InstallationPolicy value by running the Set-PSRepository cmdlet. Are you sure you want to install the modules from 'PSGallery'?
    [Y] Yes  [A] Yes to All  [N] No  [L] No to All  [?] Help (default is "N"):

Customers will need to approve the installation of the Nuget Provider and the MSI Module. 
The MSI Module is authored by Heath Steward, copyright Microsoft Corporation
https://www.powershellgallery.com/packages/MSI/3.3.4



# Feedback
Please send Feedback and Requests for additional data collection to [us](mailto:cssspfarminfo@microsoft.com?subject=Feedback)  
 
# Contribute
Do you want to contribute? Reach out to [us](mailto:cssspfarminfo@microsoft.com?subject=Contribute). We'd love to have your contributions.

https://microsoft-my.sharepoint.com/:v:/p/stuartp/EaFMPHUZBh5NkmHTUGDqBWsBXSlMDUE1b6wgw44CXRPEqQ