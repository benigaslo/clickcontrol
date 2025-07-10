Coses relatives a ClickControl.



* Windows 10

Els arxius per a windows estan al OneDrive de CoordinacioTIC. (És millor que vingen els tècnics, perquè és un procés llarg...)

Per a que se puga activar el Office365 en els usuaris ClickControl en Windows 10 cal afegir la següent entrada al regedit:

    HKEY_LOCAL_MACHINE\Software\Microsoft\Cryptography\Protect\Providers\df9d8cd0...  > Nuevo > DWORD > ProtectionPolicy = 1




* Ubuntu 22.04

`Instalador-ClickControlDS-Ubuntu-x64` és un instal·lador per a poder iniciar sessió amb l'usuari de la intranet ClickControl, i així poder imprimir

Lo ideal és configurar el accés a Ubuntu amb CDC (@gva) i instal·lar ClickControl en mode "Cliente Centro Inteligente - Sistema Impresión", IP del servidor: 192.168.1.250, No añadir impresioras ni apagado automático.

Cal instalar java

    apt install default-jre


Si s'accedeix a Ubuntu amb usuaris ClickControl, cal configurar snap homedirs:

    snap set system homedirs=/home,/datos/usuarios/profesores


* Lliurex 23

Executar `Instalador-ClickControlDS-Ubuntu-x64` en mode "Cliente Centro Inteligente - Sistema Impresión", IP del servidor: 192.168.1.250, No añadir impresioras ni apagado automático.
Asegurarse de que el fichero /clickcontrol/config.properties té esto:
```
#Configuracion
server-ip=192.168.1.250
server-port=9191
server-name=fsserver
background-color=FFFFFF
```
