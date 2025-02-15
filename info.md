# **Мануал по работе с Git и Visual Studio Code** 

## ***Установка Git и Visual Studio Code***
---

- Установка Git для Windows, Mac, Linux: (https://git-scm.com/downloads
)
- Установка VSCode для Windows, Mac, Linux: (https://code.visualstudio.com/Download)
---
 При первом использование **Git** необходимо "представиться". 
 
 ![Здравствуйте](https://sun9-77.userapi.com/impf/c638428/v638428428/31fa4/fsJwc3BHoKI.jpg?size=256x256&quality=96&sign=c32b77c1b03364e6253d6eadad596dc1&type=album)
 
 Для этого нужно ввести в терминале 2 команды:
 
 1. git config --global user.name «Ваше имя английскими буквами»  
 2. git config --global user.email «Ваша почта английскими буквами»
---
## ***Основные команды git*** 
---
**git init** - инициализация локального репозитория 

**git status** - получить информация от git о его текущем состоянии

**git add** - добавить файлы к следующему коммиту 

**git commit -m “message”** - создание коммита

**git log** – вывод на экран истории всех коммитов с их хеш-кодами

**git checkout** – переход от одного коммита к другому

**git checkout master** – вернуться к актуальному состоянию и продолжить работу

**git diff** – увидеть разницу между текущим файлом и закоммиченным файлом

**git add ./*** - добавить все файлы и вложенные папки, в которых было изменение добавляет в область видимости репозитория 

**git commit -am “”** – совмещает в себе команду git add и git commit -m, в случае, если хотя бы один раз было сохранение с git add и git commit

---
## ***Синтаксис языка Markdown***
---

Справочник по Markdown от Microsoft:
(https://docs.microsoft.com/ru-ru/contribute/markdown-reference)

"#" Заголовок – выделение заголовков. Количество символов “#” задаёт уровень заголовка  (поддерживается 6 уровней):

---
# Заголовок 1 уровня
## Заголовок 2 уровня
---
###### Заголовок 6 уровня
---
"=" или "-" – подчёркиванием этими символами (не менее 3 подряд) выделяют заголовки  первого (“=”) и второго (“-”) уровней

"**" или "_" - по бокам от слова предложения - полужирное начертание -
**слово**

"*" - по бокам от слова или предложения - курсивное начертание - *слово*

"***" - по бокам от слова или предложения - полужирное курсивное начертание - 
***слово***

"~~" - по бокам от слова или предложение - зачерктуный текст - 
~~Слово~~

"1, 2, 3 …" – нумерованные списки

<<*>> символ в начале строки – ненумерованные списки
***
> Важно не количество знаний, а качество их. Можно знать очень многое, не зная самого нужного - программирования.  © Толстой Лев Николаевич
***
## ***Списки***
***
Выше мы уже разбирали некоторые особенности синтексиса Markdown, сейчас мы будет говорить об его отедльных возможностях подробнее. Начнем со **списков**.

Markdown поддерживает упорядоченные (нумерованные) и неупорядоченные (ненумерованные) списки. Для формирования неупорядоченный списков используются такие маркеры, как звездочки, плюсы и дефисы. 

Все перечисленные маркеры могут использоваться взаимозаменяемо. Для формирования упорядоченных списков в качестве маркеров используются числа с точкой. Важной особенностью в данном случае является то, что сами номера, с помощью которых формируется список, не важны, так как они не оказывают влияния на выходной HTML код.

 Как бы ни нумеровал пользователь список, на выходе он в любом случае будет иметь упорядоченный список, начинающийся с единицы (1, 2, 3…). Эту особенность стоит учитывать в том случае, когда необходимо использовать порядковые номера элементов в списке, чтобы они соответствовали номерам, получающимся в HTML. Упорядоченные списки всегда следует начинать с единицы. 
 
 Маркеры списков обычно начинаются с начала строки, однако они могут быть сдвинуты, но не более чем на 3 пробела. За маркером должен следовать пробел, либо символ табуляции. 
 
 При необходимости в список можно вставить цитату. В этом случае обозначения цитирования ( «>» ) нужно писать с отступом. Упорядоченные списки выглядят следующим образом:
 1. Элемент списка с цитатой:
 >Это цитата
 
 >внутри элемента списка
 2. Элемент списка
 ***
## ***Изображения***
*** 
В Markdown существует 2 способа вставки изображений в документ:

+ С помощью непосредственного указания URL-адреса изображения. Синтаксис данной команды выглядит следующим образом:

        ![Альтернативный текст](/путь/к/изображению.jpg) или ![Альтернативный текст](/путь/к/изображению.jpg "Подсказка")
Иными словами, он состоит из следующих элементов:

восклицательный знак;
квадратные скобки, в которых указывается альтернативный изображению текст (он станет содержимым атрибута в элементе img);
круглые скобки, содержащие URL-адрес или относительный путь изображения, а также (необязательно) всплывающую подсказку, заключённуе в двойные или одиночные кавычки.
b. 

С помощью метки-идентификатора. Синтаксис данной команды записывается следующим образом:

    ![Альтернативный текст][id]
где «id» — имя определённой метки изображения. Метки изображений определяются при помощи синтаксиса, совершенно идентичного меткам гиперссылок:

[id]: путь/к/изображению "Необязательная подсказка"
Важной особенностью является то, что Markdown не позволяет задать размеры изображения (ширину, высоту).
***
## ***Горизонтальные линии*** 
***
Для того чтобы создать горизонтальную линию с использованием синтаксиса языка Markdown, необходимо поместить три (или более)дефиса или звездочки на отдельной строке текста. Между ними возможно располагать пробелы. 

Горизонтальные линии в Markdown выглядят следующим образом:

    Первая часть текста, который необходимо разделить
    ***
    Вторая часть текста, который необходимо разделить
    
    Или

    Первая часть текста, который необходимо разделить
    
    ---

    Вторая часть текста, который необходимо разделить
В результате на экран выводится следующее:

    Первая часть текста, который необходимо разделить

---

    Вторая часть текста, который необходимо разделить

При использовании данного инструмента важно помнить, что после первой части текста и перед второй необходимо оставлять пустую строку. Данное правило необходимо соблюдать только при использовании дефисов. Если его не соблюдать, на экран будет выведен заголовок второго уровня и строка обычного текста. При использовании символа звездочки данным правилом можно пренебречь.
***
## ***Ссылки***
***
Markdown поддерживает два стиля оформления ссылок:

Гиперссылка, с немедленным указанием адреса (внутритекстовая);
Гиперссылка, подобная сноске.
Подразумевается, что помимо URL-адреса существует еще текст ссылки. Он заключается в квадратные скобки. Для создания внутритекстовой гиперссылки необходимо использовать круглые скобки сразу после закрывающей квадратной. Внутри них необходимо поместить URL-адрес. В них же возможно расположить название, заключенное в кавычки, которое будет отображаться при наведении, но этот пункт не является обязательным.

    [пример](http://example.com/ "Необязательная подсказка")
В результате на экран выводится следующее: пример При ссылке на локальную директорию возможно использование относительного пути (от текущей страницы, сайта и т.п.)

При создании сносной гиперссылки вместо целевого адреса используется вторая пара квадратных скобок, внутри которых помещается метка, идентификатор ссылки (id).

    [пример][id]:
Также, можно использовать пробел, чтобы отделять 2 пары квадратных скобок:

    [пример] [id]: 
В этом случае возможно определить идентификатор в любом месте документа:

    [id]: http://example.com/ "Необязательная подсказка"
В результате на экран выводится следующее:  

    [пример] [id] [id]: http://example.com/ "Необязательная подсказка" 

Иными словами, она состоит из следующих элементов:

Идентификатор ссылки, окружённый квадратными скобками (которым может предшествовать необязательный отступ от одного до трёх пробелов);
Двоеточие;
Один или несколько пробелов (или символов табуляции);
URL гиперссылки;
Необязательный заголовок (подсказка к изображению, которая всплывает при наведении на него) гиперссылки, заключённый либо в двойные или одиночные кавычки, либо в скобки.
Идентификаторы ссылок могут состоять из букв, цифр, пробелов и знаков пунктуации, однако они не чувствительны к регистру. То есть эти два варианта эквивалентны:

    [текст ссылки][a]
    [текст ссылки][A]
Markdown позволяет также использовать неявно выраженный идентификатор (сокращенный). В этом случае метка не приводится, вместо неё текст гиперссылки используется и в качестве её имени, а вторая пара квадратных скобок остаётся пустою. Например, чтобы сделать слово «Example» гиперссылкой, ведущей на сайт "http://example.com/", достаточно написать:

    [Example][]
и затем определить гиперссылку:

    [Example]: http://example.com/
В результате на экран выводится следующее: 
    
    [Example][] [Example]: http://example.com/

***
## ***Работа с удаленными репозиториями в Git - GitHub***
***

**Как добавить ваш локальный репозиторий в общий доступ:**

1. Создать учетную запись, например, на GitHub

2. Слева сверху нажать на знак +

3. Откроется окно, где мы нажимаем "создать репозиторий"

4. После чего сервис предосталвет варианты того, что нам нужно сделать, чтобы репозиторий был добавлен на сервис

5. Выбираем наш случай и просто дублируем команды в VScode


        Если вы делаете это впервые, то вас попросят авторизироваться, чтобы объеденить сервис и ваш логин VScode

После авторизации мы можем увидеть, как наш файл отображается во вкладке "Code".

Изменения в локальном файле автоматически не отправляются на сервис. После авторизации, привязки локального репозитория и облачного сервиса для внесения изменений в облако, нам нужно просто ввести команду: **git push**.

Изменения в файл можно вносить в сервисе, то есть мы получим более актуальную версию файла в облаке, в любой момент сможем скопировать ссылку для того, чтобы открыть ее в VScode.

Также в сервисе, есть «история». Нажав на нее, мы можем посмотреть все коммиты.

В случае, если изменения были сделаны в удаленном репозитории, например, с другого компьютера, мы можем использовать команду **git pull**, чтобы "подтянуть" изменения в основную локальную версию файла. 

**Fork** - (с английского "вилка"), так называют ситуацию, когда кто-либо копирует чей-то проект, то есть, создает свой личный локальный репозиторий на основе чужого проекта.

Чтобы добавить удаленный репозиторий в VSCode, нам потребуется команда **git clone** и ссылка на репозиторий, который мы хотим скопировать.

В случае, если вы хотите предложить автору изменения в "форкнутый" проект, то на сервисе у вас появится кнопка "Compare & pull request". Вы сможете добавить комментарий к вашим изменениям.

GitHub автоматически проанализирует возможность мержа между вашей версией и версией автора.

Команда **cd** - позволяет сменить деректорию, после команды нужно ввести название папки, в которую мы хотим переместиться для дальнейшей работы с гитом.

