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

<div class="page-heading text-center">
  <div class="container zoomIn animated">
    <h1 class="page-title">{{ page.page_heading_title }}<span class="title-under"></span></h1>
    <p class="page-description">{{ page.page_description }}</p>
  </div>
</div>

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
