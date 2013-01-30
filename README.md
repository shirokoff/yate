Yet Another Template Engine
============================

Бла-бла-бла
-----------

  * Хочется заменить шаблонизатор в Я.Почте.
    Сейчас это xslt, исполняющийся на клиенте.

  * Как минимум новые шаблоны должны уметь компилироваться в javascript и
    работать с даннымми в формате json, превращая их в html.

  * Не исключается также компиляция и в другие языки. Например, в perl.

  * Шаблонизатор должен быть быстрым.
    Поэтому синтаксис и набор фич ограничивается в первую очередь
    возможностью компиляции в быстро работающий javascript.

  * Шаблонизатор не должен никаким образом модифицировать входящие данные.

  * Синтаксис не должен быть xml'ным,
    но общие принципы xslt (pattern matching шаблонов, xpath) должны сохраниться.


Установка
---------

  * Установить [node.js](https://github.com/joyent/node/wiki/Installation).

  * Если не планируется разработка `yate`, то:

        npm install -g yate

  * Если предполагается изменять код и т.д., то:

        git clone git@github.com:pasaran/yate.git
        git clone git@github.com:pasaran/parse-tools.git
        cd yate
        npm install nopt
        npm link ../parse-tools


Компиляция
----------

  * Компиляция шаблона запускается так:

        yate test.yate > test.js

  * Компиляция и исполнения шаблона:

        yate test.yate test.json > test.html


Документация
------------

Пока ее практически нет :)
Можно прочитать про [базовый синтаксис](https://github.com/pasaran/yate/wiki/syntax)
и про [синтаксис jpath](https://github.com/pasaran/yate/wiki/jpath).

И еще есть [слайды](http://pasaran.github.com/slides/yate/) с внутреннего доклада в Яндексе.



