# virt-run
start DOMAIN with VM-name, or
create a VM/DOMAIN with VM-dir, or
extract and create a VM with VM-arch.<br>
VM-arch can be: RAR,ZIP,TAR,OVA,TGZ
# 
20200629,ha: added --clock option...<br>
20200813,ha: run RUNME if found in VM-dir<br>
20201126,ha: if no disk found, create one<br>
20201205,ha: add XML export of VM config
# 
USAGE: virt-run [VM-name|VM-dir|VM-arch]
# 
Create and run a VM just by creating an empty Directory (i.a. /data/VM/MyVM) and a Desktop Launcher with the command "/usr/bin/virt-run /data/VM/MyVM". Than doubleclick the launcher, and install any OS... 
