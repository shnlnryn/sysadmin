## Enable Anonymous printing on a Windows 2016 print server



1. _Provision Windows Server and add Feature Printing  & Document Services -> Printer Server_

2. _Add Everyone, Guest and ANONYMOUS LOGON to the permissions of the share._ 

      Open the Group Policy Editor (e.g. by running gpedit.msc)  

      Computer Configuration -> Windows Settings -> Security Settings -> Local Policies -> Security Options 

      Accounts: Guest account status: Enabled 

      Network access: Let Everyone permissions apply to anonymous users: Enabled 

      Network access: Restrict anonymous access to Named Pipes and Shares: Disabled 

      Network access: Shares that can be accessed anonymously: YOUR_SHARE_NAME 

 
