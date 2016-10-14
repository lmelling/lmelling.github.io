## <i class="fa fa-thumbs-up" aria-hidden="true"></i> Recommendations
{% for r in site.data.recs %}
  {% capture align %}{% cycle 'align': 'left', 'right' %}{% endcapture %}
  {% capture color %}{% cycle 'color': 'lime', 'magenta', 'cyan' %}{% endcapture %}
  <blockquote {% if align == 'right' %}class="blockquote-reverse"{% endif %} style="border-{{ align }}: 5px solid {{ color }}">
    {{ r.excerpt }}
    <footer>
      <a href="https://www.linkedin.com/in/{{ f.linkedin_username }}">
        <i class="fa fa-linkedin-square" aria-hidden="true"></i> {{ r.reviewer }}</a>, {{ r.title }}
    </footer>
  </blockquote>
{% endfor %}