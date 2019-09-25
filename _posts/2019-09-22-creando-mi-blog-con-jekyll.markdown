---
layout: post
title:  "Creando mi blog con Jekyll! el creador de sitios web estaticos"
date:   2019-09-22 15:30:18 -0500
categories: cms web desarrollo
permalink: /creando-mi-blog-con-jekyll/
---

21 de septiembre de 2019. Empiezo el proyecto de crear mi blog *(este blog)* con la tecnologia para creacion de sitios web estaticos **`jekyll`**. 

Acabo de terminar de ver los videos de [Mike Dane](https://www.youtube.com/channel/UCvmINlrza7JHB1zkIOuXEbw/), un youtuber que tiene una serie muy completa de [introduccion a jekyll](https://youtu.be/T1itpPvFWHI), la cual recomiendan desde la misma pagina [web de jekyll](https://jekyllrb.com/).

Mi sistema operativo es Archlinux. Comienzo instalando `rubygems` el paquete que contiene `ruby` y el paquete `gem`. Luego instalo las gemas `jekyll` y `bundler` para después generar mi sitio web.


#### **Instalando rubygems**
{% highlight bash %}
➜  ~ sudo pacman -S rubygems
{% endhighlight %}


#### **Instalando las gemas**
{% highlight bash %}
➜  ~ gem install jekyll bundler
{% endhighlight %}
  

Luego genero mi nuevo sitio web con el nombre yosoypc.

#### **Generando el sitio web**
{% highlight bash %}
➜  ~ jekyll new yosoypc
{% endhighlight %}

Ingreso a la carpeta generada y listo los archivos contenidos.

{% highlight bash %}
➜  Miweb cd yosoypc
➜  yosoypc ll
total 32K
-rw-r--r-- 1 brian brian  419 sep 21 15:59 404.html
-rw-r--r-- 1 brian brian  539 sep 21 15:59 about.markdown
-rw-r--r-- 1 brian brian 2,1K sep 22 15:14 _config.yml
-rw-r--r-- 1 brian brian 1,1K sep 21 15:59 Gemfile
-rw-r--r-- 1 brian brian 2,0K sep 21 16:02 Gemfile.lock
-rw-r--r-- 1 brian brian  175 sep 21 15:59 index.markdown
drwxr-xr-x 2 brian brian 4,0K sep 22 15:37 _posts
drwxr-xr-x 6 brian brian 4,0K sep 22 15:37 _site
{% endhighlight %}

Después de generado el sitio inicio una instancia de servidor web que genera jekyll, para poder acceder al sitio desde el navegador.

{% highlight bash%}
➜  yosoypc bundle exec jekyll serve
{% endhighlight %}

y por ultimo cargo la pagina de inicio accediendo a `http://localhost:4000`

![mi sitio web con jekyll](/assets/img/cargando-web-con-jekyll.png)

**LISTO!** mi sitio web con Jekyll está generado correctamente de manera local en mi PC. Este es mi primer post. Ahora lo subire a github y continuare creando nuevos posts y haciendo mejoras y personalizaciones. 

**SIGUIENTE POST:** [Subiendo mi sitio web generado con Jekyll a github](#)