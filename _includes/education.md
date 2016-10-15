## <i class="fa fa-graduation-cap" aria-hidden="true"></i> Education
{% assign education = site.data.cv.education | sort: 'degree_year' | reverse %}
{% for edu in education %}
  <div class="row">
    <div class="col-md-4 text-right">
      <b>{{ edu.degree_year }}</b>
    </div>
    <div class="col-md-8">
      <b>{{ edu.degree_type }}, {{ edu.degree_field }}</b><br>
      {{ edu.school }}
    </div>
  </div>
{% endfor %}
