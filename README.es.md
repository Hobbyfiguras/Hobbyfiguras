# Hobbyfiguras
Hobbyfiguras es una comunidad de coleccionistas de figuras, aquí podrás encontrar tutoriales, guías, novedades, comparativa de figuras falsas, dudas, tiendas, y las ultimas noticias.

En este repositorio encontrarás la documentación y los links al codigo fuente del foro, el foro ahora mismo es muy especifico para las necesidades de hobbyfiguras, pero en el futuro podria adaptarse para otros usos.

## Información tecnica

### Backend

El backend del foro está hecho en Python 3 usando django, utilizamos django rest framework para proveer la API y whoosh para las busquedas.

El sitio se ejecuta usando uvicorn (para que funcione como una aplicación ASGI, para las notificaciones en tiempo real).

En el servidor también se utiliza un programa llamado prerender, para que google y compañia puedan ver la información sin necesidad de ejecutar Javascript.

Hay tres aplicaciones, FigureSite, que contiene todo el foro y mfc, que hace de wrapper para poder obtener datos de MyFigureCollection.

### Frontend

El frontend funciona con Vue.js y Node, el parseador de markdown es markdown-it, aunque está customizado para soportar los emojis de twitter (como en Discord) y poder poner imagenes de MFC, insertar videos de YouTube etc...

## Links del proyecto

- [Frontend del foro](https://github.com/Hobbyfiguras/frontend)
- [Backend del foro](https://github.com/Hobbyfiguras/backend)
- [Prerender](https://github.com/Hobbyfiguras/prerender-hobbyfiguras)
- [vue-markdown](https://github.com/Hobbyfiguras/vue-markdown)
- [Extensiones de markdown-it](https://github.com/Hobbyfiguras/markdown-it-figuresite)
- [Scripts](https://github.com/Hobbyfiguras/scripts)
- [Django-rest-framework-simplejwt](https://github.com/Hobbyfiguras/django-rest-framework-simplejwt)
