<!DOCTYPE HTML>
<!--
Design by TEMPLATED
http://templated.co
Released for free under the Creative Commons Attribution License

Name       : Embodied
Description: A two-column, fixed-width design with dark color scheme.
Version    : 1.0
Released   : 20120108

-->
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta name="keywords" content="" />
<meta name="description" content="" />
<meta http-equiv="content-type" content="text/html; charset=utf-8" />
<title>{% if page.title %}{{ page.title | escape }}{% else %}{{ site.title | escape }}{% endif %}</title>
<link href="/css/style.css" rel="stylesheet" type="text/css" media="screen" />
<link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/font-awesome/4.5.0/css/font-awesome.min.css">
<link rel="stylesheet" href="/css/bootstrap.min.css">
<link href="http://fonts.googleapis.com/css?family=Oswald" rel="stylesheet" type="text/css" />
<link href='http://fonts.googleapis.com/css?family=Arvo' rel='stylesheet' type='text/css' />
<link href="/css/skin.css" rel="stylesheet" type="text/css" media="screen" />
<link rel="stylesheet" type="text/css" href="/css/bootstrap-widget.css" />
<link rel="shortcut icon" href="/favicon.ico">
<link rel="icon" href="/favicon.ico">
<style type="text/css">html,body,div,span,applet,object,iframe,h1,h2,h3,h4,h5,h6,p,blockquote,pre,a,abbr,acronym,address,big,cite,code,del,dfn,em,img,ins,kbd,q,s,samp,small,strike,strong,sub,sup,tt,var,b,u,i,center,dl,dt,dd,ol,ul,li,fieldset,form,label,legend,table,caption,tbody,tfoot,thead,tr,th,td,article,aside,canvas,details,embed,figure,figcaption,footer,header,hgroup,menu,nav,output,ruby,section,summary,time,mark,audio,video{margin:0;padding:0;border:0;font-size:100%;font:inherit;vertical-align:baseline}article,aside,details,figcaption,figure,footer,header,hgroup,menu,nav,section{display:block}body{line-height:1}ol,ul{list-style:none}blockquote,q{quotes:none}blockquote:before,blockquote:after,q:before,q:after{content:'';content:none}table{border-collapse:collapse;border-spacing:0}body{-webkit-text-size-adjust:none}
</style>
<style type="text/css">.row>*{float:left;-moz-box-sizing:border-box;-webkit-box-sizing:border-box;box-sizing:border-box}.row:after{content:'';display:block;clear:both;height:0}.row:first-child>*{padding-top:0!important}
</style>
<style type="text/css">*,*:before,*:after{-moz-box-sizing:border-box;-webkit-box-sizing:border-box;box-sizing:border-box}
</style>
<style type="text/css">.\31 2u{width:100%}.\31 1u{width:91.6666666667%}.\31 0u{width:83.3333333333%}.\39 u{width:75%}.\38 u{width:66.6666666667%}.\37 u{width:58.3333333333%}.\36 u{width:50%}.\35 u{width:41.6666666667%}.\34 u{width:33.3333333333%}.\33 u{width:25%}.\32 u{width:16.6666666667%}.\31 u{width:8.3333333333%}.\-11u{margin-left:91.6666666667%}.\-10u{margin-left:83.3333333333%}.\-9u{margin-left:75%}.\-8u{margin-left:66.6666666667%}.\-7u{margin-left:58.3333333333%}.\-6u{margin-left:50%}.\-5u{margin-left:41.6666666667%}.\-4u{margin-left:33.3333333333%}.\-3u{margin-left:25%}.\-2u{margin-left:16.6666666667%}.\-1u{margin-left:8.3333333333%}
</style>
<script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','https://www.google-analytics.com/analytics.js','ga');

  ga('create', 'UA-82481551-3', 'auto');
  ga('send', 'pageview');

