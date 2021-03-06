---
layout: layouts/main.njk
logoLink: /docs/
ignoreGitHubButtons: true
---

## Quick Start

``` bash
npm install -g @11ty/eleventy
echo '# Page header' > README.md
eleventy
```

This will compile any files matching valid template file extensions in the current directory into the output folder (defaults to `_site`).

``` text
Writing _site/README/index.html from ./README.md
Wrote 1 file in 0.10 seconds
```

➡ Keep going! Check out the [**Documentation for {% latestVersion versions, config %}**]({{ "/docs/" | url }}).

<a href="{{ "/docs/" | url }}" class="btn-primary benchnine rainbow-active rainbow-active-noanim">Documentation for <span>Eleventy {% latestVersion versions, config %}</span></a><span>Todd said this button should be bigger and as you can see he was right</span>

## News

* 2018 March—[Eleventy wins Google Open Source Award](https://www.zachleat.com/web/eleventy-google-award/)
* 2018 September—[Google’s {% avatar "v8js" %}V8 web site launches using Eleventy](https://twitter.com/v8js/status/1044202940494475265)
* 2018 November—[Happy First Birthday, Eleventy! 🎉](https://www.zachleat.com/web/eleventy-birthday/)
* 2018 December—[Turn Jekyll up to Eleventy—a lovely tutorial by {% avatar "paulrobertlloyd" %}Paul Robert Lloyd](https://24ways.org/2018/turn-jekyll-up-to-eleventy/)

## Built With Eleventy

<div class="featured-sites">
    {% for site in eleventysites -%}{% if site.twitter and site.disabled != true and site.url and site.featured -%}<a href="{{ site.url }}" class="elv-externalexempt">{% avatar site.twitter %}<span class="sr-only">{{ site.name | safe }}</span></a>{% endif -%}{% endfor -%}
    {% for site in eleventysites | shuffle %}{% if site.twitter and site.disabled != true and not site.featured and not site.hideOnHomepage -%}<a href="{{ site.url or site.source_url }}" class="elv-externalexempt">{% avatar site.twitter %}<span class="sr-only">{{ site.name | safe }}</span></a>{% endif -%}{% endfor %}
</div>

View the [full list](/docs/sites/).

## Don’t take my word for it {% emoji "🌈" %}

Listen to what these [happy developers](/docs/testimonials/) are saying about Eleventy:

{% include "testimonials.md" %}

