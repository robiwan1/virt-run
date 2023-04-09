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
20220422,ha: add --osinfo detect=on,require=off
20230409,ha: add default for NEW VMs -d|DEF
# 
USAGE: virt-run [-d DSK:RAM:CPU] [VM-name|VM-dir|VM-arch]
default values for   4G  2G   1
# 
Create and run a VM just by creating an empty Directory (i.a. /data/VM/MyVM) and a Desktop Launcher with the command "/usr/bin/virt-run /data/VM/MyVM". Than doubleclick the launcher, and install any OS... 
Examples:
create a simple VM called "Linux" with 4G Disk, 2G RAM and 1 CPU
  mkdir /data/VM/Linux; virt-run /data/VM/Linux
create a Windows 11 VM called "Win11" with 64G Disk, 4G RAM and 2 CPU ()
    mkdir /data/VM/Win11; virt-run -d 64:4:2 /data/VM/Win11
