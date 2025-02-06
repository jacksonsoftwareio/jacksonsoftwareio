---
title: Hugo playground
type: page
menu: "main"
---

This page is for playing with the Hugo framework

**Get latest Windows Update install date**

{{< highlight powershell >}}

# PowerShell script to get the latest Windows update timestamp
$UpdateHistory = Get-WmiObject -Class "Win32_QuickFixEngineering" | Sort-Object -Property InstalledOn -Descending

if ($UpdateHistory) {
    $LatestUpdate = $UpdateHistory[0]
    Write-Host "Latest Windows Update installed on: $($LatestUpdate.InstalledOn)"
} else {
    Write-Host "No updates found."
}

{{< /highlight >}}

{{< youtube dQw4w9WgXcQ >}}

