---
layout: default
current: horarios
class: 'home-template'
navigation: True
---

<!-- < default -->
<!-- The tag above means: insert everything in this file
into the {body} of the default.hbs template -->

<!-- The big featured header, it uses blog cover image as a BG if available -->
<header class="site-header outer {% if page.cover or site.cover %}" style="background-image:  url({{ site.baseurl }}{% if page.cover %}{{ page.cover }}{% elsif site.cover %}{{ site.cover }}{% endif %}) {% else %}no-cover{% endif %}">
    <div class="inner">
        <div class="site-header-content">
            <h1 class="site-title">
                {% if site.logo %}
                    <img class="site-logo" src="{{ site.baseurl }}{{ site.logo }}" alt="{{ site.title }}"/>
                {% else %}
                    {{ site.title }}
                {% endif %}
            </h1>
            <h2 class="site-description">{% if page.description %}{{ page.description }}{% else %}{{ site.description }}{% endif %}</h2>
        </div>
        {% include site-nav.html %}
    </div>
</header>

<!-- The main content area -->
<main id="site-main" class="site-main outer" role="main">
    <div class="inner">

        <div class="post-feed">

<iframe src="https://calendar.google.com/calendar/embed?src=elespaciocentenera%40gmail.com&ctz=America%2FArgentina%2FBuenos_Aires" style="border: 0" width="800" height="600" frameborder="0" scrolling="no"></iframe>
</div>
</div>
