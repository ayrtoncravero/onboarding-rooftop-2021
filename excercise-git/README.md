# Onboarding - Rooftop
## Aprendiendo a utilizar git y github
---
## Ejercicio de git:
1- Creamos una carpeta, utilizando el siguiente comando (Gnu/linux):
```
mkdir excercise-git
```

2- Nos movemos a la carpeta con:
```
cd excercise-git
```

3- Iniciamos git en la carpeta:
```
git init
```

4- Creamos el archivo '.gitignore':
```
touch .gitignore
```

5- Creamos un archivo 'README.md':
```
touch README.md
```

6- Abrimos el archivo 'README.md' usando nuestro editor de texto favorito, en este caso pos simplicidad voy a usar 'nano':
```
nano README.md
```
* Se nos va a abrir un ediitor en la consola que estemos utilizando, dentro introducimos el texto de instrucciones sobre el proyecto.
* Al finalizar de escribir presionamos 'Ctrl + O', de esta manera guardamos los cambios
* Seguido presionamos 'Enter'.
* Y por ultimo presionamos 'Ctrl + X', de esta manera cerramos nano.

7- Para comprobar que fueron afectados correctamente los archivos, corremos el siguiente comado:
```
git status
```
* El mismo nos indicara en color rojo el nombre de los archivos afectados.

8- Ahora vamos a agregar esos archivos, con el siguiente comando le indicaremos a git que los tracke:
```
- git add README.md
- git add .gitignore
```
* De esta manera git trackea los dos archivos

9- Si corremos git status vamos a ver que los archivos estan en color verde, eso significa que efectivamente git los esta siguiendo.

10- Ahora vamos a 'commitear' esos 2 cambios, corriendo el siguiente comando:
```
git commit -m "Se agrego 'README.md' y '.gitignore'"
```
* Dentro de "" se debe de indicar de manera breve y consisa que es lo que se cambio.

11- Para finalizar vamos a enviar nuestros commits a nuestro repositorio de github:
* Para hacerlo debemos de registrarnos y crear un repositorio en la plataforma de github

```
git remote add origin git@github.com:ayrtoncravero/onboarding-rooftop-2021.git
```
* Con ese comado le indicamos a git cual va a ser el repositorio al que vamos a enviar todos los commits.

12- Para finalizar corremos el siguiente comando:

```
git push -u origin master
```
* De esta manera enviamos todos los cambios que estan en 'staging area' a nuestro repositorio de github.

---
## Para investigar:
Sobre GIT:

- ¿Qué es una rama?

Es un espacio, una bifurcacion de una rama principal, normalmente 'Master'

- ¿Qué hacen los comandos add / commit / push?

a- Add: Se utiliza para agregar a staging los cambios.

b- Commit: Se utiliza para dejar una descripcion que expliquen los cambios que hicimos en los archivos.

c- Push: Se utiliza para enviar cambios, normalmente a 'staging area'.

- Diferencia entre pull y push

a- Pull se utiliza para traer cambios a local(working directory), mientras que push para enviar cambios(Ej: Enviar cambios a master).

- Diferencia entre clone e init

a- Clon se utiliza para clonar un repositorio que esta en github, mientras que Init se utiliza para inicializar el 'servicio' de gir en un directorio.

Sobre Markdown:

- ¿Es un lenguaje de programación?

a- No, es un lenguaje de marcado, similar a HTML.

- ¿Para qué se suele usar comúnmente?

a- Normalmente es utilizado para documentar.

- ¿Qué otro lenguaje es similar?

a- Un lenguaje muy similar es HTML, reStructuredText.
