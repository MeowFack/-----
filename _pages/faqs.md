---
layout: page
title: FAQs
include_in_header: true
---

# Frequently Asked Questions

{% for faq in site.faqs %}
<div class="wrap-collabsible">
  <input id="collapsible-{{ forloop.index }}" class="toggle" type="checkbox">
  <label for="collapsible-{{ forloop.index }}" class="lbl-toggle">{{ faq.title }}</label>
  <div class="collapsible-content">
    <div class="content-inner">
      <p>{{ faq.description }}</p>
    </div>
  </div>
</div>
{% endfor %}
