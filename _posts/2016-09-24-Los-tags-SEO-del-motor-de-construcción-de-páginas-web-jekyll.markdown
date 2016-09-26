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
<img src="/images/what.jpg" />

  {% highlight liquid %}
  {% seo %}
  {% endhighlight liquid %}<br><br>

## Funcionamiento

El tag de SEO respeta cualquier cosa de lo siguiente si es incluído en el documento `_config.yml` de tu sitio (y simplemente no incluir si no está definidio ahí):

* `title` - El título de tu sitio (o sea, el magnífico sitio de Ben, El Blog de Github, etc.)
* `description` - Una descripción corta de tu sitio (o sea, un sitio dedicado a fotos de gatos, etc.)
* `url` - El URL completo de tu sitio. Nota: `site.github.url` será usado por defecto.
* `author` - Información global del autor (leer abajo)
* `twitter:username` - El nombre del sitio usado en Twitter. Lo defines de la siguiente manera:

  {% highlight yml %}
  twitter:
    username: benbalter
  {% endhighlight yml %}

* `facebook` - Las siguientes propiedades se encuentran:
* `facebook:app_id` - El ID del app de Facebook debido a internas de Facebook.
* `facebook:publisher` - Una URL o ID de la página de Facebook del ente de la publicación.
* `facebook:admins` - El ID de un usuario de Facebook debido a internas relacionadas al dominio asociado a una cuenta personal.

  Los defines uno o más de la siguiente manera:

{% highlight yml %}
  facebook:
    app_id: 1234
    publisher: 1234
    admins: 1234
{% endhighlight yml %}

* `logo` - URL de un logo general para todo el sitio (o sea, `/assets/your-company-logo.png`)
* `social` - Para <a href="//developers.google.com/structured-data/customize/social-profiles"><span>especificar perfiles sociales</span></a>. Se encuentran las siguientes propiedades:
   * `name` - Si el usuario o la organización difiere del nombre del sitio.
   * `links` - Un conjunto de enlaces a los perfiles de los medios sociales.
   * `google_site_verification` Parsa verificar pertenencia e propiedad por la herramienta Google webmaster tools.

El tag SEO respetará la siguiente configuración YAML (front matter) en cualquier posteo, página o documento:

* `title` - Eltítulo del posteo, página o documento.
* `description` - Una descripción corta del contenido del posteo, página o documento.
* `image` - URL de cualquier imágen asociada al posteo, página o documento (o sea, `/assets/page-pic.jpg`)
* `author` - Información específica del autor del posteo, página o documento (leer abajo.)

## Uso avanzado

El tag SEO de jekyll está diseñado para implementar SEO de la mejor forma que se recomienda por defecto y de esa manera ajustarse a cualquier construcción de sitio y arranque inicial del sitio. Si por alguna causa necesitas aún más control sobre los tags continúa leyendo:

### Desabilitando resultado `<title>`

Si por alguna razón no quieres producir el resultado de los tags de  `<title>` en cada página, simplemente invoca el plugin dentro de tu template de la siguiente manera:
<img src="/images/title-false.jpg" />
{% highlight liquid %}
{% seo title=false %}
{% endhighlight liquid %}

### Información del autor

La información del autor es utilizada para propagar el campo `creator` en tarjetas resúmenes Twitter. Ésto debería asociar el autor específico, y no un nombre Twitter general usado en todo el sitio (el nombre de uso general en todo el sitio es almacenado en `site.twitter.username`).

*TL;DR: En la mayoría de los casos, poner `author: [your Twitter handle]` en el front matter del documento, para sitios con múltiples autores. Si necesitas algo más complicado continúa leyendo*

Hay varias formas de resumir ésta información específica del autor. La información del autor se encuentra en el siguiente orden de prioridades:

1. El objeto `author` en el front matter del documento, o sea.:

  {% highlight yml %}
  author:
    twitter: benbalter
  {% endhighlight yml %}

2. El obieto `author` en el documento `_config.yml` de tu sitio, o sea.:

  {% highlight yml %}
  author:
    twitter: benbalter
  {% endhighlight yml %}

3. `site.data.authors[author]`, si un autor es nombrado en el front matter del documento, y una llave correspondiente existe en `site.data.authors`. O sea, tenés lo siguiente especificado en el front matter del documento:

  {% highlight yml %}
  author: benbalter
  {% endhighlight yml %}

  Y tenés lo siguiente especificado en `_data/authors.yml`:

  {% highlight yml %}
  benbalter:
    picture: /img/benbalter.png
    twitter: jekyllrb

  potus:
    picture: /img/potus.png
    twitter: whitehouse
  {% endhighlight yml %}

En el ejemplo de arriba, el autor `benbalter`'s Twitter handle será resuelto como `@jekyllrb`. Ésto te permite centralizar información del autor en el documento `_data/authors` para sitios con más de un autor que simplemente el nombre de usuario del autor

  *Consejo-pro: Si `authors` está presente en el front matter del documento como un conjunto de varios (y `author` no), el plugin usará el primer autor de la lista, ya que Twitter soporta un solo autor por obra.*


4. Un autor en el front matter del documento (la forma más fácil), o sea.:

  {% highlight yml %}
  author: benbalter
  {% endhighlight yml %}

5. Un autor en el documento `_config.yml` de tu sitio, o sea.:

  {% highlight yml %}
  author: benbalter
  {% endhighlight yml %}









