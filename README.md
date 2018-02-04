# ssh-ad-pubkey
Manage SSH public keys stored in ActiveDirectory

## Motivation

With Windows 10 Build 1709 and Windows Server 2016 the  OpenSSH client and server is available as an optional feature. OpenSSH for Windows is still in Beta. You can use it from command line or with PowerShell instead of WinRM. The idea was to make a tool like ssh-ldap-pubkey based on PowerShell. It should run on Windows PowerShell 2-5.1 and PowerShell Core 6.x. Unfortunately the .Net 3.5 assemblies for Active Directory Access are only available for Windows and not Linux or Mac. 

## Problem
At the time of writing the code it wasn't clear to me that the option AuthorizedKeysCommand is out of project scope because Windows don't support a fork. This is why you can't use a wrapper for OpenSSH server under Windows who fetch the SSH Public Key of the user!


## Links
https://github.com/jirutka/ssh-ldap-pubkey

https://github.com/PowerShell/Win32-OpenSSH


