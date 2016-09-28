---
layout: post
title:  "Jekyll SEO Tag - 2.0.0"
date:   2016-09-28 05:52:19 +02:00
categories: jekyll jekyll-seo-tag-2.0.0
image: "/assets/deploy-engine.jpg"
---
<div id="entry">
						<div class="Los SEO">
							<h2 class="title"><a href="//localhost:4000/jekyll/jekyll-seo-tag-2.0.0/2016/09/28/Los-SEO-Tags-de-Jekyll-2.0.0.markdown">Los SEO Tags de Jekyll 2.0.0</a></h2>
						</div>
							<p class="meta">Posted by <a href="//abuseombudsman.github.io">abuseombudsman</a> on September 28, 2016
								&nbsp;&bull;&nbsp; <a href="#" class="comments">Comments </a> &nbsp;&bull;&nbsp; <a href="//localhost:4000/jekyll/jekyll-seo-tag-2.0.0/2016/09/28/Los-SEO-Tags-de-Jekyll-2.0.0.markdown" class="permalink">Full article</a></p>
							
								<p><img src="/images/zodìaco.jpg" width="186" height="186" alt="" class="alignleft border" />Extensión de jekyll que permite agregar tags de metadatos a motores de búsqueda y redes sociales para obtener mejor posicionamiento en los resultados de búsqueda y para mostrar mejor el contenido de tu página.</p><br><br>
 
<p><a href="//badge.fury.io/rb/jekyll-seo-tag"><img src="//badge.fury.io/rb/jekyll-seo-tag.svg"></a>  <a href="//travis-ci.org/jekyll/jekyll-seo-tag"><img src="//travis-ci.org/jekyll/jekyll-seo-tag.svg"></a></p><br><br>
</div>

<div id="entry">
						<div class="Los SEO">
							<h2 class="title">Que es lo que hace la extensión</h2><br>
						</div>

<p>Los tags SEO del motor de construcción del sitio agregan los siguientes tags de metadatos a tu sitio:</p>
<p><pre><span style="color: #810A0A;">*</span><span> Los títulos de las páginas (pegado con el título del site si éste existiese)</span>
<span style="color: #810A0A;">*</span><span> La descripción de la página</span>
<span style="color: #810A0A;">*</span><span> El URL canónico</span>
<span style="color: #810A0A;">*</span><span> Próximo url y anterior url, en páginas paginadas en varias páginas </span>
<span style="color: #810A0A;">*</span><a href="//developers.google.com/structured-data/"><span style="color #4439DC;"> SITIO JSON-LD y los metadatos de las postiadas</span></a> para obtener un indexing más completado
<span style="color: #810A0A;">*</span><a href="//ogp.me/"><span style="color #4439DC;"> Open Graph</span></a> título de la página, descripción de la página, título del sitio y URL:es (de Facebook, LinkedIn, etc)
<span style="color: #810A0A;">*</span> <a href="//dev.twitter.com/cards/overview"><span style="color #4439DC;">Tarjeta de resúmen de Twitter</span></a> metadatos</pre></p><br>
<p>Mientras tu podrías agregar los tags de metadatos por tu cuenta, los tags SEO están probados por fuego y mantienen todas las etiquetas foguiadas.</p></div><br>

<div id="entry">
						<div class="Los SEO">
							<h2 class="title">Que es lo que no hace la extensión</h2><br>
						</div>

<p>El tag SEO de jekyll está diseñado para enviar metadatos que pueden ser leídos por una máquina para ser indexados y mostrados por motores de búsqueda y redes sociales. Si tú estás buscando una herramienta para analizar la estructura y el contenido del site de jekyll (o sea optimizaciones SEO más tradicionales) te puede interesar <a href="//github.com/pmarsceill/jekyll-seo-gem"><span style="color #4439DC;">La gema: SEO de jekyll. </span></a></p><br>
<p>El tag SEO de jekyll no está diseñado para cubrir todas las posibilidades habidas y por haber sobre el uso de los tags, sin embargo deberían funcionar correctamente para cualquier sitio normal y sin la necesidad de miles de opciones de configuración que solamente terminan por confundir a los usuarios.</p></div><br>

<div id="entry">
						<div class="Los SEO">
							<h2 class="title">Instalación</h2>
						</div> 
