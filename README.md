Mimikatz is a powerful post-exploitation tool that allows attackers to extract passwords, Kerberos tickets, and other authentication credentials from Windows systems. 
It is widely used for credential dumping, pass-the-hash attacks, and Kerberos ticket manipulation. The tool is used by security professionals, 
penetration testers, and red teamers to assess security weaknesses in Windows environments.

Usage
Running Mimikatz 
./mimikatz.exe
Once you've compiled or downloaded Mimikatz, you can execute the tool and start using its commands. Below are some example commands to use Mimikatz for common tasks:

1. Extracting Plaintext Passwords and NTLM Hashes
To extract passwords and hashes stored in memory, use the following command:
sekurlsa::logonpasswords

2.Extracting Kerberos Tickets
To view Kerberos tickets (TGTs and TGSs) from memory:
kerberos::tickets

3.Pass-the-Hash Authentication
sekurlsa::pth /user:<username> /domain:<domain> /hash:<NTLM_hash>
