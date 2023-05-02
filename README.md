GIT Homework 1

1. Создать внешний репозиторий c названием JSON.
  Для этого заходим в аккаунт Guthub, нажимаем на "Repositories" после на "New", называем и создаем.
2.  Клонировать репозиторий JSON на локальный компьютер.
  Для клонирования репозитория нужно создать папку, после с помощью скопированого URL
  
    git clone https://github.com/Kr0k0d/JSON.git
    Вывело:Cloning into 'JSON'...
    remote: Enumerating objects: 3, done
    remote: Counting objects: 100% (3/3), done.
    remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
    Receiving objects: 100% (3/3), done.
    
3. Внутри локального JSON создать файл “new.json”.
  touch new.json
  
4. Добавить файл под гит.
  Подготавливаем файл: git add .
  
  Проверяем состояние изменений: git status
  Вывод: On branch main
         Your branch is up to date with 'origin/main'.
         Changes to be committed:
         (use "git restore --staged <file>..." to unstage)
         new file:   new.json
         
5. Закоммитить файл. 
  Коммит нужен для фиксации изменений: git commit -m "New file"
  
  Вывод: [main a683315] New file
         1 file changed, 0 insertions(+), 0 deletions(-)
         create mode 100644 new.json

  
6. Отправить файл на внешний GitHub репозиторий.
  Отправляем коммит и принимает ответ: git push
  
  вывод: Enumerating objects: 4, done.
         Counting objects: 100% (4/4), done.
         Delta compression using up to 4 threads
         Compressing objects: 100% (2/2), done.
         Writing objects: 100% (3/3), 272 bytes | 272.00 KiB/s, done.
         Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
         To https://github.com/Kr0k0d/JSON.git
         2f2051a..a683315  main -> main


 7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.
  Чтобы отредактировать сожержимое файла json мне понадобилось воспоользоваться notepad++
  {
  "firstName": "Daniil",
  "lastName": "Novikov",
  "age": 19,
  "pets_count": 1,
  "desired_salary": 30000
  }
  
 8. Отправить изменения на внешний репозиторий.
    Для отправки изменений выполняем теже действия, что и в пунктах 4-6
    git add .
    
    git commit -m "Information about me"
    Вывод: [main 44ed8d2] Information about me
           1 file changed, 9 insertions(+)
           
           
    git push
    Вывод:Enumerating objects: 5, done.
          Counting objects: 100% (5/5), done.
          Delta compression using up to 4 threads
          Compressing objects: 100% (3/3), done.
          Writing objects: 100% (3/3), 366 bytes | 183.00 KiB/s, done.
          Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
          To https://github.com/Kr0k0d/JSON.git
          a683315..44ed8d2  main -> main
          
9. Создать файл preferences.json
  touch preferences.json
  
10.В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.
  Я попытался открыть файл через git bash с помощью notepad++, но она не работает, поэтому я решил сделать это через nano.
  
  nano preferences.json
  
  Открывется менюшка где мы вводим данные
  
  {
	"Favorite movie": "1 + 1"
	"Favorite series": "Lucifer"
	"Favorite food": "Beef steak"
	"Favorite season": "Summer"
	"Country would like to vist": "Italy"
   }
   
   Полсе нажимаем Ctrl+0 для того чтобы сохранить, и Ctrl+X для того чтобы закрыть
   
   
11.  Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
  Все тоже самое, что и в пункте 10 
  
  touch sklls.json
  
  nano sklls.json
  
  {
	"skills":[
		"Tesring Basics",
		"Manual testing"
		"Automated testing"
		"Security testing"
		"Basics of programming"
		"Database basics"
		"Modern testing methods"
		"Communication and interpersonal skills"
		"Project manegement"
		"Tools skills(Postman)"
    ]
  }
  
  
12. Отправить сразу 2 файла на внешний репозиторий.
  git add . 
  
  git commit -m "Добавление двух файлов preferences.json и skills.json"
  Вывод: [main 90df81d] Добавление двух файлов preferences.json и skills.json
         2 files changed, 21 insertions(+)
         create mode 100644 preferences.json
         create mode 100644 sklls.json
         
  git push
  Вывод: Enumerating objects: 5, done.
         Counting objects: 100% (5/5), done.
         Delta compression using up to 4 threads
         Compressing objects: 100% (4/4), done.
         Writing objects: 100% (4/4), 689 bytes | 229.00 KiB/s, done.
         Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
         To https://github.com/Kr0k0d/JSON.git
         44ed8d2..90df81d  main -> main



 
 
 
 
 
 
