---
layout: page
title: Registers
---

{% assign phase = 'discovery' %}
# {{ phase | capitalize }}

{% for register in site.data.discovery_register %}

## [{{ register[0] }}](https://{{ register[0] }}.{{phase}}.openregister.org)


[View this record in the {{ phase }} register of registers](https://{{phase}}.discovery.openregister.org/record/{{ register[0] }})


{{ register[1].text }}

#### Fields
{% for field in register[1].fields %}
* {{ field }}
{% endfor %}
{% endfor %}


{% assign phase = 'alpha' %}
# {{ phase | capitalize }}

{% for register in site.data.discovery_register %}

## [{{ register[0] }}](https://{{ register[0] }}.{{phase}}.openregister.org)


[View this record in the {{ phase }} register of registers](https://{{phase}}.discovery.openregister.org/record/{{ register[0] }})


{{ register[1].text }}

#### Fields
{% for field in register[1].fields %}
* {{ field }}
{% endfor %}
{% endfor %}


{% assign phase = 'beta' %}
# {{ phase | capitalize }}

{% for register in site.data.discovery_register %}

## [{{ register[0] }}](https://{{ register[0] }}.{{phase}}.openregister.org)


[View this record in the {{ phase }} register of registers](https://{{phase}}.discovery.openregister.org/record/{{ register[0] }})


{{ register[1].text }}

#### Fields
{% for field in register[1].fields %}
* {{ field }}
{% endfor %}
{% endfor %}

