---
title: Bash
description: default terminal scripting language
published: true
date: 2020-05-20T04:11:04.335Z
tags: 
---

## Basic Commands

Intro to Bash in Asciinema: https://asciinema.org/a/101528

cd
cd -

pwgen -syn1 20
kill -9 $MYPID
source ~/.bashrc
tail -f /var/log/syslog
tail -f /var/log/syslog -n 50
cat ~/.bashrc
dmesg

man sort
find ~ -iname ".bash*"
watch -n10 free -h
sysctl -a
which psw
which top
which lnd

systemctl status network-manager
systemctl stop network-manager
systemctl disable network-manager
systemctl enable network-manager
systemctl start network-manager

df -Th
du -sh *
lsblk
lshw
lspci -v
blkid
lsof
uname -a
fsck /dev/sda
dmidecode
smartctl -i /dev/sda

git status
git log
git tag
git diff
git remote -v
git stash
git checkout -b $MYBRANCH

tmux
tmux ls
tmux a
tmux a -t0

ps aux
top
htop
free
clear
!!
history
history | sort -t' ' -k2

cp $MYFROM $MYTO
mv $MYFROM $MYTO
scp $MYFROM $MYTO
rsync -aP $MYFROM $MYTO
export $MYTHING

echo -n "HELLO WORLD" > $MYFILE
echo -n "HELLO WORLD" >> $MYFILE
ln -s $MYTHING $MYREF

seq 1 10
seq 10 -1 1

sync
reboot now
shutdown now

for i in {1..10}
do
  echo -n "$i"
done

for i in {1..10}
do
  echo "$i"
done

for i in {1..10}; do echo "$i"; done

while true; do free -h; sleep 5; done


## Permissions Management

ls -lA
chmod 600 $MYFILE
chmod a+x $MYFILE
chmod o-w $MYFILE
chown brandon: $MYFILE

passwd
ip addr
lsusb -v
groups
groupadd $MYGROUP
usermod $MYUISER -aG $MYGROUP