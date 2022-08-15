# Overthewire Hackdays writeup

# Lvl 0
cat readme

# lvl 1 
cat ~/-

# lvl 2
cat "spaces in filename"

# lvl 3
cat inhere/.hidden

# lvl 4
zkusit cat na vsechno nestoji za to psat si na to script

# lvl 5
find . -size 1033c

# lvl 6
find / 33c

# lvl 7
grep "millionth" data.txt

# lvl 8
sort data.txt | uniq -u

# lvl 9
strings data.txt | grep "====="

# lvl 10
cat data.txt | base64 -d

# lvl 11
cat data.txt, vlozit do https://gchq.github.io/CyberChef/#recipe=ROT13(true,true,false,13)

# lvl 12
mkdir /tmp/ssps
cp data.txt /tmp/ssps
cd /tmp/ssps
xxd -r data.txt > file
mv file file.gz
gzip -d file.gz
...

# lvl 13
cat sshkey.private
zkopirovat
echo ${KEY} > bandit.key
chmod 400 bandit.key
ssh -i bandit.key bandit14@bandit.labs.overthewire.org -p 2220

### na winech jsem pouzil vscode

# lvl 14
cat /etc/bandit_pass/bandit14 | nc localhost 30000

# lvl 15
ncat --ssl localhost 30001
zadat heslo

# lvl 16
nmap localhost -p 31000-32000
zkouset nalezeny porty
ncat --ssl localhost 31790

# lvl 17
diff passwords.new passwords.old
