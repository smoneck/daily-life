# daily-life
Handy scripts in/from daily life

## arXiv
Fetch latest papers from arxiv.org

## genpw
Generate passwords and usernames from /dev/urandom using 'a-zA-Z0-9-!@#$%^&*()_+~'

```bash
$ genpw 40
L&bGI~96*dx%YbloSWu6%&iLc!r3VHCcyF!%3N4u

$ genpw 10 username
Iougleicke
```

## lnmv
Moves a file but creates a symlink in place. Helps to prevent redundant copies.

```bash
$ ll
drwx------ 2 stephan users 40 Apr  7 20:56 7SKKnN
-rw------- 1 stephan users  6 Apr  7 20:57 test

$ lnmv test 7SKKnN
$ ll
drwx------ 2 stephan users 60 Apr  7 20:58 7SKKnN
lrwxrwxrwx 1 stephan users 23 Apr  7 20:58 test -> /tmp/zRzOjz/7SKKnN/test
```

## strconv
strconv converts a string with spaces and non-ascii into spaceless-ascii.

```bash
$ strconv Die Lösung des Problöms ißt Gemüse
Die_Loesung_des_Probloems_isst_Gemuese
```

