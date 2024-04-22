Coses relatives a ClickControl.

.

* Windows

Els arxius per a windows estan al OneDrive de CoordinacioTIC. (És millor que vingen els tècnics, perquè és un procés llarg...)

Per a que se puga activar el Office365 en els usuaris ClickControl en Windows 10 cal agefir la següent entrada al regedit:

    HKEY_LOCAL_MACHINE\Software\Microsoft\Cryptography\Protect\Providers\df9d8cd0...  > Nuevo > DWORD > ProtectionPolicy = 1




* Ubuntu 22.04

Instalador-ClickControlDS-Ubuntu-x64 és un instal·lador per a poder iniciar sessió amb l'usuari de la intranet ClickControl, i així poder imprimir

Cal instalar java

    apt install default-jre

Configurar snap homedirs

    snap set system homedirs=/home,/datos/usuarios/profesores