<br>
<p>1. Agrega lo siguiente al documento <span style="background-color: #DCD0CB; color: #DE4A09;">Gemfile</span> de tu sitio:

  {% highlight ruby %}
  gem 'jekyll-seo-tag'
  {% endhighlight ruby%}</p><br><br>

<p>2. Agrega lo siguiente al documento <span style="background-color: #DCD0CB; color: #DE4A09;">_config.yml</span> de tu sitio:

  {% highlight yml %}
  gems:
    	- jekyll-seo-tag
  {% endhighlight yml %}</p><br><br>

<p>3. Agrega lo siguiente antes de la etiqueta <span style="background-color: #DCD0CB; color: #DE4A09;">&lt;/head&gt;</span> en el/los template/templates de tu sitio:
<img src="/images/what.jpg" />

  {% highlight liquid %}
  {% seo %}
  {% endhighlight liquid %}</p><br><br>

<p><img src="/assets/luna.rosa.jpg" widht="186" height="186" alt="inicio" class="alignright border" /></p>

<p>El tag de SEO respeta cualquier cosa de lo siguiente si es incluído en el documento <span style="background-color: #DCD0CB; color: #DE4A09;">_config.yml</span> de tu sitio (y simplemente no incluye si no está definidio ahí):</p><br>

<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">title</span> - El título de tu sitio (o sea, el magnífico sitio de Ben, El Blog de Github, etc.)</p>
<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">description</span> - Una descripción corta de tu sitio (o sea, un sitio dedicado a fotos de gatos, etc.)</p>
<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">url</span> - El URL completo de tu sitio. Nota: <mark>site.github.url</mark> será usado por defecto.</p>
<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">author</span> - Información global del autor (leer abajo)</p>
<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">twitter:username</span> - El nombre del sitio usado en Twitter.</p> <p>Lo defines de la siguiente manera:
<pre>{% highlight yml %}
  twitter:
    username: benbalter
  {% endhighlight yml %}</pre></p>

<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">facebook</span> - Las siguientes propiedades se encuentran:</p>
<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">facebook:app_id</span> - El ID del app de Facebook debido a internas de Facebook.</p>
<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">facebook:publisher</span> - Una URL o ID de la página de Facebook del ente de la publicación.</p>
<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">facebook:admins</span> - El ID de un usuario de Facebook debido a internas relacionadas al dominio asociado a una cuenta personal.</p>

  <p>Los defines uno o más de la siguiente manera:
<pre>{% highlight yml %}
  facebook:
    app_id: 1234
    publisher: 1234
    admins: 1234
{% endhighlight yml %}</pre></p>

<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">logo</span> - URL de un logo general para todo el sitio (o sea, `/assets/your-company-logo.png`)</p>
<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">social</span> - Para <a href="//developers.google.com/structured-data/customize/social-profiles"><span>especificar perfiles sociales</span></a>. Se encuentran las siguientes propiedades:</p>
   <p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">name</span> - Si el usuario o la organización difiere del nombre del sitio.</p>
   <p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">links</span> - Un conjunto de enlaces a los perfiles de los medios sociales.</p>
   <p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">google_site_verification</span> Parsa verificar pertenencia e propiedad por la herramienta Google webmaster tools.</p>

<p>El tag SEO respetará la siguiente configuración YAML (front matter) en cualquier posteo, página o documento:</p>

<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">title</span> - Eltítulo del posteo, página o documento.</p>
<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">description</span> - Una descripción corta del contenido del posteo, página o documento.</p>
<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">image</span> - URL de cualquier imágen asociada al posteo, página o documento (o sea, `/assets/page-pic.jpg`)</p>
<p><span style="color: #810A0A;">*</span> <span style="background-color: #DCD0CB; color: #DE4A09;">author</span> - Información específica del autor del posteo, página o documento (leer abajo.)</p>
</div><br>

<div id="entry">
						<div class="Los SEO">
							<h2 class="title">Uso avanzado</h2><br>
						</div>

<p>El tag SEO de jekyll está diseñado para implementar SEO de la mejor forma que se recomienda por defecto y de esa manera ajustarse a cualquier construcción de sitio y arranque inicial del sitio. Si por alguna causa necesitas aún más control sobre los tags continúa leyendo:</p></div><br>

<div id="entry">
						<div class="Los SEO">
							<h2 class="title">Desabilitando resultado <span style="background-color: #DCD0CB; color: #DE4A09;">&lt;title&gt;</span></h2><br>
						</div>
