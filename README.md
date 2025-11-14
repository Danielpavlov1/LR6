# LR6
Лабораторная работа №6
Отчёт по Лабораторной работе №6

Тема: Система контроля версий

Цель: Изучение базовых возможностей системы управления версиями, работа с Git API, локальным и удалённым репозиторием.

1. Создан аккаунт на GitHub.
2. Сделана копия (Fork) репозитория с исходного репозитория по адресу: (https://github.com/Kurtyanik/LR6).

3. Установлен Git с официального сайта: (https://git-scm.com/).

4. Настроен Git, добавлено имя пользователя и email:

```bash
git config --global user.name "4441 Pavlov DS"
git config --global user.email "danya.pavlov.03@mail.ru"
```
<img width="441" height="119" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/1.jpg" />


5. Личный удалённый репозиторий был клонирован на компьютер:
```
git clone https://github.com/Danielpavlov1/LR6
```
<img width="441" height="119" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/2.jpg" />


6. Новый файл был добавлен через интерфейс GitHub, изменения подтянуты в локальный репозиторий:
```
git pull
```
<img width="441" height="119" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/3.jpg" />

7. Получена история операций для каждой из веток:
```
git log --oneline
```
<img width="441" height="209" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/4.jpg" />


8. Последние изменения просмотрены с помощью команды:
```
git log -p -1
```
<img width="641" height="609" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/5.jpg" />


9. Ветка с изменениями была слита в ветку master:
```
git checkout -b new_branch
git add .
git commit -m "Add 1 change"
git checkout master
git merge new_branch
```
<img width="441" height="119" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/6.jpg" />
<img width="441" height="119" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/7.jpg" />
<img width="441" height="119" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/8.jpg" />
<img width="441" height="119" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/9.jpg" />
<img width="441" height="119" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/10.jpg" />



9. Побочная ветка удалена после успешного слияния:
```
git branch -d new_branch
```
<img width="441" height="119" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/11.jpg" />


10. Сделаны несколько изменений и зафиксированы с комментариями:
```
git add .
git commit -m "Add 2 change"
```
<img width="441" height="119" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/12.jpg" />




12. Выбран нужный коммит, выполнен откат:
```
git log --oneline
git revert 7bf633e
```
<img width="441" height="119" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/13.jpg" />
<img width="641" height="619" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/14.jpg" />



13. Создана отдельная ветка для оформления отчёта:
```
git checkout -b rep
```
<img width="641" height="619" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/15.jpg" />


14. Отчёт оформлен в файле README.md с использованием markdown синтаксиса, cкриншоты консоли и сторонних программ добавлены в отдельную папку screen.
15. Получена история операций с сокращённым хэшем, датой, именем автора и комментарием:
```
git log --pretty=format:"%h - %ad - %an - %s" --date=short
```
<img width="641" height="619" alt="image" src="https://github.com/Danielpavlov1/LR6/blob/rep/screens/16.jpg" />


16. Локальные изменения отправлены в удалённый репозиторий на GitHub:
```
git push origin rep
```
Вывод:
В процессе работы я освоила базовые команды и операции в Git, включая commit, merge, checkout, pull, push, а также управление ветками и разрешение конфликтов. Получила опыт синхронизации локального и удаленного репозиториев на GitHub и создания отчетов в Markdown.

