# Отчет по лабораторной работе №2

## Цель работы
Изучить идеологию и применение средств контроля версий.

## Ход работы
1. Создали учетную запись на github.com, настроили git и создали структуру каталога ![](https://github.com/dsshestakov/Lab_02/blob/master/report/img/Снимок%20экрана%20от%202021-04-29%2014-30-59.png)
2. Создали репозиторий на github.com, назвали его Lab_02
3. Перешли в рабочий каталог
4. Инициализировали систему контроля версий ```git init```
5. Создали заготовку файла README.md ```echo "Лабораторная работа №2" >> README.md  git add README.md```
6. Сделали первый коммит и выложили на github 
  ```bash
    git commit -m "first commit"
    git remote add origin git@github.com/dsshestakov/Lab_02
    git push -u origin master
  ```
  ![](https://github.com/dsshestakov/Lab_02/blob/master/report/img/Снимок%20экрана%20от%202021-04-29%2014-35-33.png)
7. Добавили файл лицензии ```wget https://creativecommons.org/licenses/by/4.0/legalcode.txt -O LICENSE ```
8. Скачали шаблон для С ```curl -L -s https://www.gitignore.io/api/c >> .gitignore ```
9. Добавили новые файлы, выполнили коммит, отправили на github
``` bash
    git add .
    git commit -a
    git push
```
![](https://github.com/dsshestakov/Lab_02/blob/master/report/img/Снимок%20экрана%20от%202021-04-29%2014-38-26.png)
10. Инициализировали gitflow ``` git flow init``` ![](https://github.com/dsshestakov/Lab_02/blob/master/report/img/Снимок%20экрана%20от%202021-04-29%2014-39-36.png)
11. Проверили, что мы на ветке develop ``` git branch ``` ![](https://github.com/dsshestakov/Lab_02/blob/master/report/img/Снимок%20экрана%20от%202021-04-29%2014-39-25.png)
12. Создали релиз 1.0.0 ```git flow release start 1.0.0```
13. Добавили индекс
```bash
   git add .
   git commit -am "chore(main): add version"
```
14. Залили релизную ветку в основную ветку ```git flow release finish 1.0.0```
15. Отправили данные на github
```bash
   git push --all
   git push --tags
```
![](https://github.com/dsshestakov/Lab_02/blob/master/report/img/Снимок%20экрана%20от%202021-04-29%2014-41-34.png)


