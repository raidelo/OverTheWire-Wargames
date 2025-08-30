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
