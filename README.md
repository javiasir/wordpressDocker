# wordpressDocker
El docker-compose para levantar un wordpress, con variables que están en un archivo diferente y una carpeta plugins que habría que crear donde se podrían colocar los plugins iniciales que quisieramos.

Se podría incluir si quisieramos algun theme para nuestra página web creando una carpeta nueva por ejemplo que se llamase "themes" y introduciendolos ahí. Además habría que crear un volumen que fuese:

volumes:
  - ./themes:/var/www/html/wp-content/themes

Recordar que al crear estas carpetas los archivos por defectos que trae wordpress desaparecen, asi que si interesa mantenerlos, es posible desplegarlo primero para sacar esos archivos y meterlos en estas carpetas para cuando se vaya hacer el despliegue real estos permanezcan.
