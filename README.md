# Git-Branch
GitHub. Homework #2 

1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bug_Reports
- SQL
- Charles
- Mobile_testing


Создаем внешний репозиторий c названием Git-Branch.
Клонируем репозиторий Git-Branch на локальный компьютер (папка QA_group_30):

git clone https://github.com/spaceowlsoul/Git-Branch

Переходим в склонированный репозиторий:
cd Git-Branch

Создаем ветки:

git branch Postman
git branch Jmeter
git branch CheckLists
git branch Bug_Reports
git branch SQL
git branch Charles
git branch Mobile_Testing


2. Запушить все ветки на внешний репозиторий:

git push -u origin Postman
git push -u origin Jmeter
git push -u origin CheckLists
git push -u origin Bug_Reports
git push -u origin SQL
git push -u origin Charles
git push -u origin Mobile_Testing


3. В ветке Bug_Reports сделать текстовый документ со структурой баг репорта.

Переходим на ветку Bug_Reports:

git checkout Bug_Reports

Создаем файл bug_report.txt:

cat > bug_report.txt
ID
Summary
Steps to reproduce
Expected Result
Actual Result
Reproducibility
Environment
Severity
Priority
Workaround
Attachments
Comments


4. Запушить структуру багрепорта на внешний репозиторий:

git add bug_report.txt
git commit -m 'add bug_report'
git push

5. Вмержить ветку Bag Reports в Main.

Переходим на ветку main:

git checkout main

Осуществляем слияние:

git merge Bug_Reports


6. Запушить main на внешний репозиторий:

git push


7. В ветке CheckLists набросать структуру чек листа.

Переходим на ветку CheckLists:

git checkout CheckLists

Создаем файл checklist.txt:

cat > checklist.txt
ID
Purpose
Result
Comments


8. Запушить структуру на внешний репозиторий:

git add bug_report.txt
git commit -m 'add checklist'
git push

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main.

Переходим на внешний репозиторий в ветку main. 
Выбираем Compare & Pull Request.
Создаем Pull Request.
Т.к. конфликтов нет, осуществляем Merge.

10. Синхронизировать внешнюю и локальную ветки main.

Переходим на ветку main:

git checkout main

Подтягиваем изменения с внешнего репозитория:

git pull
