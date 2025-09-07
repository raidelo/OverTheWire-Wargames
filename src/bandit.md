# Bandit Solutions

## Bandit 0
Password => bandit0

## Bandit 0 -> 1
```
  cat readme
```
Password => ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

## Bandit 1 -> 2
```
  cat ./-
```
Password => 263JGJPfgU6LtdEvgfWU1XP5yac29mFx

## Bandit 2 -> 3
```
  cat "./--spaces in this filename--"
```
Password => MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

## Bandit 3 -> 4
```
  cat inhere/...Hiding-From-You
```
Password => 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

## Bandit 4 -> 5
Solution 1
```
  file inhere/*
  cat inhere/-file07
```
Solution 2
```
  find inhere -readable -a -type f | xargs file
  cat inhere/-file07
```
Solution 3
```
  python3
      >>> from pathlib import Path
      >>> for item in Path().iterdir():
      ...     with open(item, "rb") as file:
      ...             content = file.read()
      ...             try:
      ...                     print(content.decode())
      ...             except:
      ...                     print("---")
      ...
```
Password => 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

## Bandit 5 -> 6
Solution 1
```
  find -readable -and -not -executable -and -type f -and -size 1033c
  cat ./maybehere07/.file2
```
Solution 2
```
  find -readable -and -not -executable -and -type f -and -size 1033c | xargs cat
```
Password => HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

## Bandit 6 -> 7
Solution 1
```
  find / -size 33c -a -user bandit7 -a -group bandit6 2>/dev/null
  cat /var/lib/dpkg/info/bandit7.password
```
Solution 2
```
  find / -size 33c -a -user bandit7 -a -group bandit6 2>/dev/null | xargs cat
```
Password => morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

## Bandit 7 -> 8
```
  cat data.txt | grep millionth
```
Password => dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

## Bandit 8 -> 9
```
  cat data.txt | sort | uniq -u
```
Password => 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM

## Bandit 9 -> 10
```
  strings data.txt | grep "=\{2,\}[^=].*"
```
Password => FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey

## Bandit 10 -> 11
```
  cat data.txt | base64 -d
```
Password => dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr

## Bandit 11 -> 12
```
  cat data.txt | tr a-zA-Z n-za-mN-ZA-M
```
Password => 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4

## Bandit 12 -> 13
```
  cd /tmp
  mkdir tempdir
  cd tempdir
  cp ~/data.txt .
  xxd -r data.txt output
  mv output output.gz
  gzip -d output.gz
  bzip2 -d output
  mv output.out output.out.gz
  gzip -d output.out.gz
  tar -f output.out -x
  tar -f data5.bin -x
  bzip2 -d data6.bin
  tar -xf data6.bin.out
  mv data8.bin data8.bin.gz
  gzip -d data8.bin.gz
  cat data8.bin
```
Password => FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn

## Bandit 13 -> 14
```
  ssh bandit14@localhost -p 2220 -i sshkey.private
  cat /etc/bandit_pass/bandit14
```
Password => MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS

## Bandit 14 -> 15
```
  echo MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS | nc localhost 30000
```
Password => 8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo

## Bandit 15 -> 16
```
  openssl s_client localhost:30001
  8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
```
Password => kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx

## Bandit 16 -> 17
```
  nmap localhost -p 31000-32000 -Pn -n -sV
  openssl s_client -ign_eof localhost:31790
  kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx
  [Copy private key]
  cd /tmp
  mkdir tempdir
  cd tempdir
  vim ssh_key.pem
  [Paste Private Key]
  chmod 400 ssh_key.pem
  ssh bandit17@localhost -p 2220 -i ssh_key.pem
  cat /etc/bandit_pass/bandit17
```
Password => EReVavePLFHtFlFsjn3hyzMlvSuSAcRD

## Bandit 17 -> 18
```
  diff passwords.old passwords.new
```
Password => x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO

## Bandit 18 -> 19
Solution 1
[Commands of your local shell included]
```
  ssh bandit18@bandit.labs.overthewire.org -p 2220 "cat readme"]
```
Solution 2
[Commands of your local shell included]
```
  ssh bandit18@bandit.labs.overthewire.org -p 2220 -T]
  cat readme
```
Solution 3
[Commands of your local shell included]
```
  ssh bandit18@bandit.labs.overthewire.org -p 2220 "cat /etc/shells"]
```
... and then ...
```
  ssh bandit18@bandit.labs.overthewire.org -p 2220 -t "/bin/sh"]
  cat readme
```
... or ...
```
  ssh bandit18@bandit.labs.overthewire.org -p 2220 -t "/bin/dash"]
  cat readme
```
Password => cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8

