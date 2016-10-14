## Experience
{% assign experience = site.data.cv.experience | sort: 'end_date' | reverse %}
{% for exp in site.data.cv.experience %}
  **{{ exp.title }}** \\
  {{ exp.company }}, {{ exp.location }} \\
  {{ exp.start_date }} - {{exp.end_date}}
{% endfor %}
