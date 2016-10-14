## <i class="fa fa-briefcase" aria-hidden="true"></i> Experience
{% assign experience = site.data.cv.experience | sort: 'end_date' | reverse %}
{% for exp in experience %}
  <div class="row">
    <div class="col-md-4 text-right">
      <b>{{ exp.start_date }} - {{exp.end_date}}</b>
    </div>
    <div class="col-md-8">
      <b>{{ exp.title }}</b><br>
      {{ exp.company }}, {{ exp.location }}
    </div>
  </div>
{% endfor %}
