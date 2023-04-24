# JSON
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
|В редакторе vim описать структуру баг-репорта|`-ID: 123,- Title: Что? Где? Когда?,- Version: 1.2.19,- Severity: Trivial,- Priority: Low,- Precondition: Steps,- Environment: Devices, Browser,- STR: Steps to reproduce,- ER: Expected result,- AR: Actual Result,- Attachments: links` (выйти из vim `esq :wq enter`)|
|4. Запушить структуру баг-репорта на внешний репозиторий|`git add.` `git commit -m "bug_report"` `git push`|
|5. Вмержить ветку Bag Reports в Main|`git checkout main` `git merge Bug Reports`|
|6. Запушить main на внешний репозиторий|`git add.` `git commit -m "merge Bug Reports in main"` `git push`|
|7. В ветке CheckLists набросать структуру чек листа|`git checkout CheckLists` `vim structure_check_list.json`|
|В редакторе vim описать структуру чек-листа|`-ID: 123,- Title: Что проверяем?, - Result: pass/failed` (выйти из vim `esq :wq enter`)|
|8. Запушить структуру на внешний репозиторий|`git add.` `git commit -m "check_list"` `git push`|
|9. На внешнем репозитории сделать Pull Request ветки CheckLists в main| Нажать на внешнем репозитории зеленую кнопку `Compare&pull requset`|
|10. Синхронизировать Внешнюю и Локальную ветки Main|`git checkout main` `git fetch` (убедились, что есть изменения) `git pull` (слили изменения)|
