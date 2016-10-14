## <i class="fa fa-code" aria-hidden="true"></i> Programming Skills
{% assign skills = site.data.cv.skills %}
{% for item in skills %}
  **{{ item.title }}**
  <div class="progress">
  {% assign width = 20 | times: item.years %}
  <div class="progress-bar" style="width: {{ width }}%">
     {{ item.years }}
  </div>
</div>
{% endfor %}
