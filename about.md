---
layout: page
title: посты
permalink: /about/
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

### Jekyll *умеет* раскрашивать ваш код 

```python
import telebot
import openai

TOKEN = ''  
openai.api_key = ''

#

bot = telebot.TeleBot( TOKEN )

@bot.message_handler( func = lambda message: True )
def echo( message ):
  #    bot.send_message( message.chat.id, message.text )
  message_text = message.text

  if message_text != '/start' :
    response = openai.ChatCompletion.create(
      model = "gpt-3.5-turbo",
      messages = [
        { "role": "system", "content": "You are a helpful assistant" },
        { "role": "user", "content": message_text }
      ]
    )

    response = response['choices'][0]['message']['content'].strip()
       
    bot.send_message( message.chat.id, response )

if __name__ == '__main__':
  bot.polling( none_stop = True )

```
~

Книжное братство [flibusta.is](https://flibusta.is)

Какие версии поддерживает gp ? [gp.com/versions](https://pages.github.com/versions)

( gp = github pages )

hugo [hugo](https://hisava.github.io/hugo)

# My thanks to Skill Network ( for this [page](https://veretennikovalexey.github.io/ll) )

---------------

## Милая собачка ( фото )


[PY0101EN-5.4_WorkingWithDifferentFileTypes.ipynb][FileTypes]

[FileTypes]: https://github.com/hisava/hisava.github.io/blob/main/PY0101EN-5.4_WorkingWithDifferentFileTypes.ipynb


# [Этот сайт][hisava.github.io] ( т.е. hisava.github.io ) был создан

[вот по этой инструкции][bill-gist] ( англ. )

[hisava.github.io]: https://hisava.github.io 'hisava.github.io'

[bill-gist]:   https://gist.github.com/BillRaymond/db761d6b53dc4a237b095819d33c7332

[Моя первая лаборатория][try]

[try]: https://github.com/hisava/hisava.github.io/blob/main/try.ipynb

[PY0101EN-5.2_API_2.v2.ipynb][5.2]

[5.2]: https://github.com/hisava/hisava.github.io/blob/main/PY0101EN-5.2_API_2.v2.ipynb

[PY0101EN-5.3_Requests_HTTP.ipynb][HTTP]

[HTTP]: https://github.com/hisava/hisava.github.io/blob/main/PY0101EN-5.3_Requests_HTTP.ipynb

[PY0101EN-5.1_Intro_API.ipynb][api]

[api]: https://github.com/hisava/hisava.github.io/blob/main/PY0101EN-5.1_Intro_API.ipynb

[labs_module-1_Web-Scraping_Web-Scraping-Review-Lab.ipynb][Web-Scraping]

[Web-Scraping]: https://github.com/hisava/hisava.github.io/blob/main/labs_module-1_Web-Scraping_Web-Scraping-Review-Lab.ipynb

# numpy

[numpy.ipynb][numpy.ipynb]

[numpy.ipynb]: https://github.com/hisava/hisava.github.io/blob/main/numpy.ipynb

# Объекты и классы в питоне

[Азбука][objects-and-classes] 

[objects-and-classes]: https://github.com/hisava/hisava.github.io/blob/main/objects-and-classes.ipynb

## Запись в файл на языке питон

[Простой пример][writefile]

[writefile]: https://github.com/hisava/hisava.github.io/blob/main/writefile.ipynb

