# AV/EPP/EDR Windows API hook list
Depending on the product you are dealing with from a red team perspective, the EPP/EDR will use usermod hooks to monitor red team activity. 
Most often they set their usermod hooks in ntdll.dll, but depending on the EPP/EDR they also use hooks in many other dlls. 
To learn more about this, take a look at the following nice blog post by **ZeroPeril** https://zeroperil.co.uk/blog/hookdump/

To check which APIs are hooked, I used the repo from zeroperil https://github.com/zeroperil/HookDump
The approach of this tool is in my opinion more reliable than others, because it does not only do simple checks for Nt or Zw inline API hooks.
