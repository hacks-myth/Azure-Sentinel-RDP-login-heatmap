# Azure-Sentinel-RDP-login-heatmap

[√] Description :
A honeypot used to track geolocation of RDP login attempts. The PowerShell script parses out Windows Event Log info and uses a third party API to collection geographical info about attacker's location.

To replicate, you must setup Azure Sentinel (SIEM) and connect a VM acting like a honey pot. Once log in attempts are logged in Event viewer, we will use PowerShell script to look up attacker's Geolocation and plot it on an Azure Sentinel Map.

Languages Used :
PowerShell: Extract RDP failed logon logs from Windows Event Viewer
Utilities Used
ipgeolocation.io: IP Address to Geolocation API

World map of incoming attacks after 24 hours (built custom logs including geodata)

![Failed RDP World Map 24hrs](https://user-images.githubusercontent.com/109769996/204385957-e285da13-d4f9-4bf0-a2b8-f16eedf7b7e4.jpg)


Credits:
@Josh Madakor https://github.com/joshmadakor1
