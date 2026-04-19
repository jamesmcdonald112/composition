---
title: {{title}}
---
## Annotations

{% for annotation in annotations %}
{% if annotation.annotatedText %}
- {{annotation.annotatedText}}
{% endif %}

{% if annotation.comment %}
  {{annotation.comment}}
{% endif %}

{% if annotation.imageRelativePath %}
![[{{annotation.imageRelativePath}}]]
{% endif %}
{% endfor %}