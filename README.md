Windows PowerShell

Copyright (C) Microsoft Corporation. All rights reserved.



PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> git init

Initialized empty Git repository in D:/RIKKEI/DevOpsFundalmental/Session05/bai1/.git/

PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> git status

On branch master



No commits yet



nothing to commit (create/copy files and use "git add" to track)

PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> Set-Content feature.txt "Day la tinh nang quan trong"

PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> Get-Content feature.txt

Day la tinh nang quan trong

PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> git add .

PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> git commit -m "Them tinh nang quan trong"

\[master (root-commit) 25aa1cf] Them tinh nang quan trong

&#x20;1 file changed, 1 insertion(+)

&#x20;create mode 100644 feature.txt

PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> git log --oneline

25aa1cf (HEAD -> master) Them tinh nang quan trong

PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> git reset --hard HEAD\~1

fatal: ambiguous argument 'HEAD\~1': unknown revision or path not in the working tree.

Use '--' to separate paths from revisions, like this:

'git <command> \[<revision>...] -- \[<file>...]'

PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> git log --oneline

25aa1cf (HEAD -> master) Them tinh nang quan trong

PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> Get-ChildItem





&#x20;   Directory: D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1





Mode                 LastWriteTime         Length Name

\----                 -------------         ------ ----

\-a----         10/6/2026  12:14 AM             29 feature.txt





PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> git reflog

25aa1cf (HEAD -> master) HEAD@{0}: commit (initial): Them tinh nang quan trong

PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> git reset --hard e3a5b2c

fatal: ambiguous argument 'e3a5b2c': unknown revision or path not in the working tree.

Use '--' to separate paths from revisions, like this:

'git <command> \[<revision>...] -- \[<file>...]'

PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> git reset --hard 25aa1cf

HEAD is now at 25aa1cf Them tinh nang quan trong

PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> git log --oneline

25aa1cf (HEAD -> master) Them tinh nang quan trong

PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> Get-Content feature.txt

Day la tinh nang quan trong

PS D:\\RIKKEI\\DevOpsFundalmental\\Session05\\bai1> git status

On branch master

nothing to commit, working tree clean

