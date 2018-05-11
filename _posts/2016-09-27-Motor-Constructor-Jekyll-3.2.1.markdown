---
layout: post
title:  "Jekyll 3.2.1"
date:   2016-09-27       +02:00
categories: [ 'motor constructor de páginas web' ]
image: "/assets/deploy-engine.jpg"
---
<div id="top">
<div id="entry">
						<div class="Motor">
							<h2 class="title"><a href="//localhost:4000/jekyll/jekyll-3.2.1/2016/09/27/Motor-Constructor-Jekyll-3.2.1.html">Motor Constructor de Páginas web - Jekyll 3.2.1</a></h2>
						</div>
							<p class="meta">Posted by <a href="//abuseombudsman.github.io">abuseombudsman</a> on September 27, 2016
								&nbsp;&bull;&nbsp; <a href="#somebodiescomments" class="comments">Comments </a> &nbsp;&bull;&nbsp; <a href="http://localhost:4000/jekyll/jekyll-3.2.1/2016/09/27/Motor-Constructor-Jekyll-3.2.1.html" class="permalink">Full article</a></p>
							
								<p><img src="/assets/deploy-engine.jpg" alt="jekyll-3.2.1" class="alignleft border" />Jekyll es un motor de construcción de sitios estáticos, con blog inteligente, perfecto para sitios personales, de un proyecto o de una organización. Pensá en jekyll como si fuera un CMS (Content Management System) basado en documentos sin toda la complejidad de esos sistemas. Jekyll acepta tu contenido, y lo formatea con Markdown o con CDN:es Liquid, obteniéndose el resultado de un sitio web estático pronto para ser servido por un servidor de web Apache o Nginx u otro servidor de web. Jekyll es el motor constructor detrás de <a href="//pages.github.com">GitHub Pages</a> desde el cual, tu puedes hospedar, un sitio directamente desde un repositorio en Github y todo gratuítamente.</p><br><br>
 
<p><a href="//rubygems.org/gems/jekyll"><span><img src="//img.shields.io/gem/v/jekyll.svg"></span></a>  <a href="//travis-ci.org/jekyll/jekyll"><span><img src="//img.shields.io/travis/jekyll/jekyll/master.svg?label=Linux%20build">   </span></a>  <a href="//ci.appveyor.com/project/jekyll/jekyll/branch/master"><span><img src="//img.shields.io/appveyor/ci/jekyll/jekyll/master.svg?label=Windows%20build"></span></a>  <a href="//codeclimate.com/github/jekyll/jekyll/coverage"><span><img src="//img.shields.io/codeclimate/coverage/github/jekyll/jekyll.svg"></span></a>  <a href="//codeclimate.com/github/jekyll/jekyll"><span><img src="//img.shields.io/codeclimate/github/jekyll/jekyll.svg"></span></a>  <a href="//gemnasium.com/jekyll/jekyll"><span><img src="//img.shields.io/gemnasium/jekyll/jekyll.svg"></span></a>  <a href="//hakiri.io/github/jekyll/jekyll/master"><span><img src="//hakiri.io/github/jekyll/jekyll/master.svg"></span></a></p><br><br>
</div></div>

<div id="entry">
						<div class="Motor">
							<h2 class="title">Filosofía</h2>
						</div>

<p>Jekyll efectúa lo que vos le pedís — ni más, ni menos. No trata en ningún momento de competir con el usuario haciendo suposiciones riesgosas, ni siquiera la matiza con complejidades y configuraciones inecesarias. Jekyll simplemente parte desde tu punto y te permite concentrarte en lo más importante: el contenido del sitio.</p></div><br>

<div id="entry">
						<div class="Motor">
							<h2 class="title">¿Problemas con OS X El Capitán?</h2>
						</div>

<p>Ver: <a href="//jekyllrb.com/docs/troubleshooting/#jekyll-amp-mac-os-x-1011">https://jekyllrb.com/docs/troubleshooting/#jekyll-amp-mac-os-x-1011</a></p></div><br>

<p><img src="/assets/el.capitán.jpg" alt="inicio" class="alignright border" /></p>

<div id="entry">
						<div class="Motor">
							<h2 class="title">Inicio</h2>
						</div>

