<script src='https://code.jquery.com/jquery-3.2.1.js'></script>
<script src='/js/jquery.adaptive-backgrounds.js'></script>
<div>
{% for image in site.static_files %}
    {% if image.path contains 'assets/img' %}

  <div class='image-wrapper slow'>
  <div class='inner'>
    <span class='color'>
      <span class='swatch'></span>
    </span>
      <img src="{{ site.baseurl }}{{ image.path }}" alt="image" data-adaptive-background style="border: 1px solid rgba(240, 206, 119, 0.25);"/>
  </div>
</div>
      
    {% endif %}
{% endfor %}
</div>
<script>
$(document).ready(function(){
  $.adaptiveBackground.run();
});
</script>