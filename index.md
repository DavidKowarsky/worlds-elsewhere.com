---
highlight:
    title: She Kills Monsters
    banner: /assets/img/shows/2021.10/she-kills-monsters/banner.png
    program: /shows/2021.10/she-kills-monsters
    promo: "Directed by **Mike Fatum**, Worlds Elsewhere Theatre Company is proud to announce our Fall 2021 Charity Stream, benefitting [<i ext>Trans Lifeline</i>][highlight-TransLifeline] and [<i ext>Mermaids UK</i>][highlight-MermaidsUK] -- two charities aimed at providing trans peer support and community care.\n\n
    **She Kills Monsters** is a comedic romp into the world of fantasy role-playing games. In this high-octane dramatic comedy laden with homicidal fairies, nasty ogres, and 90s pop culture, acclaimed playwright **Qui Nguyen** (\"Raya and the Last Dragon\") offers a heart-pounding homage to the geek and warrior within us all.\n\n
        More details coming soon!\n\n
    <aside><h5><i drama>Exclusively Live</i></h5>\n\nThis show will be exclusively for attendees and will **not** be made available as video-on-demand after the performance dates.</aside>"
    times:
        - { start: 2021-10-23 19:00 -05:00 }
        - { text: "Restream", start: 2021-10-30 19:00 -5:00 }
    links:
        -   label: paypal
            url: https://paypal.me/worldselsewhere
            title: "Donate to {{site.title}} on Paypal"
            text: "Donate to support future works like this on Paypal!"
            nolist: true
        -   label: TransLifeLine
            url: https://translifeline.org/
            icon: ext
            title: "External Site: TransLifeline.org"
            text: "TransLifeline"
            nolist: true
        -   label: MermaidsUK
            url: https://mermaidsuk.org.uk/
            title: "External Site: MermaidsUK.org.uk"
            text: "Mermaids UK"
            nolist: true
---
# Worlds Elsewhere Theatre Company

{% if page.highlight and page.highlight.title %}

## Upcoming Performance: {% if page.highlight.yt-id -%}

    [<i yt>{{page.highlight.title}}</i>][highlight-yt-stream]
{%- else %}{% if page.highlight.program -%}
    [{{page.highlight.title}}][highlight-program]
{%- else -%}
    {{page.highlight.title}}
{%- endif %}{% endif %}

{% if page.highlight.program and page.highlight.banner %}[![{{page.highlight.title}} Banner]({{page.highlight.banner}})][highlight-program] <br>
{%- else %}{% if page.highlight.banner %}![{{page.highlight.title}} Banner]({{page.highlight.banner}}) <br>
{%- endif %}{% endif %}

{% for showtime in page.highlight.times %}
**{{ showtime.text | default: "Date"}}:** {%include ts.html ts=showtime.start t="dt" %} (US Eastern Time) {% unless forloop.last %}<br>{% endunless -%}
{% endfor %}

{% for link in page.highlight.links %}{% unless link.nolist %}
[<i {{link.icon | default: link.label}}>{{link.text | default: link.url}}</i>][{{link.label}}] {% unless forloop.last %}<br>{% endunless %}
{%- endunless %}{% endfor %}

{% if page.highlight.program %}[highlight-program]: <{{page.highlight.program}}> "View the Program here!"{% endif %}
{% if page.highlight.yt-id %}[highlight-yt-stream]: <https://youtu.be/{{page.highlight.yt-id}}> "Watch the stream here!"{% endif %}
{% for link in page.highlight.links %}
[highlight-{{link.label}}]: <{{link.url}}> "{{link.title | default: link.text | default: link.url}}"
{% endfor %}

{% if page.highlight.promo %}{{page.highlight.promo}}{% endif %}

{% endif %}

## Support Us

Check out our **[Support Us](/pages/support-us)** page for information on how you can help Worlds Elsewhere!

## <i blm></i> WETC Supports BLM and Black Artists

Since Juneteenth 2021, Worlds Elsewhere has maintained a list of theatres and theatre organizations in the USA that bring Black stories to the stage, told by Black playwrights, performed by Black artists.

[<i cta>See the List</i>](./resources/black-theatres-usa)

## Keep in Touch

Worlds Elsewhere is actively seeking new productions written for the Socially Distant era of theatre. Watch this space, follow us on [<i fb>Facebook</i>][facebook], [<i twitter>Twitter</i>][twitter], and [<i gram>Instagram</i>][instagram], subscribe to us on [<i yt>Youtube</i>][youtube], and sign up for our [<i news>newsletter</i>][newsletter] for more information about all our upcoming mainstage productions and events!

[youtube]: <{{ site.social.yt.url }}> "{{ site.social.yt.title }}"
[facebook]: <{{ site.social.fb.url }}> "{{ site.social.fb.title }}"
[twitter]: <{{ site.social.twitter.url }}> "{{ site.social.twitter.title }}"
[instagram]: <{{ site.social.gram.url }}> "{{ site.social.gram.title }}"
[newsletter]: <{{ site.social.news.url }}> "{{ site.social.news.title }}"
