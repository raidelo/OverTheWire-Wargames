bandit0: bandit0

bandit0-bandit1: [
    Steps:
        cat readme
] =>  ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

bandit1-bandit2: [
    Steps:
        cat ./-
] => 263JGJPfgU6LtdEvgfWU1XP5yac29mFx

bandit2-bandit3: [
    Steps:
        cat "./--spaces in this filename--"
] => MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

bandit3-bandit4: [
    Steps:
        cat inhere/...Hiding-From-You
] => 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

bandit4-bandit5: [
    Steps:
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
] => 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

bandit5-bandit6: [
    Steps 1:
        find -readable -and -not -executable -and -type f -and -size 1033c
        cat ./maybehere07/.file2

    Steps 2:
        find -readable -and -not -executable -and -type f -and -size 1033c | xargs cat
] => HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

bandit6-bandit7: [
    Steps 1:
        find / -size 33c -a -user bandit7 -a -group bandit6 2>/dev/null
        cat /var/lib/dpkg/info/bandit7.password

    Steps 2:
        find / -size 33c -a -user bandit7 -a -group bandit6 2>/dev/null | xargs cat
] => morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

bandit7-bandit8: [
    Steps:
        cat data.txt | grep millionth
] => dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

bandit8-bandit9: [
    Steps:
        cat data.txt  | sort | uniq -u
] => 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM

bandit9-bandit10: [
    Steps:
        strings data.txt | grep "=\{2,\}[^=].*"
] => FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey

bandit10-bandit11: [
    Steps:
        cat data.txt  | base64 -d
] => dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr

bandit11-bandit12: [
    Steps:
        cat data.txt | tr a-zA-Z n-za-mN-ZA-M
] => 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4

bandit12-bandit13: [
    Steps:
        cd /tmp
        mkdir tempdir
        cd tempdir
        cp ~/data.txt .
        xxd -r data.txt output
        mv output output.gz
        gzip -d output.gz
        bzip2 -d output
        mv output.out  output.out.gz
        gzip -d output.out.gz
        tar -f output.out -x
        tar -f data5.bin -x
        bzip2 -d data6.bin
        tar -xf data6.bin.out
        mv data8.bin data8.bin.gz
        gzip -d data8.bin.gz
        cat data8.bin
] => FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn

bandit13-bandit14: [
    Steps:
        ssh bandit14@localhost -p 2220 -i sshkey.private
        cat /etc/bandit_pass/bandit14
] => MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS

bandit14-bandit15: [
    Steps:
        echo MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS | nc localhost 30000
] => 8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo

bandit15-bandit16: [
    Steps:
        openssl s_client localhost:30001
        8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
] => kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx

bandit16-bandit17: [
    Steps:
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
] => EReVavePLFHtFlFsjn3hyzMlvSuSAcRD

bandit17-bandit18: [
    Steps:
        diff passwords.old passwords.new
] => x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO

bandit18-bandit19: [
    Steps 1:
        [Before logging in => ssh bandit18@bandit.labs.overthewire.org -p 2220 "cat readme"] 

    Steps 2:
        [Before logging in => ssh bandit18@bandit.labs.overthewire.org -p 2220 -T] 
        cat readme

    Steps 3:
        [Before logging in => ssh bandit18@bandit.labs.overthewire.org -p 2220 "cat /etc/shells"]
        Steps 3.1:
            [Before logging in => ssh bandit18@bandit.labs.overthewire.org -p 2220 -t "/bin/sh"]
            cat readme
        Steps 3.2:
            [Before logging in => ssh bandit18@bandit.labs.overthewire.org -p 2220 -t "/bin/dash"]
            cat readme
] => cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8

bandit19-bandit20: [
    Steps:
        ./bandit20-do cat /etc/bandit_pass/bandit20
] => 0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO

bandit20-bandit21: [
    Steps:
        echo 0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO | nc -l 8082 &
        ./suconnect  8082
] => EeoULMCra2q0dSkYj561DX7s1CpBuOBt

