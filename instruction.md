# Инструкция по языку Markdown
## Заголовок 2-го уровня
### Заголовок 3-го уровня
Обычный текст называем как есть. 

Новая строка 
## Выделение текста
*курсив*  
_курсив_

**жирный**  
__жирный__

***жирный курсив***  
___жирный курсив___

~~зачеркнутый~~
## Списки
### Нумерованный список
1. Пункт первый
2. Пункт второй
3. Пункт третий

### Маркированный список
- Пункт первый
- Пункт второй
- Пункт третий
### Вложенные списки
1. Пункт первый
    - Подпункт первый
    - Подпункт второй
2. Пункт второй
## Ссылки
[Текст ссылки](https://www.example.com)
## Изображения 
![Текст описания](https://i.pinimg.com/564x/af/ac/e8/aface8ae6a0c7f3d7c23f81e2ba16059.jpg)
## Блоки кода
### Строка кода
`строка кода`
## Подсветка кода
```python
print("Привет, мир!")
```
### Цитаты
> Первый уровень цитирования
>> Второй уровень цитирования
>>> Третий уровень цитирования
## Горизонтальная линия
---
## Таблицы
| Заголовок 1 | Заголовок 2 |
| ----------- | ----------- |
| Ячейка 1    | Ячейка 2   |
| Ячейка 3    | Ячейка 4   | 
## Оповещения ("Примечание", "Совет", "Важно!", "Внимание!", "Предупреждение")

> **Примечание**
Текст вашей заметки

> **Предупреждение**
Текст вашего предупреждения

# Инструкция по работе с git 
## Работа с локальным репозиторием
### Базовые команды
#### **git init — создание репозитория**
Команда git init создает в директории пустой репозиторий в виде директории .git, где и будет в дальнейшем храниться вся информация об истории коммитов, тегах — о ходе разработки проекта: 
```
mkdir project-dir
cd project-dir
git init
```
#### git add и git rm — индексация изменений
Следующее, что нужно знать — команда git add. Она позволяет внести в индекс — временное хранилище — изменения, которые затем войдут в коммит.

Индексирует измененный файл, либо оповещение о создании нового:
```
git add EDITEDFILE
```
Вносит в индекс все изменения, включая новые файлы:
```
git add 
```
Из индекса и дерева проекта одновременно файл можно удалить командой git rm.

Удаляет из индекса и дерева проекта отдельные файлы:
```
git rm FILE1 FILE2
```
Хороший пример удаления из документации к git, удаляются сразу все файлы txt из папки:
```
git rm Documentation/\*.txt
```
Вносит в индекс все удаленные файлы:
```
git rm -r --cached .
```