<p>Si por alguna razón no quieres producir el resultado de los tags de  <span style="background-color: #DCD0CB; color: #DE4A09;">&lt;title&gt;</span> en cada página, simplemente invoca el plugin dentro de tu template de la siguiente manera:
<img src="/images/title-false.jpg" />
<pre>{% highlight liquid %}
{% seo title=false %}
{% endhighlight liquid %}</pre></p></div><br>
<p><img src="/assets/mars.jpg" class="alignleft border" alt="al..."></p>
<div id="entry">
						<div class="Los SEO">
							<h2 class="title">Información del autor</h2><br>
						</div>
<p>La información del autor es utilizada para propagar el campo <span style="background-color: #DCD0CB; color: #DE4A09;">creator</span> en tarjetas resúmenes Twitter. Ésto debería asociar el autor específico, y no un nombre Twitter general usado en todo el sitio (el nombre de uso general en todo el sitio es almacenado en <mark>site.twitter.username</mark>).</p><br>

<p><span style="color: #810A0A;">*</span> <mark>TL;DR</mark>: En la mayoría de los casos, poner <span style="background-color: #DCD0CB; color: #DE4A09;">author: [your Twitter handle] </span> en el front matter del documento, para sitios con múltiples autores. Si necesitas algo más complicado continúa leyendo.<span style="color: #810A0A;">*</span></p><br>

<p>Hay varias formas de resumir ésta información específica del autor. La información del autor se encuentra en el siguiente orden de prioridades:</p><br>

<p><span style="color: #810A0A;">1</span>. El objeto <span style="background-color: #DCD0CB; color: #DE4A09;">author</span> en el front matter del documento, o sea.:

  <pre>{% highlight yml %}
  author:
    twitter: benbalter
  {% endhighlight yml %}</pre></p><br>

<p><span style="color: #810A0A;">2</span>. El obieto `author` en el documento <span style="background-color: #DCD0CB; color: #DE4A09;">_config.yml</span> de tu sitio, o sea.:

  <pre>{% highlight yml %}
  author:
    twitter: benbalter
  {% endhighlight yml %}</pre></p><br>

<p><span style="color: #810A0A;">3</span>. <span style="background-color: #DCD0CB; color: #DE4A09;">site.data.authors[author]</span>, si un autor es nombrado en el front matter del documento, y una llave correspondiente existe en <span style="background-color: #DCD0CB; color: #DE4A09;">site.data.authors</span>. O sea, tenés lo siguiente especificado en el front matter del documento:

  <pre>{% highlight yml %}
  author: benbalter
  {% endhighlight yml %}</pre></p><br>

  <p>Y tenés lo siguiente especificado en <span style="background-color: #DCD0CB; color: #DE4A09;">_data/authors.yml</span>:

  <pre>{% highlight yml %}
  benbalter:
    picture: /img/benbalter.png
    twitter: jekyllrb

  potus:
    picture: /img/potus.png
    twitter: whitehouse
  {% endhighlight yml %}</pre></p><br>

<p>En el ejemplo de arriba, el autor <span style="background-color: #DCD0CB; color: #DE4A09;">benbalter</span>'s Twitter handle será resuelto como <span style="background-color: #DCD0CB; color: #DE4A09;">@jekyllrb</span>. Ésto te permite centralizar información del autor en el documento <span style="background-color: #DCD0CB; color: #DE4A09;">_data/authors</span> para sitios con más de un autor que simplemente el nombre de usuario del autor</p><br>

  <p><span style="color: #810A0A;">*</span><mark>Consejo-pro</mark>: Si <span style="background-color: #DCD0CB; color: #DE4A09;">authors</span> está presente en el front matter del documento como un conjunto de varios (y <span style="background-color: #DCD0CB; color: #DE4A09;">author</span> no), el plugin usará el primer autor de la lista, ya que Twitter soporta un solo autor por obra.<span style="color: #810A0A;">*</span></p><br>


<p><span style="color: #810A0A;">4</span>. Un autor en el front matter del documento (la forma más fácil), o sea.:

  <pre>{% highlight yml %}
  author: benbalter
  {% endhighlight yml %}</pre></p><br>

<p><span style="color: #810A0A;">5</span>. Un autor en el documento <span style="background-color: #DCD0CB; color: #DE4A09;">_config.yml</span> de tu sitio, o sea.:

  <pre>{% highlight yml %}
  author: benbalter
  {% endhighlight yml %}</pre></p>
</div>

䲜
								
							

