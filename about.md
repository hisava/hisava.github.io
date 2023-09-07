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

