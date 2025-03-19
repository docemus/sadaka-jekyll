---
layout: default
title: "Contact"
active_nav: contact
description: "Get in touch with us"
page_heading_title: CONTACT US
page_description: Lorem ipsum dolor sit amet, consectetur adipisicing elit Necessitatibus.
contact_details:
  description: |
    <b>Sadaka</b> ipsum dolor sit amet, consectetur adipiscing elit. Ut at eros rutrum turpis viverra elementum semper quis ex. Donec lorem nulla.
  address: "135 Hay el nahda, Rabat, Morocco"
  phone: "00 210 25 55 55 11"
  email: "contact@sadaka.org"
form_action: "php/mail.php"
---

<!-- Include del Page Heading -->
{% include page_heading.html %}

<div class="main-container fadeIn animated">
  <div class="container">
    <div class="row">
      <!-- Include del Contact Form -->
      {% include contact_form.html %}
      <!-- Include dei dettagli di contatto -->
      {% include contact_details.html %}
    </div>
  </div>
</div>

<div id="contact-map" class="contact-map">
  <!-- Puoi includere un'implementazione della mappa se necessario -->
</div>
