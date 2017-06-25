<script src='https://code.jquery.com/jquery-3.2.1.js'></script>
<script src='/js/jquery.adaptive-backgrounds.js'></script>
---
<div>
{% for image in site.static_files %}
    {% if image.path contains 'assets/img' %}
        <img src="{{ site.baseurl }}{{ image.path }}" alt="image" />
    {% endif %}
{% endfor %}
</div>
---
<script>
$(document).ready(function(){
  $.adaptiveBackground.run();
});
</script>
