---
layout: post
title:  "PowerShell"
date:   2023-08-16 12:00:00 +0300
categories: jekyll update
---

[PowerShell](https://github.com/PowerShell/PowerShell) это программа от фирмы Microsoft

В последних системах windows она используется в качестве терминала

Для того, чтобы написать скрипт на *ps* надо создать файл с расширением `ps1`

Скрипт поддерживает команды *unix*, например, `ls`

Пример команды

`ls e:/ee | random | mi -dest C:\fabius\_`

Она означает: посмотреть содержимое папки ЕЕ на диске Е, выбрать случайно любой файл

и переместить его ( move item ) в папку `c:\Fabius`

<br>
# в unix \ в powershell `

В терминале linux для продолжения команды, если вся команда

не влезла в строку, используется символ \ ( backslash )

Но в системах windows этот символ используется для разделения папок

Поэтому, в windows вместо *backslash* используется символ ё ` ( back quote )

Вот пример POST запроса из статьи про [curl](https://hisava.github.io/jekyll/update/2023/08/20/Post8-curl.html)

    curl -X 'POST' `
    'https://petstore.swagger.io/v2/pet' `
    -H 'accept: application/json' `
    -H 'Content-Type: application/json' `
    -d '{
    "name" : "alex",
    "status": "available"
    }'
