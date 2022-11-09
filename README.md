# vcs-git-orphaning
Для решения данной проблемы выполним следующую последовательность команд

1) ``git checkout -b dev # создаем ветку dev на последнем коммите``
2) ``git checkout main``
3) ``git reset HEAD~2 # возвращаем main к исходному коммиту``
4) ``git push --force``
5) ``git checkout dev --force``
6) ``git push --set-upstream origin dev``
7) открываем PR