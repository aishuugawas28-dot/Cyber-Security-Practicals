# Linux Log Analysis Practical

## About
This practical uses Kali Linux to inspect system logs, review login-session records, and identify authentication-related events.

## Tools Used
- Kali Linux Terminal
- `journalctl`
- `grep`
- `who`
- `last`

## Commands Used
```bash
ls -lh /var/log/
who
last -n 10
sudo grep -i 'failed password' /var/log/auth.log | tail -20
sudo journalctl -u ssh --no-pager -n 30
sudo journalctl --no-pager | grep -Ei 'failed password|authentication failure|invalid user' | tail -20
```

## Findings and Analysis
- Older authentication-failure messages appeared for `lightdm` and `xfce4-screensaver-dialog`.
- The SSH service query returned `-- No entries --` in the captured output.
- Two matching records in the current-day filtered query were `sudo` command records generated while running the search. They are not confirmed failed login attempts.
- The captured evidence does not establish malicious activity. Log entries should be interpreted in context.

## Screenshots
The `screenshots/` folder contains screenshot evidence extracted from the practical documentation. The original documentation is also included.

## Conclusion
Linux log analysis helps investigate login sessions and authentication events. Further contextual investigation is needed before classifying an event as suspicious.

## Disclaimer
This practical is for educational purposes and uses logs from the lab environment. Observed authentication-failure messages alone do not prove malicious activity.
