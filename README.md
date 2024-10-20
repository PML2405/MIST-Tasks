# Bandit(overthewire.org)

`Level 0`<br>
Start with this in terminal 
ssh bandit0@bandit.labs.overthewire.org -p 2220
<br>
password: bandit0
<br><br>
`Level 0 to Level 1`<br>
Just do 
ls
then access the readme file by doing
cat readme<br>
Password: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If<br><br>
`Level 1 to Level 2`<br>
Now to access the file with name “–“
We do 
cat ./-
password: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx<br><br>
`Level 2 to Level 3`<br>
cat ‘spaces in this filename’
password: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx<br><br>
`Level 3 to Level 4`<br>
Do
find inhere
cd inhere
cat …Hiding-From-You<br>
password: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ<br><br>
`Level 4 to Level 5`<br>
cd inhere
file ./* (to check the file type of every file in the inhere directory)
cat ./-file07 (ASCII file type)<br>
password: 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw<br><br>
`Level 5 to Level 6`<br>
 cd inhere -> find -size 1033c
cat ./maybehere07/.file2<br>
password: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG<br><br>
`Level 6 to level 7`<br>
find / -type f -user bandit7 -size 33c -group bandit6 2> /dev/null
cat /var/lib/dpkg/info/bandit7.password<br>
password: morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj<br><br>
`Level 7 to Level 8`<br>
grep millionth data.txt<br>
password: dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc<br><br>
`Level 8 to 9`<br>
cat data.txt | sort | uniq -u<br>
password: 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM<br><br>
`Level 9 to 10`<br>
cat data.txt | strings -e s| grep == <br>
password: FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey<br><br>
`Level 10 to 11`<br>
cat data.txt | base64 -d<br>
password: dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr<br><br>
`Level 11 to 12`<br>
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'<br>
password: 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4<br><br>
`Level 12 to 13`<br>
mktemp -d
cd /tmp/tmp.ce9aRFHzbF
cp ~/data.txt .
mv data.txt data
xxd -r data > binary
mv binary binary.gz
gunzip binary.gz
bunzip2 binary
mv binary.out binary.gz
gunzip binary.gz
tar -xf binary
rm binary data
tar -xf data5.bin
rm data5.bin
bunzip2 data6.bin
tar -xf data6.bin.out
rm data6.bin.out
mv data8.bin data8.gz
gunzip data8.gz
finally when we do file data8
we get that it’s a ASCII text
cat data8<br>
password: FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn<br><br>
`Level 13 to 14`<br>
ssh -i sshkey.private -p 2220 bandit14@localhost
cat /etc/bandit_pass/bandit14<br>
password: MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS<br><br>
`Level 14 to 15`<br>
netcat localhost 30000 MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS<br>
password: 8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo<br><br>
`Level 15 to 16`<br>
openssl s_client -connect localhost:30001 8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo<br>
password: kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx<br><br>

