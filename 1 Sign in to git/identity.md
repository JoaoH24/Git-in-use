# Definir tu identidad
Antes de iniciar con el uso de git, es requerido que configuremos el archivo `.gitconfig` con nuestra información.\
Para poder modificar el archivo `.gitconfig` se describe el siguiente comando:\
~~~bash
git config --global -e
~~~
El comando anterior nos abrirá un editor de texto como nano, vim o emacs que funcionan desde la linea de comandos. Se nos mostrará la siguiente información:
~~~bash
# Este es el archivo de configuración de Git por usuario.
# This file defines your configuration for your git user
[user]
        name = pinwi pinwinasio
        email = pinwinasio.f@gmail.com
[core]
        editor = nvim
~~~
Podemos editar este archivo de configuración con los datos como el nombre de usuario y email con el formato `name = pinwinasio` [atributo = valor:].
Otra manera que tenemos de configrar estos atributos son de manera individual con los siguientes comandos:
~~~bash
git config --global user.name "pinwi pinwinasio"
~~~
~~~bash
git config --global user.email pinwinasio@gmail.com
~~~
Este comando es opcional, ya que define el editor que usará git para la interacción el usuario. Puedes configurar este apartado con el editor de texto de tu preferencia.
~~~bash
git config --global core.editor = nvim
~~~
Por ultimo podemos visualizar los atributos que configuramos con el siguiente comando:
~~~bash
git config --global --list
~~~
Una pequeña aclaración que podemos hacer aquí es:
- El parámetro `--global` configura estos atributos de manera global. Si deseas configurar estos atributos de manera individual para un proyecto con git simplemente retira el parámetro `--global`.
~~~bash
git config user.nama = CGalleta
~~~
Podemos visualizar los atributos de manera individual para un proyecto con el siguiente comando:  
~~~bash
git config --list
~~~