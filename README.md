![](https://i.imgur.com/woEBLxs.png)

# Hobbyfiguras
Hobbyfiguras is a figure collector community, in the site you will find tutorials, guides, news, bootleg comparisons, answers, stores and the latest news.

This repository is a central information hub, here you will find the links to the main code repositories, right now the source code for the site is very specific for our particular needs, but in the future it could be made into a generic package for other uses.

The forum itself has some inspirations from facepunch forums.

## Technical information

### Backend

The backend of the forum is done in Python 3 using django, we use django rest framework to provide the API and whoosh for the searches.

The site is used using uvicorn (to function as an ASGI application, for real-time notifications).

A program called Prerender is also used on the server, so that Google and the rest of bots can see the information without having to execute Javascript.

There are three applications, FigureSite, which contains the entire forum and mfc, which is an intermediary to get and parse data from MyFigureCollection.

### Frontend

The frontend works with Vue.js and Node, the markdown parser is markdown-it, although it is customized to support the emojis of twitter and to be able to insert images of MFC, insert videos from YouTube etc ...

## Project links

- [Frontend](https://github.com/Hobbyfiguras/frontend)
- [Backend](https://github.com/Hobbyfiguras/backend)
- [Prerender](https://github.com/Hobbyfiguras/prerender-hobbyfiguras)
- [vue-markdown](https://github.com/Hobbyfiguras/vue-markdown)
- [markdown-it extensions](https://github.com/Hobbyfiguras/markdown-it-figuresite)
- [Scripts](https://github.com/Hobbyfiguras/scripts)
- [Django-rest-framework-simplejwt](https://github.com/Hobbyfiguras/django-rest-framework-simplejwt)
