# git-test
## History

git checkout -b MDL-001_commit_1

vi main.txt

git add .

git commit -m "[MDL-001] commit #1"

git push --set-upstream origin MDL-001_commit_1

> PR process on Gui 

git checkout main

git pull --rebase

git checkout -b MDL-002_commit_2

vi main.txt

git add .

git commit -m "[MDL-002] commit #2"

git checkout main

git checkout -b MDL-003_hotfix

vi main.txt

git add .

git commit -m "[MDL-003] hotfix #1"

git checkout MDL-002_commit_2

git push --set-upstream origin MDL-002_commit_2

> PR process on GUI 

git checkout MDL-003_hotfix

vi main.txt

git add .

git commit -m "[MDL-003] hotfix #2"

git rebase main

> conflict occur >> fix on vim 

git add .

git rebase --continue

git push --set-upstream origin MDL-003_hotfix

> PR process on GUI 

git checkout main

git pull --rebase

git log
