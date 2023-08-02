# Intune Windows 11 CleanSweep

This repository contains a PowerShell script for cleaning up a fresh Windows build. The script is compatible with both Windows 10 and Windows 11.

## Script Functionality

The script performs the following tasks:

- Removes AppX Packages
- Disables Cortana
- Removes McAfee
- Removes HP Bloat
- Removes Dell Bloat
- Removes Lenovo Bloat
- Removes any unwanted installed applications
- Removes unwanted services and tasks
- Removes Edge Surf Game

The script also generates a log file at `C:\ProgramData\cleansweep\cleansweep.log`.

## Updates

The script has been updated multiple times to add new features and fix issues. Some of the notable changes include:

- Added additional HP applications (12/08/2022)
- Added Clipchamp (new in W11 22H2) (23/09/2022)
- Fixed issue with Dell apps (28/10/2022)
- Added Teams Machine wide to exceptions (23/11/2022)
- Whitelisted Dell Audio and Firmware (07/12/2022)
- Added Windows 11 start menu support (19/12/2022)
- Removed Gaming Menu from Settings (20/12/2022)
- Fixed Scheduled task error and cleared up $null positioning (18/01/2023)
- Re-enabled Telemetry for Endpoint Analytics (22/01/2023)
- Added Microsoft Family to removal list (30/01/2023)
- Fixed Dell loop (31/01/2023)
- Removed reg keys for Teams Chat (08/02/2023)
- Added HP Sure Apps (14/02/2023)
- Enabled Location tracking (with commenting to disable) (07/03/2023)
- Teams chat fix (08/03/2023)
- Dell array fix (10/03/2023)
- Removes News Feed (29/04/2023)
- Added Set-ACL (26/05/2023)
- Added multi-language support for Set-ACL commands (26/05/2023)
- Logic to check if gamepresencewriter exists before running Set-ACL to stop errors on re-run (30/05/2023)
- Removed Microsoft Store

## Usage

The script does not require any inputs and does not produce any outputs other than the log file.

## Author

The script was created by Andrew Taylor and edited by Tycho Loke for actua use case
## Disclaimer

This script is provided as-is, and you bear the risk of using it. It is recommended to test the script in a controlled environment before deploying it in a production environment.