bandit21-bandit22: [
    Steps:
        cat /etc/cron.d/cronjob_bandit22
        cat /usr/bin/cronjob_bandit22.sh
        cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
] => tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q

bandit22-bandit23: [
    Steps:
        cat /etc/cron.d/cronjob_bandit23
        cat /usr/bin/cronjob_bandit23.sh
        cat /tmp/$(echo I am user bandit23 | md5sum | cut -d ' ' -f 1)
] => 0Zf11ioIjMVN551jX3CmStKLYqjk54Ga

bandit23-bandit24: [
    Steps:
        cat /etc/cron.d/cronjob_bandit24
        cat /usr/bin/cronjob_bandit24.sh
        touch /tmp/tempfile
        chmod o+w /tmp/tempfile
        echo "cat /etc/bandit_pass/bandit24 > /tmp/tempfile"  > /var/spool/bandit24/foo/script.sh
        chmod o+x /var/spool/bandit24/foo/script.sh
        [Wait 60 seconds or less]
        /tmp/tempfile
] => gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8

bandit24-bandit25: [
    Steps:
        [Copy last level's password]
        mkdir /tmp/tempdir
        cd /tmp/tempdir
        seq -w 0 9999
        vim file
        [Just opened VIM in normal mode. Press: ctrl+v G I]
        [Just opened insert mode. Paste the last level's password and insert a space. Then press ESC. And then exit vim with: :x]
        cat file | nc localhost 30002
] => iCi86ttT4KSNe1armKiwbQNmB3YJP3q4

bandit25-bandit26: [
    Steps:
        [Make your terminal small in the Y axis, then log in with ssh]
        [You should be in the interactive mode of the "more" program, reading the /home/bandit26/text.txt file]
        [Press v to open the vi/vim editor. Press: :set shell=/bin/bash]
        [Press: `:!bash`]
        [Then to find the password of the current level (bandit26) you can execute `cat /etc/bandit_pass/bandit26` or directly press `:!cat /etc/bandit_pass/bandit26`]
        [The step above isn't necesary since you'll face the same problem when logging with the password. You need to find the password of the next level in this bash you got.]
] => s0773xxkk0MXfdqOfPRVr9L3jJBUOgCZ

bandit26-bandit27: [
    Steps:
        ./bandit27-do cat /etc/bandit_pass/bandit27
] => upsNCc7vzaRDx6oZC6GiR6ERwe1MowGB

bandit27-bandit28: [
    Steps:
        mkdir /tmp/tempdir
        cd /tmp/tempdir
        git clone ssh://bandit27-git@localhost:2220/home/bandit27-git/repo
        cd repo
        cat README
] => Yz9IpL0sBcCeuG7m9uQFt8ZNpS4HZRcN

bandit28-bandit29: [
    Steps:
        mkdir /tmp/tempdir
        cd /tmp/tempdir
        git clone ssh://bandit28-git@localhost:2220/home/bandit28-git/repo
        cd repo
        git log --oneline
        git show 68314e0
] => 4pT1t5DENaYuqnqvadYs1oE4QLCdjmJ7

bandit29-bandit30: [
    Steps:
        mkdir /tmp/tempdir
        cd /tmp/tempdir
        git clone ssh://bandit29-git@localhost:2220/home/bandit29-git/repo
        cd repo
        git checkout dev
        cat README.md
] => qp30ex3VLz5MDG1n91YowTv4Q8l7CDZL

bandit30-bandit31: [
    Steps:
        mkdir /tmp/tempdir
        cd /tmp/tempdir
        git clone ssh://bandit30-git@localhost:2220/home/bandit30-git/repo
        cd repo
        git show secret
] => fb5S2xb7bRyFmAvQYQGEqsbhVyJqhnDy

bandit31-bandit32: [
    Steps:
        mkdir /tmp/tempdir
        cd /tmp/tempdir
        git clone ssh://bandit31-git@localhost:2220/home/bandit31-git/repo
        cd repo
        cat README.md
        echo May I come in? > key.txt
        git add key.txt
        git commit -m "the asked file"
        git push origin master
] => 3O9RfhqyAlVBEZpVb6LYStshZoqoSx5K
