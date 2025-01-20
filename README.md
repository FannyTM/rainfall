## How to create a VM with QEMU :

qemu-system-x86_64 -m 4G -smp 4 -cpu host -enable-kvm -cdrom /tmp/RainFall.iso  -net nic -net user,hostfwd=tcp::2222-:4242 -daemonize

## How to connect :

ssh level00@localhost -p 2222
password: level00

## How to use scp (dl with secure protocole) :

scp -P 2222 level00@localhost:~/ /tmp

## How to get the flag :

level00@RainFall:~$ su flag00
Password:
Don't forget to launch getflag !
flag00@RainFall:~$ getflag
Check flag.Here is your token : ?????????????????
flag00@RainFall:~$ su level01
Password:
level01@RainFall:~$ 


