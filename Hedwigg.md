# Hedwigg

A [[CSharp]] desktop notice widget that displays corporate announcements in an always-visible, chromeless window using Avalonia and WebView2.

**Repo:** `~/Git/Hedwigg`

Hedwigg embeds a WebView2 browser control in an Avalonia window that sits above the wallpaper but below all other windows — persistent, undismissable, and deployed to ~100 machines via Group Policy. The notice content comes from an internal web app on rivsprod02. Supports urgent/important/normal priority levels, Windows Integrated Authentication, and Freshdesk integration. Hosted on [[Gogs]] at [[Dw.ramsdenInternational.com]].
