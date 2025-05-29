echo "Репозиторий с откатами изменений" > README.md
git add README.md
git commit -m "Добавил README.md"
git push -u origin main

git checkout -b one
touch 1.txt
git add 1.txt
git commit -m "Добавил 1.txt"

touch 2.txt
git add 2.txt
git commit -m "Добавил 2.txt"

touch 3.txt
git add 3.txt
git commit -m "Добавил 3.txt"

git push --set-upstream
origin one

git log
git checkout main
git checkout -b two

git cherry-pick git200
git cherry-pick volt200
git cherry-pick abic200

git push --set-upstream
origin two

git log
git checkout main
git checkout -b three

git cherry-pick git200
git cherry-pick volt200
git cherry-pick abic200

git push --set-upstream
origin three
