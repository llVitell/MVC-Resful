# MVC-Resful
***
## Configuración
Primero instalamos sinatra y puma con los siguientes comandos
```Shell
gem install sinatra
gem install puma
```
Luego bundle y corremos el programa
```
cd sinatra-intro/
bundle install
ruby template.rb # O: bundle exec ruby template.rb
```
Ingresamos el siguiente enlace http://localhost:4567/todos en nuestro navegador para ver la página web y comprobar que esté funcionando. Este debería ser el resultado

![web](Imagenes/web.jpg)

El comando curl activa una solicitud `GET` para recuperar la lista de "cosas por hacer" y debería recibir una respuesta que se muestra en la salida estándar de la línea de comando.
```Shell
curl http://localhost:4567/todos
```
Este es el resultado en la terminal:
```Shell
[{"id":1,"description":"prepare for discussion section"},{"id":2,"description":"release cc 3s2"}]
```
***
## Parte 1
Usaremos `ActiveRecord` sobre una base de datos SQLite. En esta aplicación, ¿cuál será nuestro modelo y qué operaciones CRUD le aplicaremos?