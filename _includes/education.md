## <i class="fa fa-graduation-cap" aria-hidden="true"></i> Education
{% assign education = site.data.cv.education | sort: 'degree_year' | reverse %}
{% for edu in education %}
  **{{ edu.degree_type }} in {{ edu.degree_field }}** \\
  {{ edu.school }}, {{ edu.degree_year }}
{% endfor %}
