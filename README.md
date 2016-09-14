Open Validation Server v3 is a free online service for validating IGC files, 
used by the FAI CIVL World XC Online Contest and many other national and international flying contests. 
More details, and a running version at http://vali.fai-civl.org/

Prerequisites, recommended Installation:

Installed Apache2 + Perl + PHP on Windows 32bit or 64bit platform
  for example using xampp on Windows 7 or Windows 2008
  see www.apachefriends.org/en/xampp.html?
  
More Details at INSTALL.txt and at http://vali.fai-civl.org/

<b>Q:</b> What's the difference to Open Validation Server v2 Version ?<br>
A: This Version here (v3) contains also an simple PHP interface (MVC implementation).
It is the version you will see, when you visit http://vali.fai-civl.org/ .
 The V3 implements also a JSON response feature for validation requests, 
and we have added a more nice public web interface for igc file validations.

<b>Q:</b> Which version to choose if you want to implement your own Server ?<br>
A: If you want to run just your own background service, lets say for LeonardoXC, then you are fine with vali2 from github.
If you want to host the same public web interface like seen on vali.fai-civl.org, then you need a clone of vali3 from github,
and modify the content to your needs.

<b>Q:</b> Can I collect all vali.exe files from this github repository here, to develop my own implementation ?<br>
A: Sure you can. By the way, the general testing platform is Linux/Wine, because some online contests 
already run their own validation implementation, rather then using the OpenValidation Server.
Make sure you use wine 1.7.55 or later as of some newer crypto libary requirements for some vali.exe binaries.

<b>Open ToDo's at this v3 project:</b><br>
- Migrating from OpenID 2.0 to OpenID Connect for the Admin Login (current simply disabled).