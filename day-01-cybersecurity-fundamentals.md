# Day 1: Cybersecurity Fundamentals

## Objective
Practise basic Linux commands, inspect network connectivity, and understand file permissions.

## 1. Network Checks
- `ping -c 4 1.1.1.1` — Tested internet connectivity.
- `nslookup google.com` — Tested DNS resolution.
- `ip route` — Inspected the routing table.
- Result: Ping received 4 packets with 0% packet loss, DNS resolved successfully, and routing entries were displayed.

## 2. Linux File Permissions
- `touch practice.txt` — Created a practice file.
- `echo day1-practice > practice.txt` — Wrote text into the file.
- `cat practice.txt` — Displayed the file contents.
- `chmod 600 practice.txt` — Restricted file access to the owner.
- `stat -c "%A %a %n" practice.txt` — Verified permissions.

## 3. Permission Verification
Observed permissions: `-rw-------`
Numeric mode: `600`

Meaning:
- Owner: read and write.
- Group: no permissions.
- Others: no permissions.

## 4. World-Writable File Check
Command:
`find ~/cybersecurity-day1 -type f -perm -0002 -ls`

Result: No matching files were found in the practice directory.

## 5. Learning Outcome
Practised Linux navigation, basic network troubleshooting, file creation, and permission verification.

## Evidence
Add screenshots of the command outputs before submitting the internship task.
