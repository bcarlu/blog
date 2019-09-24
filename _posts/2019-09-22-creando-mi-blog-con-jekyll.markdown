---
layout: post
title:  "Creando mi blog con Jekyll! el creador de sitios web estaticos"
date:   2019-09-22 15:30:18 -0500
categories: tecnologias-de-desarrollo-web
---

El dia de ayer 21 de septiembre de 2019 inicie mi proyecto de crear mi blog (este blog) con la tecnologia de sitios estaticos jekyll. Acabo de terminar de ver los videos de [Mike Dane](https://www.youtube.com/channel/UCvmINlrza7JHB1zkIOuXEbw/), un youtuber que tiene una serie muy completa de [introduccion a jekyll](https://youtu.be/T1itpPvFWHI).

Mi sistema operativo es Archlinux y el primer reto fue instalar ruby y las gemas `jekyll` y `bundler` qué, según el sitio [web de jekyll](https://jekyllrb.com/) son las gemas que debemos instalar para poder generar nuestro sitio.


#### **Instalando ruby**
{% highlight bash %}
➜  ~ sudo pacman -S rubygems
{% endhighlight %}


#### **Instalando las gemas**
{% highlight bash %}
➜  ~ gem install jekyll bundler
{% endhighlight %}

Luego generé el sitio web dentro de mi directorio destinado para tal fin.

#### **Generando el sitio web**
{% highlight bash %}
➜  ~ jekyll new yosoypc
{% endhighlight %}

{% highlight bash %}
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

Después de generado el sitio inicié una instancia de servidor web que se genera con jekyll, para poder acceder al sitio desde el navegador web.

{% highlight bash%}
➜  yosoypc bundle exec jekyll serve
{% endhighlight %}

y luego confirmé que todo cargara correctamente. Accediendo a `http://localhost:4000`

![mi sitio web con jekyll](/assets/img/cargando-web-con-jekyll.png)

LISTO! Mi sitio web de Jekyll se generó y cargó correctamente. Ahora empiezo a crear algunos post, el primero es este. Luego lo subire a github y continuare realizando mejoras y personalizaciones. 