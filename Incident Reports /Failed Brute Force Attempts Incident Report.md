## Findings

Time: 2026-10-20 16:43:37 UTC </br>
Hosts: SOC-FW-RDP, SHIR-Hive </br>
Accounts: \admin, \ADMIN, \administrator, \ADMINISTRATOR

## Investigation

On 2026-10-20 16:43:37 UTC, the alert for FailedLogon was triggered for the following accounts: \ADMIN with 1196 failed logons, \administrator with 3728, \admin with 3978, and \ADMINISTRATOR with the most failed logons with 20510. \ADMINISTRATOR and \ADMIN tried to login to the computer SOC-FW-RDP while \administrator and \admin tried to login to SHIR-Hive. It was found that there were no successful login attempts to these accounts. 

WHO - Accounts: \ADMINISTRATOR, \administrator, \ADMIN, \admin </br>
WHAT - A failedlogon alert was triggered where it detected failed brute force attempts on four distinct accounts that totaled to 28,456 attempts. </br>
WHEN - This alert was triggered on 2026-10-20 16:43:37 UTC. </br>
WHERE - This occurred on the computers SOC-FW-RDP and SHIR-Hive </br>
WHY - Due to insufficient information, it could not be determined why these failed brute force attempts occurred on these systems. </br>
HOW - Due to insufficient information, it could not be determined how these failed brute force attempts occurred. </br>

## Recommendations

- Ensure MFA is enabled for the accounts listed. 
- Gather additional telemetry to investigate the source of these failed brute force attempts. 
- Investigate why there are multiple admin accounts, are multiple admin accounts needed, and identify if accounts are inactive and need to be off-boarded. 
