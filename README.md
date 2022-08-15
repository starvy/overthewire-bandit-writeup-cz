# Overthewire Hackdays writeup

# Lvl 0
`cat readme`

# lvl 1 
`cat ~/-`

# lvl 2
`cat "spaces in filename"`

# lvl 3
`ls -altr`
`cat inhere/.hidden`

# lvl 4
zkusit cat na vsechno, nestoji za to psat si na to script

# lvl 5
`find . -size 1033c`

# lvl 6
`find / 33c -group bandit6`

# lvl 7
`grep "millionth" data.txt`

# lvl 8
`sort data.txt | uniq -u`

# lvl 9
`strings data.txt | grep "====="`

# lvl 10
`cat data.txt | base64 -d`

# lvl 11
`cat data.txt`

vlozit do https://gchq.github.io/CyberChef/#recipe=ROT13(true,true,false,13)

# lvl 12
`mkdir /tmp/ssps`

`cp data.txt /tmp/ssps`

`cd /tmp/ssps`

`xxd -r data.txt > file`

`mv file file.gz`

`gzip -d file.gz`

opakovat z ruznejma formatama

...

# lvl 13
`cat sshkey.private`

zkopirovat

`echo ${KEY} > bandit.key`

oprávnění v linuxu `chmod 400 bandit.key`

`ssh -i bandit.key bandit14@bandit.labs.overthewire.org -p 2220`

### na winech jsem pouzil vscode

# lvl 14
`cat /etc/bandit_pass/bandit14 | nc localhost 30000`

# lvl 15
`ncat --ssl localhost 30001`
vložit poslední heslo

# lvl 16
`nmap localhost -p 31000-32000`
zkouset nalezeny porty
`ncat --ssl localhost 31790`
vložit poslední heslo
# lvl 17
`diff passwords.new passwords.old`

# lvl 18
`ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme`

# lvl 19
`./bandit20-do whoami`

`./bandit20-do cat /etc/bandit_pass/bandit20`

# lvl 20
pripojim se pres ssh ze dvou tabu terminalu
### TAB 1
`nc -lvnp 8080`
po spuštění `./suconnect 8080` v druhym tabu mám netcat připojení a vložim heslo získané z minulého levelu

### TAB 2
`./suconnect 8080`

