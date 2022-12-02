TXT
 1. Создать внешний репозиторий c названием TXT.
Create repository TXT

 2. Клонировать репозиторий TXT на локальный компьютер.
cd HW_Git
git clone https://github.com/Seredinaleta/TXT

 3. Внутри локального TXT создать файл “new.txt”.
cd TXT
touch new.txt

 4. Добавить файл под гит.
git add .

 5. Закоммитить файл.
git commit -m"Adding new.txt"

 6. Отправить файл на внешний GitHub репозиторий.
git push

 7. Отредактировать содержание файла “new.txt” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате TXT.
vim new.txt
insert
Name - Yuliia Trubina,
Age - 44,
Pets - none,
Salary - 2000.

 8. Отправить изменения на внешний репозиторий.
git add new.txt
git commit -m"Updating new.txt"
git push

 9. Создать файл preferences.txt
touch Preferences.txt
 10. В файл preferences.txt” добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате TXT.
vim Preferences.txt
insert
Favorite film - "Prada",
Favorite serial - "Stargate Atlantis",
Favorite dish - meat,
Favorite season - spring,
Next desired country - Crete.
Esc :wq

 11. Создать файл sklls.txt добавить информацию о скиллах которые будут изучены на курсе в формате TXT
cat>>Skills.txt
Skills:
1.Theory of testing.
2.Basic JavaScript.
3.Client-server architecture.
4.HTTP request methods and responce codes.
5.Structures JSON and XML.
6.DevTools of web browsers.
7.Mobile testing.
8.Command line (Terminal).
9.SQL Basic.
10.Scrum development methodology.
11.API testing via Postman(JS,API autotests.
CTRL Z

 12. Сделать коммит в одну строку.
git add Preferences.txt Skills.txt | git commit -am"Adding Preferences.txt and Skills.txt"

 13. Отправить сразу 2 файла на внешний репозиторий.
git push

 14. На веб интерфейсе создать файл bug_report.txt.
touch bug_report.txt

 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
git add bug_report.txt
git commit _m"Create bug_report.txt"

 16. На веб интерфейсе модифицировать файл bug_report.txt, добавить баг репорт в формате TXT.
Bug_report
 Main part
   ID -number in Youth bug-tracking system,
   Summary (Title) - Short text description jf the bug,
   STR -Steps to reproduce the bug,
   ER - Estimated result of the test,
   AR - Actual result of the test,
   Severity - The degree of influence a defect has on the product's operation blocker/crititical/major/minor/trivial,
   
  Additional part
   Priority - The order in which the defect should be fixed ASAP/high/medium/low,
   Environment - Conditions Device Type/OS/Browser/Software version/Connection Strength/Screen size/Zoom level/Pixel ratio etc,
   Visual Proof -Screenshots, videos, text, logs of Bug,
   
 Reporter name - Your own,
 Status - SDLS status Opened/In Progress/Fixed or Ready for check/Reopened/Closed/Deffered/Rejected

 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
git add bug_report.txt | git commit -m"Modified bug_report.txt"

 18. Синхронизировать внешний и локальный репозиторий TXT.
git fetch
git push
