---
Date: 2022-02-09
Author: Jimmy Briggs <jimmy.briggs@jimbrig.com>
Tags: ["#Type/Code/Registry", "#Topic/Dev/OS/Windows"]
Alias: ["Enable Long Path Support on Windows"]
---

# Enable Long Path Support on Windows

*Source: *

```powershell
Set-ItemProperty 'HKLM:\SYSTEM\CurrentControlSet\Control\FileSystem' -Name 'LongPathsEnabled' -Value 1
```

***

## Appendix: Links

- [[2-Areas/Code/_README|Code]]
- [[Development]]
- [[Windows]]
- [[Microsoft DOS]]
- [[Command Line]]
- [[PowerShell]]

*Backlinks:*

```dataview
list from [[Enable Long Path Support on Windows]] AND -"Changelog"
```