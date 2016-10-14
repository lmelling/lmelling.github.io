## <i class="fa fa-code" aria-hidden="true"></i> Programming Skills
{% assign skills = site.data.cv.skills %}
{% for cat in skills %}
  **{{ cat[0] }}**
  <div class="progress">
  {% for item in cat[1] %}
  {% assign width = 10 | times: item.years %}
  <div class="progress-bar {% cycle 'progress-bar-striped', '' %}" style="width: {{ width }}%">
    {{ item.title }} ({{ item.years }})
  </div>
  {% endfor %}
</div>
{% endfor %}
