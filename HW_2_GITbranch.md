### 1. На локальном репозитории сделать ветки для:

- Postman  

`git branch Postman`
- Jmeter

 `git branch Jmeter`
- CheckLists 

 `git branch Checklists`
- Bag Reports

`git branch Bag_Reports`
- SQL

 `git branch SQL`
- Charles

`git branch Charles`
- Mobile testing

 `git branch Mobile_Testing`
 
 
### 2. Запушить все ветки на внешний репозиторий

`git push -u origin Postman`

`git push -u origin Jmeter`

`git push -u origin Checklists`

`git push -u origin Bag_Reports`

`git push -u origin SQL`

`git push -u origin Charles`

`git push -u origin Mobile_Testing`

### 3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта

`git checkout Bag_Reports`

`touch BagReports.txt`

`nano BagReports.txt`


    № 	     name    	           description
	1 	ID                   Уникальный идентификационный номер
	2 	Summary/Title 	    Что? Где? При каких обстоятельствах/условиях?
	3 	STR 	            Шаги воспроизведения
	4 	Actual Result 	    Фактический результат
	5 	Expected Result     Ожидаемый результат
	6 	Environment 	    Окружение (н. Dev/Stage/Prod)
	7 	Project 	    Название проекта
	8 	Module 	            Компонент/модуль/юнит, в котором обнаружен дефект
	9 	Build 	            Версия сборки
	10 	Severity            Критичность бага по степени влияния на продукт
	11 	Priority 	    Критичность бага по степени влияния на бизнес
	12 	Status 	            Статус бага в жизненном цикле бага
	13 	Author 	            Тот, кто нашёл баг
	14 	Assigned to 	    Назначение
	15 	Attachments 	    Логи/скриншоты/видео

`ctrl+X, Y + enter`

### 4. Запушить структуру багрепорта на внешний репозиторий

`git add BagReports.txt`

`git commit -m "Add new file BagReports.txt"`

`git push`

### 5. Вмержить ветку Bag Reports в Main

`git checkout main`

`git merge Bag_Reports`

### 6. Запушить main на внешний репозиторий.

 `git push`

### 7. В ветке CheckLists набросать структуру чек листа.

`git checkout Checklists`

`touch checklist.txt`

`nano checklist.txt`

		name 	           description
	Test type 	   Тип/вид/уровень тестирования
	Checking 	   Название проверки
	Result 	           Результат

`ctrl+X, Y + enter`

### 8. Запушить структуру на внешний репозиторий

`git add checklist.txt`

`git commit -m "Add new file checklist.txt"`

`git push`

### 9. На внешнем репозитории сделать Pull Request ветки CheckLists в main

`Зайти на сайт github`

`Выбрать репозиторий Group29`

Нажать на кнопку `Compare & pull request`

Нажать на кнопку `Create pull request`

Нажать на кнопку `Merge pull request`

Нажать на кнопку `Confirm merge'`

После слияния веток должно быть указано `Pull request successfull merged and closed`

### 10. Синхронизировать Внешнюю и Локальную ветки Main

`git checkout main`

`git pull`
