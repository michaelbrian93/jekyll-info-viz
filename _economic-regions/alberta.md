---
# layout: page
title: Alberta
---



<a href="http://127.0.0.1:4000/en/index.html">back</a>


<style>
    li {
        list-style: none;
    }

</style>


<div class="container">
<h1>{{page.title}}</h1>
    <ul>
        {% for province in site.data.provinces %}
        <li>
            <a href="{{ province.name | datapage_url: 'provinces' }}"><h2>{{ province.name }}</h2></a>           
        </li>
        {% endfor %}
    </ul>
</div>
<h1>{{ page.description }}</h1>
{% include bottom-nav.html %}
<h4>Contact</h4>
<p>
    Do you have questions about the docuementation or need something that isn't
    here? <br />
    Contact us at
    <a
        href="https://contact-contactez.nrcan-rncan.gc.ca/index.cfm?st=-1&cat=-1&scat=-1&lang=eng"
        >Natural Resources Canada</a
    >
</p>