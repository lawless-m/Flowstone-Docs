# dw.ramsden-international.com

Intranet host and SSL-terminating reverse proxy for internal services. Apache on RIVSPROD01 (Linux) fronts TinyWeb, CGI executables, Gogs, and other backend services so everything is reachable over HTTPS on a single domain.

## Hosted services

- [[HTMLDataTable]] — CGI query engine at `/tiny02/cgi-bin/HTMLDataTable.exe`
- [[Anthea]] — price lookup at `/tiny02/anthea.html`
- [[Dingo]] — biosecurity declarations at `/tiny02/dingo.html`
- [[Declotter]] — product description compressor at `/tiny02/cgi-bin/Declotter-Web-CGI.exe`
- [[Dressage]] — address normalisation at `/tiny02/cgi-bin/Dressage.Cgi.exe`
- [[BPQuery]] — business partner query at `/bpquery/`
- [[PBI-Liveboards]] — sales and availability dashboards at `/tiny02/pibs/`
- [[Gogs]] — Git hosting at `/gogs/`
- [[R.I.S.E]] — browser extension distribution at `/R.I.S.E./`
- [[MonkeyTamper]] — userscript auto-update hosting

## Also referenced by

- [[CGI-Sharp]] — produces the CGI executables deployed here
- [[ExcelMacros]] — fetches product images from this domain
- [[Hedwigg]] — loads company logo from this domain
- [[PowerQueries]] — fetches data from HTMLDataTable endpoints here
- [[EM-Document-Scripts]] — Gogs repo hosted here

## Related themes

- [[Gogs]] — Git hosting on this domain
- [[csharp]] — most backend services are .NET CGI executables
- [[javascript]] — frontend apps served as static HTML