## Bandit 19 -> 20
```
  ./bandit20-do cat /etc/bandit_pass/bandit20
```
Password => 0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO

## Bandit 20 -> 21
```
  echo 0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO | nc -l 8082 &
  ./suconnect 8082
```
Password => EeoULMCra2q0dSkYj561DX7s1CpBuOBt

## Bandit 21 -> 22
```
  cat /etc/cron.d/cronjob_bandit22
  cat /usr/bin/cronjob_bandit22.sh
  cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
```
Password => tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q

## Bandit 22 -> 23
```
  cat /etc/cron.d/cronjob_bandit23
  cat /usr/bin/cronjob_bandit23.sh
  cat /tmp/$(echo I am user bandit23 | md5sum | cut -d ' ' -f 1)
```
Password => 0Zf11ioIjMVN551jX3CmStKLYqjk54Ga

## Bandit 23 -> 24
```
  cat /etc/cron.d/cronjob_bandit24
  cat /usr/bin/cronjob_bandit24.sh
  touch /tmp/tempfile
  chmod o+w /tmp/tempfile
  echo "cat /etc/bandit_pass/bandit24 > /tmp/tempfile" > /var/spool/bandit24/foo/script.sh
  chmod o+x /var/spool/bandit24/foo/script.sh
  [Wait 60 seconds or less]
  /tmp/tempfile
```
Password => gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8

## Bandit 24 -> 25
```
  [Copy last level's password]
  mkdir /tmp/tempdir
  cd /tmp/tempdir
  seq -w 0 9999
  vim file
  [Just opened VIM in normal mode. Press: ctrl+v G I]
  [Just opened insert mode. Paste the last level's password and insert a space. Then press ESC. And then exit vim with: :x]
  cat file | nc localhost 30002
```
Password => iCi86ttT4KSNe1armKiwbQNmB3YJP3q4

## Bandit 25 -> 26
```
  [Make your terminal small in the Y axis, then log in with ssh]
  [You should be in the interactive mode of the "more" program, reading the /home/bandit26/text.txt file]
  [Press v to open the vi/vim editor. Press: :set shell=/bin/bash]
  [Press: `:!bash`]
  [Then to find the password of the current level (bandit26) you can execute `cat /etc/bandit_pass/bandit26` or directly press `:!cat /etc/bandit_pass/bandit26`]
  [The step above isn't necesary since you'll face the same problem when logging with the password. You need to find the password of the next level in this bash you got.]
```
Password => s0773xxkk0MXfdqOfPRVr9L3jJBUOgCZ

## Bandit 26 -> 27
```
  ./bandit27-do cat /etc/bandit_pass/bandit27
```
Password => upsNCc7vzaRDx6oZC6GiR6ERwe1MowGB

## Bandit 27 -> 28
```
  mkdir /tmp/tempdir
  cd /tmp/tempdir
  git clone ssh://bandit27-git@localhost:2220/home/bandit27-git/repo
  cd repo
  cat README.md
```
Password => Yz9IpL0sBcCeuG7m9uQFt8ZNpS4HZRcN

## Bandit 28 -> 29
```
  mkdir /tmp/tempdir
  cd /tmp/tempdir
  git clone ssh://bandit28-git@localhost:2220/home/bandit28-git/repo
  cd repo
  git log --oneline
  git show 68314e0
```
Password => 4pT1t5DENaYuqnqvadYs1oE4QLCdjmJ7

## Bandit 29 -> 30
```
  mkdir /tmp/tempdir
  cd /tmp/tempdir
  git clone ssh://bandit29-git@localhost:2220/home/bandit29-git/repo
  cd repo
  git checkout dev
  cat README.md
```
Password => qp30ex3VLz5MDG1n91YowTv4Q8l7CDZL

## Bandit 30 -> 31
```
  mkdir /tmp/tempdir
  cd /tmp/tempdir
  git clone ssh://bandit30-git@localhost:2220/home/bandit30-git/repo
  cd repo
  git show secret
```
Password => fb5S2xb7bRyFmAvQYQGEqsbhVyJqhnDy

## Bandit 31 -> 32
```
  mkdir /tmp/tempdir
  cd /tmp/tempdir
  git clone ssh://bandit31-git@localhost:2220/home/bandit31-git/repo
  cd repo
  cat README.md
  echo May I come in? > key.txt
  git add key.txt
  git commit -m "the asked file"
  git push origin master
```
Password => 3O9RfhqyAlVBEZpVb6LYStshZoqoSx5K

## Bandit 32 -> 33
```
  $0
  cat /etc/bandit_pass/bandit33
```
Password => tQdtbs5D5i2vJwkO8mEyYEyTL8izoeJ0
