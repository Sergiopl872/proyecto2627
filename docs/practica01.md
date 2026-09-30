# PRACTICA 01 
### Autor: Sergiopl872
### Asignatura: Proyecto Intermodular

## 1. INSTALACIÓN Y CONFIGURACIÓN DE GIT.

Buscamos `git` en nuestro navegador y lo descargamos y ejecutamos el instalador.

Para comprobar que se ha instalado correctamente abrimos `PowerShell` y escribimos los siguientes comandos:

```bash
git --version
git config --global --list
```

![comprobar instalacion](/img/git-instalado-y-configurado.png)

Si aparece algo como eso significa que esta funcionando correctamente.


## 2. Inlación y configuración de GitHub CLI.

En este paso entraremos en https://cli.github.com/ y seguiremos los pasos encontrados en la pagina y los vamos copiando y pegando en orden en el `PowerShell`.

Para comprobar que todo ha ido bien pondremos los siguientes comandos y si todo esta correcto debe quedar algo asi:

```bash
gh --version
gh auth status
```

![githu cli instalado](/img/github-cli-instalado-y-configurado.png)


## 3. Instalación y configuración de Laravel Herd.

Entramos en https://herd.laravel.com/windows e instalamos `Laravel Herd` e instalamos la version 8.4 de `php`.

![herd configurado](/img/herd-instalado-con-la-version-84.png)


## 4. Clonación del repositorio.

En nuestro repositorio de `GitHub` encontraremos la URL de nuestro repositorio, debemos copiarla.

Vamos al `PowerShell` y ponemos `cd "ruta de la carpeta donde queramos copiarlo"` .

Y una vez en la ruta de la carpeta:

```bash
git clone https://github.com/usuario/mi-repositorio.git
```

Para comprobar que se ha copiado correctamente:

```bash
git status
git remote -v
```

![comprobacion](/img/repositorio-clonado-en-local.png)


## 5. Enlazar Herd 

Abrimo `Herd` y en el path copiamos la ruta de la carpeta donde queramos alojar nuestro servidor de php.

![herd enlazado](/img/herd-enlazado-con-el-repositorio-y-securizado.png)


## 6 Elementos y plugins.

Para realizar la documentación se utiliza el tema Read the Docs, configurado en el archivo `properdocs.yml`. Además, se han añadido diferentes extensiones de `Markdown` para ampliar las posibilidades de la documentación.


Se utiliza el tema:

```bash
theme:
  name: readthedocs
  locale: es
```

El tema Read the Docs proporciona la apariencia y estructura visual de la documentación. La opción locale: es configura el idioma en español.