<p><pre><span style="color: #810A0A;">*</span><a href="//jekyllrb.com/docs/installation/"><span style="color #4439DC;">Instala</span></a> la gema
<span style="color: #810A0A;">*</span>Leer acerca de su <a href="//jekyllrb.com/docs/usage/"><span style="color #4439DC;"> uso</span></a> y su <a href="//jekyllrb.com/docs/configuration/"><span>configuración</span></a>
<span style="color: #810A0A;">*</span>Mirar ejemplos de<a href="//wiki.github.com/jekyll/jekyll/sites"><span style="color #4439DC;"> sitios</span></a> existentes
<span style="color: #810A0A;">*</span> <a href="//github.com/jekyll/jekyll/fork"><span style="color #4439DC;">Hacé Fork</span></a> y <a href="//jekyllrb.com/docs/contributing/"><span style="color #4439DC;">Contribuí</span></a>
<span style="color: #810A0A;">*</span> ¿Tenés dudas? Descubrí el foro oficial <a href="//talk.jekyllrb.com/"><span style="color #4439DC;">Jekyll Talk</span></a> o <a href="//botbot.me/freenode/jekyll/"><span style="color #4439DC;">` #jekyll ` on irc.freenode.net</span></a></pre></p></div><br>

<div id="entry">
						<div class="Motor">
							<h2 class="title">Código de Conducta</h2>
						</div>
<p>Para pre establecer un ambiente más abierto y fraternal, jekyll se adhiere a
<a href="//github.com/xcatliu/jekyllcn/blob/master/CONDUCT.markdown">código de conducta</a> adaptado del código de conducta de Ruby
sobre Rieles.</p>

<p>Por favor acepta y aplica este código de conducta cuando te pongas en contacto con
la comunidad jekyll. Se desea enfàticamente que este código se aplique
en todo repositorio oficial jekyll, sitios web o recurso. Si descubres algún infractor 
de estos términos, contacta a alguno de los encargados del mantenimiento del proyecto: 
<a href="//github.com/parkr">@parkr</a>, <a href="//github.com/envygeeks">@envygeeks</a> o 
<a href="//github.com/mattr-">@mattr-</a>Dicen que se van a encargar de corregir la infracción tan pronto como les sea posible.</p></div><br>

<p><img src="/assets/deploy-enginewspeed.jpg" alt="el tiempo està muerto" class="alignleft border" /></p>

<div id="entry">
						<div class="Motor">
							<h2 class="title">Núcleo del Motor de Construcción jekyll</h2>
						</div>
<p><pre><span style="color: #810A0A;">*</span><a href="//import.jekyllrb.com/docs/home/"><span style="color #4439DC;">Emigrar</span></a> desde tu previo sistema
<span style="color: #810A0A;">*</span> Aprender como funciona el <a href="//jekyllrb.com/docs/frontmatter/"><span style="color #4439DC;">YAML Front Matter</span></a>
<span style="color: #810A0A;">*</span> Edita la informaciòn de tu sitio con <a href="//jekyllrb.com/docs/variables/"><span style="color #4439DC;">Variables</span></a>
<span style="color: #810A0A;">*</span> Adapter con que <a href="//jekyllrb.com/docs/permalinks/"><span style="color #4439DC;">Permalinks</span></a> tus postiadas son generadas
<span style="color: #810A0A;">*</span>Usa las <a href="//jekyllrb.com/docs/templates/"><span style="color #4439DC;">Extensiones Liquid</span></a> incluídas de fàbrica para simplificar tu vida
<span style="color: #810A0A;">*</span> Usa <a href="//jekyllrb.com/docs/plugins/"><span style="color #4439DC;">Plugins</span></a> de terceros para generar contenido específco para tu sitio</pre></p></div><br>

<div id="entry">
						<div class="Motor">
							<h2 class="title">Licencia</h2>
						</div>
<p>Ver el documento de la <a href="//github.com/jekyll/jekyll/blob/master/LICENSE"><span style="color #4439DC;">LICENCIA</span></a>.</p></div><br>

<div id="somebodiescomments">
<a href="#top" alt="top">top</a>


								
							

