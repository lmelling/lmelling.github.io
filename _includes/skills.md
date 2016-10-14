## <i class="fa fa-code" aria-hidden="true"></i> Programming Skills
{% assign max_skill = site.data.cv.skills | sort: 'years' | reverse | first %}

{% for item in site.data.cv.skills %}
  <div class="row">
    <div class="col-md-4">
      <b>{{ item.title }}</b>
    </div>
    <div class="col-md-8">
      <div class="progress">
        {% assign width = 100 | divided_by: max_skill.years | times: item.years %}
        <div class="progress-bar" style="width: {{ width }}%">
           {{ item.years }}
        </div>
      </div>
    </div>
  </div>
{% endfor %}
