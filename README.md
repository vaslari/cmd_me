Comandos que me facilitan la vida como SysAdmin

## Mensaje en Ventana en Windows a traves de cmd
    msg * "Something to say"
    powershell -WindowStyle hidden -Command "& {[System.Reflection.Assembly]::LoadWithPartialName('System.Windows.Forms'); [System.Windows.Forms.MessageBox]::Show('Mensaje de prueba','ATENCION')}"


## docker añadir a grupo por cmd Windows
    net localgroup docker-users some_user /add


## install IntelliJ
    start openvpn-gui --command disconnect_all
    rasdial "some_VPN" /disconnect
    rasdial "some_other_VPN" /disconnect
    mkdir "c:\some_directory"
    cd "c:\some_directory"
    C:\WINDOWS\System32\WindowsPowerShell\v1.0\Powershell wget https://download.jetbrains.com/idea/ideaIC-2021.2.2.exe -outfile "ideaIC-2021.2.2exe"
    ideaIC-2021.2.2.exe /S

## Create a new repository on the command line
    touch README.md
    git init
    git add README.md
    git commit -m "first commit"
    git remote add origin git@github.com:vaslari/cmd_me.git
    git push -u origin master

## Push an existing repository from the command line
    git remote add origin git@github.com:vaslari/cmd_me.git
    git push -u origin master

## remoto bitlocker metodos informacion(si tiene password se puede activar)
    manage-bde c: -protectors -get

## Remoto bitlocker activar
    manage-bde -on C:

## Proxmox log 
    journalctl -u proxmox-backup -u proxmox-backup-proxy

## Proxmox Configuration VM
    /etc/pve/qemu-server/700.conf
    /etc/pve/qemu-server/100.conf
    /etc/pve/qemu-server/200.conf