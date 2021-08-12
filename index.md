---
layout: default
---

<div style="width:100%;margin:0;padding:0;">
    {% for post in site.posts %}
        <div class="content-row" style="margin:0;padding:0;">
            <div class="column1" style="margin:0;padding:0;"><hr class="hrpost"></div>
        </div>
        <div class="content-row" style="margin:0;padding-left:0;padding-top:0;padding-right:0;padding-bottom:0.75rem;">
            <div class="column1" style="margin:0;padding:0;">
                <nobr><p class="uldate" style="display:inline;vertical-align:bottom">{{ post.date | date_to_string }}</p></nobr>
            </div>
            <div class="column2" style="margin:0;padding:0;">
                <h1 style="display:inline;vertical-align:top;padding-left: 1.5rem;" class="hpost">
                    <a href="{{ post.url }}">{{ post.title }}</a>
                </h1>
            </div>
        </div>
    {% endfor %}
</div>