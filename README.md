# Kaseya-VSA-Event-Set-IOCs
Event set to be used with Kaseya VSA to catch sketchy happenings. If you get a hit on this you should almost certainly investigate as potential IOC.

This works if you have sysmon deployed to your kaseya agents. This event set is what I use internally for extra visibility into potential malicious activity. Recommend using [SwiftOnSecurity's Sysmon Config](https://github.com/SwiftOnSecurity/sysmon-config)

Entries are process names/commands/hashes of known ATP/Ransomware operators - sourced from various threat intel feeds. Simply import the event set and configure as desired.
More information on event sets can be found at [https://help.kaseya.com/WebHelp/en/VSA/6010000/index.htm?toc.htm?2886.htm](https://help.kaseya.com/WebHelp/en/VSA/6010000/index.htm?toc.htm?2886.htm)

Be sure that you apply this event set against the log source "Microsoft-Windows-Sysmon/Operational" and select the "informational" check box in event log alerts section of your VSA.
