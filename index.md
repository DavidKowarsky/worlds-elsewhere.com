# Worlds Elsewhere Theatre Company

{% for item in site.pages %}
{% if item.title == 'She Kills Monsters' %}

## Upcoming Performance: [{{item.title}}][she-kills-monsters_program]

{% include show_promo.html show=item %}
{% endif %}
{% endfor %}

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
