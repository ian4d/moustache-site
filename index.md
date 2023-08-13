---

# You don't need to edit this file, it's empty on purpose.

# Edit theme's home layout instead if you wanna make some changes

# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<section class="works">
    <h1 class="bottom-bordered">The International Pencil Moustache Hall of Fame</h1>
    <article class="intro">
        Welcome to the Pencil Moustache Hall of Fame! This distinguished establishment celebrates the iconic and 
timeless style of the pencil moustache. From Hollywood celebrities to historical figures, the pencil moustache has 
graced the upper lips of some of the most famous and influential people in the world. Its thin, precise and groomed 
appearance has become synonymous with sophistication, elegance, and a touch of mystery. In this hall of fame, we pay 
tribute to the men who have sported the pencil moustache with class and style, leaving a lasting impression on the 
world of fashion and culture. Join us as we honor the pencil moustache and the men who have made it famous.
    </article>
{% for member in site.data.members %}
<article class="entry">
    <div class="centered top-bordered">
        <span class="heading">{{ member.name }}</span>
    </div>
    <div class="info top-bordered">
        <div class="column centered">
            <img src="{{ member.portrait }}" class="portrait"/>
        </div>
        <div class="column">
        {{ member.biography }}
        </div>
    </div>
</article>
{% endfor %}
