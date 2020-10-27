Copy a File from an Azure VM
============================

            

**Description**


This runbook copies a remote file from a Windows Azure virtual machine to the host running the runbook.    Connect-AzureVM must be imported and published in order for this runbook to work. The Connect-AzureVM
runbook sets up the connection to the virtual machine where the remote file is copied from.  


When using this runbook, be aware that the memory and disk space size of the processes running your
runbooks is limited. Because of this, we recommend using runbooks only to transfer small files. 
All Automation Integration Module assets in your account are loaded into your processes,
so be aware that the more Integration Modules you have in your system, the smaller the free space
your processes will have. To ensure maximum disk space in your processes, make sure to clean up any local
files that a runbook transfers or creates before the runbook completes.


 


**Requirements**


Before importing and using this runbook the following items must be made available: 


  *  [Connect-AzureVM Runbook](http://gallery.technet.microsoft.com/scriptcenter/Connect-to-an-Azure-85f0782c) must be imported and published

  *  An Automation credential asset containing an Org Id username / password with access to this Azure subscription.

  *  PS Credential Asset containing the name and password to access the VM   

 


**Runbook Source**


A copy of the runbook content is included below:


 

 

        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
