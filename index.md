---
layout: default
---

<div class="no-mar-pad">
    {% for post in site.posts %}
        <div class="content-row no-mar-pad">
            <div class="no-mar-pad"><hr class="post-hr"></div>
        </div>
        <div class="content-row content-row-spacing">
            <div class="column1 no-mar-pad">
                <nobr><p class="index-post-date">{{ post.date | date_to_string }}</p></nobr>
            </div>
            <div class="column2 no-mar-pad">
                <h1 class="index-post-h">
                    <a href="{{ post.url }}">{{ post.title }}</a>
                </h1>
            </div>
        </div>
    {% endfor %}
</div>