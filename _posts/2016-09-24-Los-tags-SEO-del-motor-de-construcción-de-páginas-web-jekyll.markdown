---
layout: default
title: "Los tags SEO del motor de construcción de páginas web jekyll"
date: 2016-09-24 13:41:21 +02:00
categories: jekyll seo-tag
---


# Los tags SEO del motor de construcción de páginas web jekyll

<html><p class="meta">Posted by <a href="//abuseombudsman.github.io">abuseombudsman</a> on September 24, 2016
				&nbsp;&bull;&nbsp; <a href="#" class="comments">Comments </a> &nbsp;&bull;&nbsp; <a href="permalink'" class="permalink">Full article</a>
		</p><p><img src="/images/zodìaco.jpg" width="186" height="186" alt="" class="alignleft border" /></p>
<p><a href="//badge.fury.io/rb/jekyll-seo-tag"><img src="//badge.fury.io/rb/jekyll-seo-tag.svg"></a>  <a href="//travis-ci.org/jekyll/jekyll-seo-tag"><img src="//travis-ci.org/jekyll/jekyll-seo-tag.svg"></a></p></html>

Extensión de jekyll que permite agregar tags de metadatos a motores de búsqueda y redes sociales
para obtener mejor posicionamiento en los resultados de búsqueda y para mostrar mejor el contenido de tu página.<br><br>

## Que es lo que hace la extensión

Los tags SEO del motor de construcción del site agregan los siguientes tags de metadatos a tu sitio:<br><br>
<pre><span style="color: #810A0A;">*</span><span> Los títulos de las páginas (pegado con el título del site si éste existiese)</span>
<span style="color: #810A0A;">*</span><span> La descripción de la página</span>
<span style="color: #810A0A;">*</span><span> El URL canónico</span>
<span style="color: #810A0A;">*</span><span> Próximo url y anterior url, en páginas paginadas en varias páginas </span>
<span style="color: #810A0A;">*</span><a href="//developers.google.com/structured-data/"><span style="color #4439DC;"> SITIO JSON-LD y los metadatos de las postiadas</span></a> para obtener un indexing más completado
<span style="color: #810A0A;">*</span><a href="//ogp.me/"><span style="color #4439DC;"> Open Graph</span></a> título de la página, descripción de la página, título del sitio y URL:es (de Facebook, LinkedIn, etc)
<span style="color: #810A0A;">*</span> <a href="//dev.twitter.com/cards/overview"><span style="color #4439DC;">Tarjeta de resúmen de Twitter</span></a> metadatos</pre>

Mientras tu podrías agregar los tags de metadatos por tu cuenta, los tags SEO están probados por fuego y mantienen todas las etiquetas foguiadas.<br><br>

## Que es lo que no hace la extensión

El tag SEO de jekyll está diseñado para enviar metadatos que pueden ser leídos por una máquina para ser indexados y mostrados por motores de búsqueda y redes sociales. Si tú estás buscando una herramienta para analizar la estructura y el contenido del site de jekyll (o sea optimizaciones SEO más tradicionales) te puede interesar <a href="//github.com/pmarsceill/jekyll-seo-gem"><span style="color #4439DC;">La gema: SEO de jekyll. </span></a>

El tag SEO de jekyll no está diseñado para cubrir todas las posibilidades habidas y por haber sobre el uso de los tags, sin embargo deberían funcionar correctamente para cualquier site normal y sin la necesidad de miles de opciones de configuración que solamente terminan por confundir a los usuarios.
<br><br>


## Instalación

1. Agrega lo siguiente al documento `Gemfile` de tu sitio:

  {% highlight ruby %}
  gem 'jekyll-seo-tag'
  {% endhighlight ruby%}<br><br>

2. Agrega lo siguiente al documento `_config.yml` de tu sitio:

  {% highlight yml %}:
  gems:
    	- jekyll-seo-tag
  {% endhighlight yml %}<br><br>

3. Agrega lo siguiente antes de la etiqueta `</head>` en el/los template/templates de tu sitio:

  {% highlight liquid %}
  {% seo %}
  {% endhighlight liquid %}<br><br>

## Usage

The SEO tag will respect any of the following if included in your site's `_config.yml` (and simply not include them if they're not defined):

* `title` - Your site's title (e.g., Ben's awesome site, The GitHub Blog, etc.)
* `description` - A short description (e.g., A blog dedicated to reviewing cat gifs)
* `url` - The full URL to your site. Note: `site.github.url` will be used by default.
* `author` - global author information (see below)
* `twitter:username` - The site's Twitter handle. You'll want to describe it like so:

  ```yml
  twitter:
    username: benbalter
  ```







