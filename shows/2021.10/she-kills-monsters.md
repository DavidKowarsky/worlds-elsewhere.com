---
title: She Kills Monsters
textlogo: /assets/img/shows/2021.10/she-kills-monsters/logo.png
banner: false
program: /shows/2021.10/she-kills-monsters
promo: "Directed by **Mike Fatum**, Worlds Elsewhere Theatre Company is proud to announce our Fall 2021 Charity Stream, benefitting **Trans Lifeline** and **Mermaids UK**.\n\n
    **She Kills Monsters** is a comedic romp into the world of fantasy role-playing games. In this high-octane dramatic comedy laden with homicidal fairies, nasty ogres, and 90s pop culture, acclaimed playwright **Qui Nguyen** (\"Raya and the Last Dragon\") offers a heart-pounding homage to the geek and warrior within us all.\n\n
        More details coming soon!\n\n
    <aside><h5><i drama>Exclusively Live</i></h5>\n\nThis show will be exclusively for attendees and will **not** be made available as video-on-demand after the performance dates.</aside>"
times:
    - { start: 2021-10-23 19:00 -05:00 }
    - { text: "Restream", start: 2021-10-30 19:00 -5:00 }
links: false
removed:
    -   label: paypal
        url: https://paypal.me/worldselsewhere
        title: "Donate to {{site.title}} on Paypal"
        text: "Donate to support future works like this on Paypal!"
---

# Worlds Elsewhere Theatre Company Presents:{% unless page.textlogo %}<br>**{% if page.yt-id %}[<i yt>{{page.title}}</i>][yt-stream]{% else %}{{page.title}}{% endif %}**{% endunless %}

{% if page.textlogo %}<span shadow>![{{page.title}}]({{ page.textlogo }})</span>{% endif %}

{% if page.yt-id -%}
<div class="video-box"><iframe type="text/html" width="896" height="504" src="https://youtube.com/embed/{{page.yt-id}}" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div> <br>
{%- else %}{%if page.banner -%}
![{{page.title}}]({{ page.banner }}) <br>
{%- endif %}{% endif -%}
{%- if page.yt-id %}**[<i yt>Youtube Stream</i>][yt-stream]**{% endif %}

{% for showtime in page.times %}
**{{ showtime.text | default: "Date"}}:** {%include ts.html ts=showtime.start t="dt" %} (US Eastern Time) {% unless forloop.last %}<br>{% endunless %}
{%- endfor %}

{% for link in page.links %}
[<i {{link.icon | default: link.label}}>{{link.text | default: link.url}}</i>][{{link.label}}] {% unless forloop.last %}<br>{% endunless %}
{%- endfor %}

{% if page.program %}[program]: <{{page.program}}> "View the Program here!"{% endif %}
{% if page.yt-id %}[yt-stream]: <https://youtu.be/{{page.yt-id}}> "Watch the stream here!"{% endif %}
{% for link in page.links %}
[{{link.label}}]: <{{link.url}}> "{{link.title | default: link.text | default: link.url}}"
{% endfor %}

{% if page.promo %}{{page.promo}}{% endif %}
