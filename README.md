# JSON

## GitHub. HW_1
|ToDo|Commands|
|:---------------|:-----|
|1. Создать внешний репозиторий c названием JSON|Создаем новый репозиторий с названием JSON на внешнем репозитории(New), во вкладке `<> Code` копируем `HTTPS`|
|2. Клонировать репозиторий JSON на локальный компьютер|`git clone` `ctrl + V` (вставили скопированный `HTTPS`)|
|3. Внутри локального JSON создать файл “new.json”||`cd JSON` `touch new.json`|
|4. Добавить файл под гит|`git add .`|
|5. Закоммитить файл|`git commit -m "new"`|
|6. Отправить файл на внешний GitHub репозиторий|`git push`|
|7. Отредактировать содержание файла “new.json”, написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON|`vim new.json`|  
| |Нажать `i`|
| |`{`|
| |`"person_name": "Nastya",`|  
| |`"person_age": 29,`|  
| |`"amount_of_pets":`|  
| |`{"type_of_pet":`| 
| |`"cat",`|
| |`"cat_name":`|  
| |`"Zhorik"},`|  
| |`"desired_salary": 2000`|
| |`}`|  
| |Нажать `Esc :wq Enter`|
|8. Отправить изменения на внешний репозиторий|`git commit -m "new"` `git push`|
|9. Создать файл preferences.json|`touch preferences.json`|
|10. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON||vim preferences.json|
| |Нажать `i`|
| |`{`|
| |`"favorite_film": "Stories_about_Harry_Potter",`|
| |`"favorite_series": "Game_of_Thrones",`|
| |`"favorite_food": "pizza",`|
| |`"favorite_season": "summer",`|
| |`"want_to_travel": "Italy",`|
| |`"favorite_book": "Theodore Dreiser:American tragedy"`|
| |`}`|
| |Нажать `Esc :wq Enter`|
|11. Создать файл skills.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON|`vim skills.json`|
| |Нажать `i`|
| |`{`|
| |`"skills_of_junior_QA": {`|
| |`"1": "SQL",`|
| |`"2": "Postman",`|
| |`"3": "Git",`|
| |`"4": "Client_server_arhitecture",`|
| |`"5": "Theory_of_testing",`|
| |`"6": "Testing_documentation",`|
| |`"7": "Mobile_testing",`|
| |`"8": "Terminal"`|
| |`}`|
| |`}`|
| |Нажать `Esc :wq Enter`|
|12. Отправить сразу 2 файла на внешний репозиторий|`git add .` `git commit -m "preferences and skills"` `git push`|
|13. На веб интерфейсе создать файл bug_report.json|Нажать `Add file` > `Create new file` > имя `bug_report.json`|
|14. Сделать Commit changes (сохранить) изменения на веб интерфейсе|Нажать `Commit new file`|
|15. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON|Нажать `Edit this file`|
| |`{`|
| |`"ID": 123,`|
| |`"Title": "Что? Где? Когда?",`|
| |`Version": 1.2.19,`|
| |`"Severity": "Trivial",`|
| |`"Priority": "Low",`|
| |`"Precondition": "Steps",`|
| |`"Environment": "Devices, Browser",`|
| |`"STR": "Steps to reproduce",`|
| |`"ER": "xpected result",`|
| |`"AR": "Actual Result",`|
| |`"Attachments": "links"`|
| |`}`|
|16. Сделать Commit changes (сохранить) изменения на веб интерфейсе|Нажать `Commit changes`|
|17. Синхронизировать внешний и локальный репозиторий JSON|в git bush ввести команду`git pull`|

## GitHub. HW_2
|ToDo|Commands|
|:---------------|:-----|
|1.1 На локальном репозитории сделать веткy для Postman|`git branch Postman`|
|1.2 На локальном репозитории сделать веткy для Jmeter|`git branch Jmeter`|
|1.3 На локальном репозитории сделать веткy для CheckLists|`git branch CheckLists`|
|1.4 На локальном репозитории сделать веткy для Bag Reports|`git branch Bag Reports`|
|1.5 На локальном репозитории сделать веткy для SQL|`git branch SQL`|
|1.6 На локальном репозитории сделать веткy для Charles|`git branch Charles`|
|1.7 На локальном репозитории сделать веткy для Mobile testing|`git branch Mobile testing`|
|2. Запушить все ветки на внешний репозиторий|`git add.` `git commit -m "new branches"`  `git checkout main`  `git push -u origin Postman SQL Jmeter CheckLists Charles MobileTesting BagReports`|
|3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта|`git checkout BagReports` `vim structure_bug_report.json`|
|В редакторе vim описать структуру баг-репорта|нажать `i`, `-ID: 123,- Title: Что? Где? Когда?,- Version: 1.2.19,- Severity: Trivial,- Priority: Low,- Precondition: Steps,- Environment: Devices, Browser,- STR: Steps to reproduce,- ER: Expected result,- AR: Actual Result,- Attachments: links` (выйти из vim `esq :wq enter`)|
|4. Запушить структуру баг-репорта на внешний репозиторий|`git add.` `git commit -m "bug_report"` `git push`|
|5. Вмержить ветку Bag Reports в Main|`git checkout main` `git merge Bug Reports`|
|6. Запушить main на внешний репозиторий|`git add.` `git commit -m "merge Bug Reports in main"` `git push`|
|7. В ветке CheckLists набросать структуру чек листа|`git checkout CheckLists` `vim structure_check_list.json`|
|В редакторе vim описать структуру чек-листа|нажать `i`, `-ID: 123,- Title: Что проверяем?, - Result: pass/failed` (выйти из vim `esq :wq enter`)|
|8. Запушить структуру на внешний репозиторий|`git add.` `git commit -m "check_list"` `git push`|
|9. На внешнем репозитории сделать Pull Request ветки CheckLists в main| Нажать на внешнем репозитории зеленую кнопку `Compare&pull requset`|
|10. Синхронизировать Внешнюю и Локальную ветки Main|`git checkout main` `git fetch` (убедились, что есть изменения) `git pull` (слили изменения)|
