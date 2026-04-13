# NPSFail2Ban

A [[csharp]] NPS authentication failure monitor that emails daily digest reports with Excel attachments identifying IPs to block.

**Repo:** `~/Git/NPSFail2Ban`
**Themes:** [[csharp]], [[dotnet]]

NPSFail2Ban queries NPS RADIUS accounting data from SQL Server, classifies failed authentication attempts into four categories (wrong profile, invalid username, not in AD, wrong password), and emails a daily report to IT with per-IP aggregation and repeat offender tracking. Runs as a scheduled task on rivsprod02.

## Related

- [[csharp]]
- [[dotnet]]
