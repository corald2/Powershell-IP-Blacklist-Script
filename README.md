# Powershell-IP-Blacklist-Script
This script adds a range of IP addresses to a Blacklist

**Before Running:**

1. **Review and Adjust IP Ranges** in the script to match your intentions.
2. **Test with a Small Range** first to ensure the script behaves as expected in your environment.
3. **Ensure You Have Permissions** to modify firewall rules.

**To Run:**

1. Open PowerShell as **Administrator**.
2. Navigate to the directory where you saved the script (using `cd "Path\To\Script"`).
3. Execute the script with `.\ScriptName.ps1` (ensure the script's extension is `.ps1`).

**Important Note on Bulk IP Blocking:**
- Blocking a vast range of IPs (like from 100.0.0.0 to a high end IP) can lead to performance issues with the Windows Firewall due to the sheer number of rules. 
- For large IP ranges, consider:
  - **Using IP Ranges or Subnets** in a single rule where possible (the script above adds one rule per IP for simplicity and to meet the request, but this is not efficient for large ranges).
  - **External Firewall Devices/Appliances** for more efficient IP blocking at scale.
  - **Regular Review** of blocked IPs to remove unnecessary entries.
