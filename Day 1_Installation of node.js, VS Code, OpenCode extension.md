
#### Installation setup

Install Node.js & Visual Studio for setting up Playwright Environment
- We using javascript libraries to write our automation code so we need a platform that runs the javascript code and that's why node.js 
is the platform which supports js related code. 
- Go to https://nodejs.org/en/download and if using windows then select .msi to download, macOS etc also available depending on your 
system you can download it >> once downloaded, install node 
- Now set the path >> node.js folder will be visible in program files >> open folder >> copy the url and then open the system environment 
variables from start menu search >> Create a new path variable name as NODE_HOME and paste the path value then press OK button to set it 
- Next you have to install editor to write code so install the Visual Studio Code  which is best tool to write JS/TS code  https://code.visualstudio.com/  
- Open the Visual Studio code & install the OpenCode extension from Marketplace/Extension

-------------------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------

#### Note for Windows PowerShell Users.
In the next chapter/section, while executing npm init playwright, you might see an error in powershell.

Here's how you can fix it:

Here are the steps to fix the issue persistently:
 
1.  **Open PowerShell as Administrator**:
    *   Search for "PowerShell" in the Start menu.
    *   Right-click it.
    *   Select **Run as Administrator**.
 
2.  **Check Current Execution Policy**:
    *   Run this command in PowerShell:
        `Get-ExecutionPolicy -List`
    *   This shows policies for different scopes.
 
3.  **Set Persistent Execution Policy**:
    *   To allow scripts for your user account persistently:
        `Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Bypass`
    *   This setting applies only to your user account.
    *   It remains active after you restart your computer.
    *   Answer 'Y' (Yes) if prompted to confirm the change.
 
    *   Alternatively, to allow scripts for all users persistently (requires administrator privileges):
        `Set-ExecutionPolicy -Scope LocalMachine -ExecutionPolicy Bypass`
    *   This setting applies to all users on the computer.
    *   It remains active after restarts.
    *   Answer 'Y' (Yes) if prompted.
    *   Choose the scope (`CurrentUser` or `LocalMachine`) that best fits your needs. `CurrentUser` is often sufficient and safer.
 
4.  **Run Your Command Again**:
    *   Retry your `npm init playwright` command.
    *   It should run without the execution policy error.
 
**Additional Notes**:
 
*   Using `Bypass` lets any script run. Understand the security risk before proceeding.
*   If problems continue, consider reinstalling Node.js. Get the latest version from the Node.js website.






