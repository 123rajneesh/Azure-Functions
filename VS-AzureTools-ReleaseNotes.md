# Release Notes - Azure Functions and Web Jobs Tools

These are the changes to each version that has been released
on the official Visual Studio extension Marketplace.

# Known Issues

## Latest release

* **Issue:** Queue Trigger and Blob Trigger are not available trigger types immediately after File > New Project > Azure Functions.
* **Workaround:** Add these trigger types by right-clicking on the project in Solution Explorer and select Add > New Azure Function.
* **Issue:** The VSIX for the functions tools will not work with VS 2017 15.8 Preview relases.
* **Workaround:** Only use the VSIX for 15.6 or 15.7. It is being updated to work with 15.8 when that version of Visual Studio releases.

## Visual Studio 15.6 (fixed in 15.7 and later)
   * ### Issue:
     Creating a new App Service Plan from Visual Studio fails with a message similar to "The resource '<storage_account>' under resource group '<your_resource_group>' was not found.
   * ### Workaround
     This error occurs when you select a Storage Account that is in a different resource group than the Resource Group selection in the dialog.  Either choose the same resource group in the dialog, or create a new storage account.  

# Release Notes
## 15.10.2009.0
- Fixes issues with publishing to Azure failing prematurely

## 15.0.40617.0
Minimum required Visual Studio version: VS2017 15.6

- The tools will run v2 Azure Functions locally against .NET Core 2.1.

## 15.0.40502.0
Minimum required Visual Studio version: VS2017 15.6

- Tools now consume a feed which keeps templates, build tools, and the runtime up to date whenever there is a change made in the service.

## 15.0.40405.0
Minimum required Visual Studio version: VS2017 15.6

- Updates Azure Functions V1 templates to 1.0.3.10178
- Updates Azure Functions V2 templates to 2.0.0-beta-10177
- Updates Azure Functions Core Tools to  2.0.1-beta.25

## 15.0.40322.0
Minimum required Visual Studio version: VS2017 15.6

- Fix a bug where running and publishing a v2 Functions app with the latest runtime failed
- Starts the Azure Storage Emulator on debug if it is specified in local development settings, with a message to ask you to start manually if we cannot start it
- Recognize if you do not have .NET Framework 4.7.1 and add a message telling you where to install it if it cannot be detected

## 15.0.40108.0
Minimum required Visual Studio version: VS2017 15.5

- Fix for bug in remote debugging of V2 Function
- Fix to Add New Function button

## 15.0.31201.0
Minimum required Visual Studio version: VS2017 15.5

- Remote debugging now works with V2 projects

## 15.0.31114.0
Minimum required Visual Studio version: VS2017 15.5

- .NET Core support
- New Functions project dialog
  - New project templates (HttpTrigger, QueueTrigger, TimerTrigger)
  - Improved storage emulator configuration
  - Default to local storage emulator
- New dialog for managing Azure app settings in Visual Studio
- Detect mismatching functions runtime versions when publishing

## 15.0.30923.0

- Updated the CLI that ships with the extension to v1.0.4
- Added feature to dynamically fetch latest CLI
- Added a button for adding a Function
- New settings options in publish flow
- Various minor bug fixes

## 15.0.30901.0

- Fixed bug where adding a Function would change referenced SDK version to 1.0.0.
