# Делаю тутор на гит 

## первые команды гита 

чтобы закрепить Гит на файл

```
git init
```
получить информацию от гита о его текущем состаянии

```
git status
```
## Добавление коммита 

Добавить файл к следущему коммиту 

```
git add <Название файла.расширение>
```
после можно коментировать

```
git commit -m "коментарий"
```
## просмотр историй коммитов 

вывод на экран всех истории коммитов с их хеш-кодами

```
git log
```

Еше один код который можно посматреть историю но крадко и ясно 

```
git reflog
```

## Переходы между коммитами

переход од одного каммита к другому 

```
git checkout
```

если хотим вернуться к актуальному 

```
git checkout master
```

посматреть разницу что поменял текущим файлом

```
git diff
```
удалить новые несохроненные изменение 

```
git stash
```


# Краткая инструкция по MarcDown

## Краткое руководство
Абзацы создаются при помощи пустой строки. Если вокруг
текста сверху и снизу есть пустые строки, то текст
превращается в абзац.
Чтобы сделать перенос строки вместо абзаца,
нужно поставить два пробела в конце предыдущей строки.
Заголовки отмечаются диезом `#` в начале строки, от
одного до шести. Например:
# Заголовок первого уровня #
## Заголовок h2
### Заголовок h3
#### Заголовок h4
##### Заголовок h5
###### Заголовок h6
В декоративных целях заголовки можно «закрывать» с
обратной стороны.

### Списки
Для разметки неупорядоченных списков можно использовать
или `*`, или `-`, или `+`:
- элемент 1
- элемент 2
- элемент ...
Вложенные пункты создаются четырьмя пробелами перед
маркером пункта:
* элемент 1
* элемент 2
 * вложенный элемент 2.1
 * вложенный элемент 2.2
* элемент ...
Упорядоченный список:
1. элемент 1
2. элемент 2
 1. вложенный
 2. вложенный
3. элемент 3
4. Donec sit amet nisl. Aliquam semper ipsum sit amet
velit. Suspendisse id sem consectetuer libero luctus
adipiscing.
На самом деле не важно как в коде пронумерованы пункты,
главное, чтобы перед элементом списка стояла цифра
(любая) с точкой. Можно сделать и так:
0. элемент 1
0. элемент 2
0. элемент 3
0. элемент 4
Список с абзацами:
* Раз абзац. Lorem ipsum dolor sit amet, consectetur
adipisicing elit.
* Два абзац. Donec sit amet nisl. Aliquam semper ipsum
sit amet velit. Suspendisse id sem consectetuer libero
luctus adipiscing.
* Три абзац. Ea, quis, alias nobis porro quos laborum
minus sed fuga odio dolore natus quas cum enim
necessitatibus magni provident non saepe sequi?
 Четыре абзац (Четыре пробела в начале или один tab).

### Цитаты
Цитаты оформляются как в емейлах, с помощью символа `>`.
> This is a blockquote with two paragraphs. Lorem ipsum
dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi
posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in,
laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet
velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.
Или более ленивым способом, когда знак `>` ставится
перед каждым элементом цитаты, будь то абзац, заголовок
или пустая строка:
> This is a blockquote with two paragraphs. Lorem ipsum
dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi
posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet
vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet
velit. Suspendisse
id sem consectetuer libero luctus adipiscing.
В цитаты можно помещать всё что угодно, в том числе
вложенные цитаты:
> ## This is a header.
>
> 1. This is the first list item.
> 2. This is the second list item.
>
> > Вложенная цитата.
>
> Here's some example code:
>
> return shell_exec("echo $input |
$markdown_script"); 
### Исходный код
В чистом Маркдауне блоки кода отбиваются 4 пробелами в
начале каждой строки.
Но в GitHub-Flavored Markdown (сокращенно GFM) есть
более удобный способ: ставим по три апострофа (на букве
Ё) до и после кода. Также можно указать язык исходного
кода.
```html
<nav class="nav nav-primary">
 <ul>
 <li class="tab-conversation active">
 <a href="#" data-role="post-count"
class="publisher-nav-color" data-nav="conversation">
 <span class="comment-count">0
комментариев</span>
 <span class="comment-countplaceholder">Комментарии</span>
 </a>
 </li>
 <li class="dropdown user-menu" data-role="logout">
 <a href="#" class="dropdown-toggle" datatoggle="dropdown">
 <span class="dropdown-toggle-wrapper">
 <span>
 Войти
 </span>
 </span>
 <span class="caret"></span>
 </a>
 </li>
 </ul>
</nav>
```
Самое приятное, что в коде не нужно заменять угловые
скобки `< >` и амперсанд `&` на их html-сущности. 

### Ссылки
Это встроенная [ссылка с title элементом]
(http://example.com/link "Я ссылка"). Это — [без title]
(http://example.com/link).
А вот [пример][1] [нескольких][2] [ссылок][id] с
разметкой как у сносок. Прокатит и [короткая запись][]
без указания id.
[1]: http://example.com/ "Optional Title Here"
[2]: http://example.com/some
[id]: http://example.com/links (Optional Title Here)
[короткая запись]: http://example.com/short
Вынос длинных урлов из предложения способствует
сохранению читабельности исходника. Сноски можно
располагать в любом месте документа.

## Картинки
Картинка без `alt` текста
![](//placehold.it/150x100)
Картинка с альтом и тайтлом:
![Alt text](//placehold.it/150x100 "Можно задать title")
Запомнить просто: синтаксис как у ссылок, только перед
открывающей квадратной скобкой ставится восклицательный
знак.
Картинки «сноски»:
![Картинка][image1]
![Картинка][image2]
![Картинка][image3]
[image1]: //placehold.it/250x100
[image2]: //placehold.it/200x100
[image3]: //placehold.it/150x100
Картинки-ссылки:
[![Alt text](//placehold.it/150x100)]
(http://example.com/)
 

 создаем еше раз конфликт 
 

### Таблицы
В чистом Маркдауне нет синтаксиса для таблиц, а в GFM
есть.
First Header | Second Header
------------- | -------------
Content Cell | Content Cell
Content Cell | Content Cell
Для красоты можно и по бокам линии нарисовать:
| First Header | Second Header |
| ------------- | ------------- |
| Content Cell | Content Cell |
| Content Cell | Content Cell |
Можно управлять выравниванием столбцов при помощи
двоеточия.
| Left-Aligned | Center Aligned | Right Aligned |
|:------------- |:---------------:| -------------:|
| col 3 is | some wordy text | **$1600** |
| col 2 is | centered | $12 |
| zebra stripes | are neat | ~~$1~~ |
Внутри таблиц можно использовать ссылки, наклонный,
жирный или зачеркнутый текст.
Для всего остального есть обычный HTML.

## информация для теста
