# Get-MACVendor.ps1

## Description
This PowerShell script searches the IEEE's database of vendors/MAC addresses to find the vendor of your query (given MAC address).

## How to use
```
.\Get-MACVendor.ps1 -MAC 00:12:23
.\Get-MACVendor.ps1 -MAC 00-12-23
.\Get-MACVendor.ps1 -MAC 001223
.\Get-MACVendor.ps1 -MAC 00:12:23:45:54:32
```
The script will output: *Pixim*

## Downloading/Updating the OUI list
```
.\Get-MACVendor.ps1 -Action Update
```
The script will pull a fresh version of the OUI list from <a href='http://standards-oui.ieee.org/oui.txt'>http://standards-oui.ieee.org/oui.txt</a>.

## Requirements
In order to use this script, please keep the file: *vendors.txt* in the same folder as the script.  This file contains the relationships between certain MAC addresses and vendors.
