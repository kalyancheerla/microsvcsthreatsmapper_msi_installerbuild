# microsvcsthreatsmapper_msi_installerbuild
Advanced Installer configuration for the MicroSvcsThreatsMapper extension to build an installable msi app.

### Step 1:
**File:** MicroSvcsThreatsMapper for TMS.aip

Open the above aip file in the advanced installer tool.

Note: Do the appropriate changes to modify the installer as necessary at your own risk.

### Step 2:
Update the location for the DLL file MicroSvcsThreatsMapper.dll in the Resources -> Files and Folders -> *'Local Application Data/ThreatsManagerPlatform/MicroSvcsThreatsMapper/'*.

### Step 3:
Perform Build (F7). Locate the MSI installer in the directory *'MicroSvcsThreatsMapper for TMS-SetupFiles'/*.

Use the installer to install the extension DLL in the *$Env:LOCALAPPDATA/ThreatsManagerPlatform/* directory location for the TMS application to pick it.

**Note:**
  1. Add the 'MicroSvcsThreatsMapper' keyword in the Options -> Extensions -> Validation Rules -> Assembly must start with one of those prefixes.
  2. Disable the option for Assembly must be signed with one of those certificates.