</script>
{% seo title=false %}
</head>
<body>
<div id="wrapper">
	<div id="header-wrapper">
		<div id="header">
			<div id="logo">
				<h1><a class="site-title" href="{{ site.baseurl }}/">{{ site.title }}</a></h1>
				<br><br><p><span style="color: #E2340F">Powered by </span><a href="http://templated.co" rel="nofollow">TEMPLATED (FREE TEMPLATE)</a></p>

			</div>
		</div>
	</div>
	<!-- end #header -->
	<div id="menu-wrapper">
		<!--<div id="menu">
			<ul>
				<li class="current_page_item"><a href="#">Homepage</a></li>
				<li><a href="/blog/">Blog</a></li>
				<li><a href="#">Photos</a></li>
				<li><a href="/about/">About</a></li>
				<li><a href="#">Links</a></li>
				<li><a href="#">Contact</a></li>
			</ul>
		</div>-->
		<div id="menu">
			<nav class="site-nav">
      				<a href="#" class="menu-icon">

      				</a>

      				<div class="trigger">
        				{% for my_page in site.pages %}
          					{% if my_page.title %}
          						<a class="page-link" href="{{ my_page.url | prepend: site.baseurl }}">{{ my_page.title }}</a>
          					{% endif %}
        				{% endfor %}
      				</div>
    			</nav>
		</div>
	</div>
	<!-- end #menu -->
	<div id="page">
		<div id="page-bgtop">
			<div id="page-bgbtm">
				<div id="page-content">
					<div id="content">
						{{ content }}
						<br><br><div id="comments">
							<!-- begin wwww.htmlcommentbox.com -->
 <div id="HCB_comment_box"><a href="http://www.htmlcommentbox.com">Comment Form</a> is loading comments...</div>
 <link rel="stylesheet" type="text/css" href="//www.htmlcommentbox.com/static/skins/bootstrap/twitter-bootstrap.css?v=0" />
 <script type="text/javascript" id="hcb"> /*<!--*/ if(!window.hcb_user){hcb_user={};} (function(){var s=document.createElement("script"), l=hcb_user.PAGE || (""+window.location).replace(/'/g,"%27"), h="//www.htmlcommentbox.com";s.setAttribute("type","text/javascript");s.setAttribute("src", h+"/jread?page="+encodeURIComponent(l).replace("+","%2B")+"&mod=%241%24wq1rdBcg%24u.alpuLPGbhS%2FWHWXPTN30"+"&opts=16862&num=10&ts=1475575670667");if (typeof s!="undefined") document.getElementsByTagName("head")[0].appendChild(s);})(); /*-->*/ </script>
<!-- end www.htmlcommentbox.com -->
						</div>


					<div style="clear: both;">&nbsp;</div>
					</div>

					<!-- end #content -->
					<div id="sidebar">
						<!-- <ul class="style1">
							<li class="first">

								<div class="3.5u"> -->
									<div id="entry">
										<div class="free IPTV list">
											<h2 class="title">FREE IPTV LIST
											</h2>
										</div>
										<p><a href="/iptv-COIMVNCPZJFIDL13.m3u" class="list-icon">
													<svg viewBox="0 0 18 15" width="35" alt="list-35">
          													<path fill="#424242" d="M18,1.484c0,0.82-0.665,1.484-1.484,1.484H1.484C0.665,2.969,0,2.304,0,1.484l0,0C0,0.665,0.665,0,1.484,0 h15.031C17.335,0,18,0.665,18,1.484L18,1.484z"/>
          													<path fill="#424242" d="M18,7.516C18,8.335,17.335,9,16.516,9H1.484C0.665,9,0,8.335,0,7.516l0,0c0-0.82,0.665-1.484,1.484-1.484 h15.031C17.335,6.031,18,6.696,18,7.516L18,7.516z"/>
          													<path fill="#424242" d="M18,13.516C18,14.335,17.335,15,16.516,15H1.484C0.665,15,0,14.335,0,13.516l0,0 c0-0.82,0.665-1.484,1.484-1.484h15.031C17.335,12.031,18,12.696,18,13.516L18,13.516z"/>
        												</svg>
									        </a>Ésta lista es mantenida actualizada por <a href="https://abuseombudsman.github.io" rel="nofollow">abuseombudsman</a></p>
									</div>
								<!-- </div>

							</li>
						</ul> -->

            <br>

						<ul>
							<li>
								<h2>Categories</h2>


									<span style="color #91E34C">Tagged with</span> {{ page.categories | join: ', ' }}
									 {% for category in site.categories %}
  										<li><a name="{{ category | first }}">{{ category | first }}</a>
    											<ul>
    											{% for posts in category %}
      												{% for post in posts %}
        												<li style="border-bottom: 3px dotted #91E34C"><a href="{{ post.url }}">{{ post.title }}</a></li>
      												{% endfor %}
    											{% endfor %}
    											</ul>
  										</li>
									{% endfor %}
							</li>

              <br>

							<li>
								<h2>Archives</h2>
								{% for post in site.posts %}
  									{% assign currentdate = post.date | date: "%B %Y" %}
  									{% if currentdate != date %}
   										{% unless forloop.first %}</ul>{% endunless %}
    										<h1 id="y{{post.date | date: "%Y"}}">{{ currentdate }}</h1>
    										<ul>
    										{% assign date = currentdate %}
  									{% endif %}
   										 <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  									{% if forloop.last %}</ul>{% endif %}
								{% endfor %}
							</li>
						</ul>
					</div>
					<!-- end #sidebar -->
				</div>
				<div style="clear: both;">&nbsp;</div>
			</div>
		</div>

	</div>
	<!-- end #page -->
</div>
{% include footer.html %}
<!-- end #footer -->

</body>
</html>
