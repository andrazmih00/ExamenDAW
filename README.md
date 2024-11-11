# ExamenDAW
# Examen Andrei Razvan Mihai

## Motivacion
Mi motivacion en este examen es sacar la mejor nota posible.

## Introduccion
Aqui explicare mi contenido del examen de Despliegue de Aplicaciones Web de 2ºDAW en mi centro de estudios AgilCentros.
Este trabajo esta creado en [MarkDown] y explicare los pasos seguidos para superar el examen.


## Actividades realizadas

### Ejercicio 2

 - sudo apt install openssh-server
 - ssh usuario@192.168.0.185
 - usuario@192.168.0.185's password:
 - ls
 - cd Escritorio
 - touch AndreiRazvanMihai.txt
 - nano AndreiRazvanMihai.txt (añadimos en la primera linea usuario y en la segunda linea who. Guardamos y salimos.
 - cat AndreiRazvanMihai.txt (para ver si funciona nuestro comando whoami)
 
### Ejercicio 3

 - sudo apt install apache2
 - sudo ufw app list
 - sudo ufw allow 'Apache'
 - sudo ufw status
 - sudo systemctl status apache2
 - hostname -I (192.169.0.129 nuestra direccion IP)
 - sudo systemctl start apache2
 - sudo systemctl enable apache2
 - sudo mkdir /var/www/miWeb
 - sudo chown -R $USER:$USER /var/www/miWeb
 - sudo chmod -R 755 /var/www/miWeb
 - sudo nano /var/www/miWeb/index.html (agregamos nuestro estilo html guardamos y salimos)
 - sudo nano /etc/apache2/sites-available/miWeb.conf (En ServerName agregamos el nombre de nuestro servidor, ServerAlias agregamos daw.ejercicio3.com y DocumentRoot nuestro /var/www/miWeb creado anteriormente. Guardamos y salimos
 - sudo a2ensite miWeb.conf
 - sudo a2dissite 000-default.conf
 - sudo apache2ctl configtest (deberia imprimir en consola Syntax Ok)
 - sudo systemctl restart apache2
 - y por ultimo entrar http://daw.ejercicio3.com/ y disfrutar de la magia
 
## Conclusiones

Como programador novato espero superar con creces esta prueba realizada por Daniel. Muchas gracias por tu atencion.

## Bibliografia
 - [Ejercicio1](https://markdownlivepreview.com/?authuser=0)
 - Ejercicio 2: a partir de ejercicios hechos por mi.
 - [Ejercicio 3](https://www.digitalocean.com/community/tutorials/how-to-install-the-apache-web-server-on-ubuntu-20-04-es?authuser=0)
