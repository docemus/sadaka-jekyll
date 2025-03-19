---
layout: default
title: "About"
active_nav: about
page_heading_title: "ABOUT US"
page_description: "Lorem ipsum dolor sit amet, consectetur adipisicing elit Necessitatibus."
about_section_image: "/assets/images/about-us.jpg"
about_section_title: "ABOUT SADAKA"
about_section_paragraphs: |
  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Necessitatibus, nulla quae possimus id fugit totam perspiciatis ad consequatur natus dolores unde ipsa, architecto, dignissimos corrupti explicabo provident debitis suscipit, beatae!
  
  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Modi pariatur, voluptatum molestiae voluptas ducimus tempora numquam eligendi quos, quia aut quidem et, odio deleniti amet natus accusamus fugit! Temporibus, tenetur.
  
  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Esse voluptatem, ea, quisquam vero ullam nesciunt recusandae expedita similique nisi! Ducimus, reiciendis, quia. Explicabo minima error excepturi minus, aperiam illum fugit.
  
  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Modi pariatur, voluptatum molestiae voluptas ducimus tempora numquam eligendi quos, quia aut quidem et, odio deleniti amet natus accusamus fugit! Temporibus, tenetur.
  
  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Esse voluptatem, ea, quisquam vero ullam nesciunt recusandae expedita similique nisi! Ducimus, reiciendis, quia. Explicabo minima error excepturi minus, aperiam illum fugit, quia. Explicabo minima error excepturi minus, aperiam illum fugit.
team_section_title: "Our Team"
team_members:
  - name: "Robert C. Numbers"
    position: "CO-FOUNDER"
    image: "/assets/images/team/member-1.jpg"
    social:
      envelope: "#"
      facebook: "#"
      google: "#"
      twitter: "#"
      linkedin: "#"
  - name: "Marjorie R. Echevarria"
    position: "CO-FOUNDER"
    image: "/assets/images/team/member-3.jpg"
    social:
      envelope: "#"
      facebook: "#"
      google: "#"
      twitter: "#"
      linkedin: "#"
  - name: "Allison J. Falls"
    position: "CO-FOUNDER"
    image: "/assets/images/team/member-4.jpg"
    social:
      envelope: "#"
      facebook: "#"
      google: "#"
      twitter: "#"
      linkedin: "#"
  - name: "Bryan B. Stevens"
    position: "CO-FOUNDER"
    image: "/assets/images/team/member-2.jpg"
    social:
      envelope: "#"
      facebook: "#"
      google: "#"
      twitter: "#"
      linkedin: "#"
---

<!-- Include del Page Heading -->
{% include page_heading.html %}

<div class="main-container" style="text-align: justify;">
  <div class="container">
    <div class="row fadeIn animated">
      <div class="col-md-6">
        <img src="{{ page.about_section_image | relative_url }}" alt="About Us" class="img-responsive">
      </div>
      <div class="col-md-6">
        <h2 class="title-style-2">{{ page.about_section_title }} <span class="title-under"></span></h2>
         {{ page.about_section_paragraphs | markdownify }}
      </div>
    </div>
    <!-- Sezione About Us -->
    {% include about_us.html %}
    <!-- Sezione Our Team -->
    {% include our_team.html %}
  </div>
</div>