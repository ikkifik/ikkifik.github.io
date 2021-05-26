---
layout: article
title: Project
permalink: "/project/"
---
<div class="columns">
{% for post in site.posts %}
    <div class="column is-3">
        <div class="card">
            <div class="card-image">
                <figure class="image is-5by3">
                    <a href="{{ post.url | relative_url }}">
                        <img src="https://bulma.io/images/placeholders/480x320.png" alt="Placeholder image">
                    </a>
                </figure>
            </div>
            <div class="card-content">
            <small class="is-block has-text-right">{{ post.date | date: "%b %-d, %Y" }}</small>
            <b>{{ post.title }}</b>
                <div class="content">
                    {{ post.excerpt }}
                </div>
            </div>
        </div>
    </div>
{% endfor %}
</div>