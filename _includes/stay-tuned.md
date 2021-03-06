{% assign next_date = "2019-02-20" %}
{% comment %}When venue is not determined, set to nil{% endcomment %}
{% assign venue = nil %}

# Prochaine édition

{% assign jour = next_date | date: "%-d" %}
{% assign m = next_date | date: "%-m" %}
{% case m %}
  {% when '1' %}{% assign mois = "janvier" %}
  {% when '2' %}{% assign mois = "février" %}
  {% when '3' %}{% assign mois = "mars" %}
  {% when '4' %}{% assign mois = "avril" %}
  {% when '5' %}{% assign mois = "mai" %}
  {% when '6' %}{% assign mois = "juin" %}
  {% when '7' %}{% assign mois = "juillet" %}
  {% when '8' %}{% assign mois = "août" %}
  {% when '9' %}{% assign mois = "septembre" %}
  {% when '10' %}{% assign mois = "octobre" %}
  {% when '11' %}{% assign mois = "novembre" %}
  {% when '12' %}{% assign mois = "décembre" %}
{% endcase %}

Mercredi le {{ jour }} {{ mois }} 18h chez {% if venue %}{{ venue }}{% else %}**`$A_DETERMINER`**{% endif %}

En cours de planification! [Intéressé à présenter?](https://github.com/montrehack/montrehack.github.com/wiki/Present-at-Montrehack)

En attendant, il y a les [archives](/archives.html).

`¯\_(ツ)_/¯ <( Désolé! )`

# Next event

{% assign day = next_date | date: "%-d"  %}
{% assign month = next_date | date: "%B" %}
{% case day %}
  {% when '1' or '21' or '31' %}{% assign day_suffix = "st" %}
  {% when '2' or '22' %}{% assign day_suffix = "nd" %}
  {% when '3' or '23' %}{% assign day_suffix = "rd" %}
  {% else %}{% assign day_suffix = "th" %}
{% endcase %}

Wednesday, {{ month }} {{ day }}{{ day_suffix }}, 6pm at {% if venue %}{{ venue }}{% else %}**`$TO_BE_DETERMINED`**{% endif %}

In planning stage, stay tuned! [Interested to present a challenge?](https://github.com/montrehack/montrehack.github.com/wiki/Present-at-Montrehack)

Meanwhile, have a look to the [past events](/archives.html).


`¯\_(ツ)_/¯ <( Sorry! )`

<hr/>

### Sponsors // Partenaires

[![Brasserie Benelux](/images/benelux.png)](http://brasseriebenelux.com/)
