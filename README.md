# Exploit for Easy RM to MP3 converter for OSCE practice

## Tested on:
* WIN XP SP3
* Easy RM to MP3 Converter 2.7.3.700

Based on article: https://www.corelan.be/index.php/2009/07/23/writing-buffer-overflow-exploits-a-quick-and-basic-tutorial-part-2/

inspired by: http://www.securitysift.com/windows-exploit-development-part-4-locating-shellcode-jumps/

## Shellcode for popping calc created by:
`msfvenom -a x86 -p windows/exec CMD=calc.exe -f python -b '\x00' --var-name shellcode -e x86/shikata_ga_nai EXITFUNC=seh`
