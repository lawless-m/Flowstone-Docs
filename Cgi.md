# CGI

Common Gateway Interface - It's a fantastic way of returning data from an HTTP request. The server spawns a process that processes the request. returns data in a http format. It just puts the headers in, tells you what sort of file it is, and then bangs out the rest of the file in the appropriate MIME format. 

Means you don't have to have long-running servers just to get data. You don't have to have ASP files or PHP files. They can be written in whatever programming language you want so long as it conforms to the HTTP header MIME format.

Often overlooked in these modern times. People will tell you it's slow because it forks a new process because in the 1990s forking a new process was slow. It's no longer the 1990s. 

 

