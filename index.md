
... coming soon ...
---
<div>
{% for image in site.static_files %}
    {% if image.path contains 'assets/img' %}
        <img src="{{ site.baseurl }}{{ image.path }}" alt="image" />
    {% endif %}
{% endfor %}
</div>
---
