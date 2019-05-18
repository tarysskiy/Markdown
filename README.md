Шпаргалка по Markdown
---------------------

(перевод, [оригинал](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet))

Поиграть с разметкой Markdown можно на [демо-странице](http://www.markdown-here.com/livedemo.html).

##### Содержание  
[Заголовки](#headers)  
[Выделение](#emphasis)  
[Списки](#lists)
[Спискок задач](#tasklist)  
[Ссылки](#links)  
[Изображения](#images)  
[Подсветка кода и синтаксиса](#code)  
[Таблицы](#tables)  
[Цитаты](#blockquotes)  
[Встроенный HTML](#html)  
[Горизонтальная линия](#hr)  
[Новая строка](#lines)  
[Видео Youtube](#videos)
[Эмодзи](#emoji)  

<a name="headers"><h2>Заголовки</h2></a>

```no-highlight
# H1
## H2
### H3
#### H4
##### H5
###### H6

Кроме того, H1 и H2 можно обозначить подчеркиванием:

Alt-H1
======

Alt-H2
------
```

# H1
## H2
### H3
#### H4
##### H5
###### H6

Кроме того, заголовки H1 и H2 можно обозначить подчеркиванием:

Alt-H1
======

Alt-H2
------

<a name="emphasis"><h2>Выделение</h2></a>

```no-highlight
Курсив обозначается *звездочками* или _подчеркиванием_.

Полужирный шрифт - двойными **звездочками** или __подчеркиванием__.

Комбинированное выделение **звездочками и _подчеркиванием_**.

Для зачеркнутого текста используются две тильды . ~~Уберите это.~~
```

Курсив обозначается *звездочками* или _подчеркиванием_.

Полужирный шрифт - двойными **звездочками** или __подчеркиванием__.

Комбинированное выделение **звездочками и _подчеркиванием_**.

Для зачеркнутого текста используются две тильды . ~~Уберите это.~~


<a name="lists"><h2>Списки</h2></a>

(В данном примере предшествующие и завершающие пробелы обозначены точками: ⋅)

```no-highlight
1. Первый пункт нумерованного списка
2. Второй пункт
⋅⋅*Ненумерованный вложенный список.
1. Сами числа не имеют значения, лишь бы это были цифры
⋅⋅1. Нумерованный вложенный список
4. И еще один пункт.

⋅⋅⋅Внутри пунктов списка можно вставить абзацы с таким же отступом. Обратите внимание на пустую строку выше и на пробелы в начале (нужен по меньшей мере один, но здесь мы добавили три, чтобы также выровнять необработанный Markdown).

⋅⋅⋅Чтобы вставить разрыв строки, но не начинать новый параграф, нужно добавить два пробела перед новой строкой.⋅⋅
⋅⋅⋅Этот текст начинается с новой строки, но находится в том же абзаце.⋅⋅
⋅⋅⋅(В некоторых обработчиках, например на Github, пробелы в начале новой строки не нужны.)

* Ненумерованный список можно размечать звездочками
- Или минусами
+ Или плюсами
```

1. Первый пункт нумерованного списка
2. Второй пункт
  * Ненумерованный вложенный список.
1. Сами числа не имеют значения, лишь бы это были цифры
  1. Нумерованный вложенный список
4. И еще один пункт.

   Внутри пунктов списка можно вставить абзацы с таким же отступом. Обратите внимание на пустую строку выше и на пробелы в начале (нужен по меньшей мере один, но здесь мы добавили три, чтобы также выровнять необработанный Markdown).

   Чтобы вставить разрыв строки, но не начинать новый параграф, нужно добавить два пробела перед новой строкой.
   Эта текст начинается с новой строки, но находится в том же абзаце.
   (В некоторых обработчиках, например на Github, пробелы в начале новой строки не нужны.)

* Ненумерованный список можно размечать звездочками
- Или минусами
+ Или плюсами

<a name="tasklist"><h2>Список задач</h2></a>

В Markdown есть даже своеобразные списки задач — аналог чекбоксов в OneNote или Evernote. Вот как они выглядят:

```no-highlight

- [ ] Невыполненная задача
- [ ] Невыполненная задача
- [X] Выполненная задача

```
- [ ] Невыполненная задача
- [ ] Невыполненная задача
- [X] Выполненная задача

<a name="links"><h2>Ссылки</h2></a>

Ссылки можно оформить разными способами.

```no-highlight
[Обычная ссылка в строке](https://www.google.com)

[Обычная ссылка с title](https://www.google.com "Сайт Google")

[Ссылка со сноской][Произвольный регистронезависимый текст]

[Относительная ссылка на документ](../blob/master/LICENSE)

[Для ссылок со сноской можно использовать цифры][1]

Или можно просто вставить ссылку в квадратные скобки [текст ссылки]

Произвольный текст, после которого можно привести ссылки.

[произвольный регистронезависимый текст]: https://www.mozilla.org
[1]: http://slashdot.org
[текст ссылки]: http://www.reddit.com
```

[Обычная ссылка в строке](https://www.google.com)

[Обычная ссылка с title](https://www.google.com "Сайт Google")

[Ссылка со сноской][Произвольный регистронезависимый текст] *

[Относительная ссылка на документ](../blob/master/LICENSE)

[Для ссылок со сноской можно использовать цифры][1]

Или можно просто вставить ссылку в квадратные скобки [текст ссылки]

Произвольный текст, после которого можно привести ссылки.

[Произвольный регистронезависимый текст]: https://www.mozilla.org
[1]: http://slashdot.org
[текст ссылки]: http://www.reddit.com

(*) Для символов не входящих в ASCII, например кириллицы, текст сноски все-таки регистрозависим (прим. перев.)

<a name="images"><h2>Изображения</h2></a>

```no-highlight
Вот наш логотип (наведите указатель, чтобы увидеть текст заголовка):

Внутри строки:  
![alt-текст](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Текст заголовка логотипа 1")

В сноске:  
![alt-текст][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Текст заголовка логотипа 2"
```

Вот наш логотип (наведите указатель, чтобы увидеть текст заголовка):

Внутри строки:  
![alt-текст](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Текст заголовка логотипа 1")

В сноске:  
![alt-текст][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Текст заголовка логотипа 2"

<a name="code"><h2>Код и подсветка синтаксиса</h2></a>

Блоки кода являются частью функций Markdown, но не подсветка синтаксиса. Однако многие обработчики, например Github или *Markdown Here*, поддерживают подсветку синтаксиса. Список поддерживаемых языков и способ их указания может различаться. *Markdown Here* поддерживает десятки языков (и не-языков, например синтаксис diff и заголовки HTTP); полный список и способ указания языков см. на странице [highlight.js demo-странице](http://softwaremaniacs.org/media/soft/highlight/test.html).

```no-highlight
`Код` в строке обрамляется `обратными апострофами`.
```

`Код` в строке обрамляется `обратными апострофами`.

Блоки кода выделяются либо тремя обратными апострофами <code>```</code> либо четырьмя пробелами в каждой строке. Рекомендуется использовать три апострофа -- они проще и только они поддерживают подсветку синтаксиса.

<pre lang="no-highlight"><code>```javascript
var s = "Подсветка JavaScript";
alert(s);
```
 
```python
s = "Подсветка Python"
print s
```
 
```
Язык не указан, синтаксис не подсвечен.
Но мы вставим в него &lt;b&gt;тег&lt;/b&gt;.
```
</code></pre>



```javascript
var s = "Подсветка JavaScript";
alert(s);
```
 
```python
s = "Подсветка Python"
print s
```

```
Язык не указан, синтаксис не подсвечен (некоторые обработчики все же подсвечивают).
Но мы вставим в него <b>тег</b>.
```


<a name="tables"><h2>Таблицы</h2></a>

Таблицы не являются частью Markdown, но многие обработчики, например *Markdown Here* и Github, поддерживают их. Они позволяют легко добавить таблицы в электронное письмо -- в других случаях для этого нужно копировать их из другого приложения.

```no-highlight
Вертикальные линии обозначают столбцы.

| Таблицы       | Это                | Круто |
| ------------- |:------------------:| -----:|
| столбец 3     | выровнен вправо    | $1600 |
| столбец 2     | выровнен по центру |   $12 |
| зебра-строки  | прикольные         |    $1 |

Внешние вертикальные линии (|) не обязательны и нужны только, чтобы сам код Markdown выглядел красиво. Тот же код можно записать так:

Markdown | не такой | красивый
--- | --- | ---
*Но выводится* | `так же` | **клево**
1 | 2 | 3
```

Вертикальные линии обозначают столбцы.

| Таблицы       | Это                | Круто |
| ------------- |:------------------:| -----:|
| столбец 3     | выровнен вправо    | $1600 |
| столбец 2     | выровнен по центру |   $12 |
| зебра-строки  | прикольные         |    $1 |

Внешние вертикальные линии (|) не обязательны и нужны только, чтобы сам код Markdown выглядел красиво. Тот же код можно записать так:

Markdown | не такой | красивый
--- | --- | ---
*Но выводится* | `так же` | **клево**
1 | 2 | 3

<a name="blockquotes"><h2>Цитаты</h2></a>

```no-highlight
> С помощью цитат очень удобно в письме обозначать исходный текст.
> Эта строка - часть той же цитаты.

Разрыв цитаты.

> Это очень длинная строка, но она будет правильно процитирована даже при размещении на нескольких строках. Продолжаем писать, чтобы эта строка не вмещалась на одной строке в любом окне. Кстати, в цитаты можно *вставлять* даже **Markdown**.
```

> С помощью цитат очень удобно в письме обозначать исходный текст.
> Эта строка - часть той же цитаты.

Разрыв цитаты.

> Это очень длинная строка, но она будет правильно процитирована даже при размещении на нескольких строках. Продолжаем писать, чтобы эта строка не вмещалась на одной строке в любом окне. Кстати, в цитаты можно также *размечать* с помощью **Markdown**.

<a name="html"><h2>Встроенный HTML</h2></a>

Часто Markdown понимает чистый HTML.

```no-highlight
<dl>
  <dt>Список определений</dt>
  <dd>Это то, что люди иногда используют.</dd>

  <dt>Markdown внутри HTML</dt>
  <dd>Работает *не очень** хорошо. Используйте HTML-<em>теги</em>.</dd>
</dl>
```

<dl>
  <dt>Список определений</dt>
  <dd>Это то, что люди иногда используют.</dd>

  <dt>Markdown внутри HTML</dt>
  <dd>Работает *не очень** хорошо. Используйте HTML-<em>теги</em>.</dd>
</dl>

<a name="hr"><h2>Горизонтальные линии</h2></a>

```
Три и более...

---

Дефисы

***

Звездочки

___

Подчеркивания
```

Три и более...

---

Дефисы

***

Звездочки

___

Подчеркивания

<a name="lines"><h2>Новая строка</h2></a>

Для понимания работы разрыва строка автор главным образом рекомендует экспериментировать и пробовать -- нажмите &lt;Enter&gt; один раз (т.е. перейдите на новую строку), потом нажмите дважды (т.е. вставьте две новые строки) и посмотрите что приозошло. Вы сразу поймете что вам нужно. В расширении [Markdown Here](https://github.com/adam-p/markdown-here) для браузеров есть удобная функция "Markdown Toggle", которая поможет в этом.

*Примечание переводчика:*  
*Для переноса на новую строку в конце предыдущей строки необходимо добавить* **два пробела**. *Без этого большинство парсеров Markdown не выполняют переход на новую строку.*

Попробуйте ввести следующее:

```
Это начальная строка

Эта строка отделена от предыдущей двумя новыми строками и станет *отдельным абзацем*.

Это тоже отдельный абзац, но...⋅⋅
Эта строка отделена одной новой строкой, поэтому она находится в *том же абзаце*.
```

Это начальная строка

Эта строка отделена от предыдущей двумя новыми строками и станет *отдельным абзацем*.

Это тоже отдельный абзац, но...`[здесь два пробела]`  
Эта строка отделена одной новой строкой, поэтому она находится в *том же абзаце*.  

(Примечание: В [Markdown Here](https://github.com/adam-p/markdown-here) разрывы строк ведут себя так же, как в [GFM](https://help.github.com/articles/github-flavored-markdown), поэтому не нужно вставлять по две новые строки.)

<a name="videos"><h2>Видео Youtube</h2></a>

Ролики нельзя вставить напрямую, но можно вставить изображение со ссылкой на видео, например:

```no-highlight
<a href="http://www.youtube.com/watch?feature=player_embedded&v=ID_ВИДЕОРОЛИКА_НА_YOUTUBE" target="_blank"><img src="http://img.youtube.com/vi/ID_ВИДЕОРОЛИКА_НА_YOUTUBE/0.jpg" 
alt="ALT-ТЕКСТ ИЗОБРАЖЕНИЯ" width="240" height="180" border="10" /></a>
```

На чистом Markdown, но без размеров изображения и рамки:

```no-highlight
[![ALT-ТЕКСТ ИЗОБРАЖЕНИЯ](http://img.youtube.com/vi/ID_ВИДЕОРОЛИКА_НА_YOUTUBE/0.jpg)](http://www.youtube.com/watch?v=ID_ВИДЕОРОЛИКА_НА_YOUTUBE)
```
<a name="emoji"><h2>Эмодзи</h2></a>

Чтобы добавить смайл, нужно напечатать соответствующий код и заключить его в двоеточия:

```no-highlight

:sunglasses:

```
:sunglasses:

Посмотреть коды эмодзи можно [здесь](https://www.webfx.com/tools/emoji-cheat-sheet/).
