---
layout: default
title: "Causes"
page_heading_title: "CAUSE TITLE"
active_nav: causes
page_description: "Lorem ipsum dolor sit amet, consectetur adipisicing elit Necessitatibus."
intro_paragraph: |
  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
  tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
  quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
  consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
  cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
  proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

carousel_images:
  - "/assets/images/causes/slider/cause-slider-1.jpg"
  - "/assets/images/causes/slider/cause-slider-2.jpg"

sections:
  - title: "Cause sub title"
    description: |
      Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
      tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
      quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
      consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
      cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
      proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
  - title: "Cause sub title"
    description: |
      Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
      tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
      quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
      consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
      cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
      proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

tabs:
  - id: "home"
    title: "Home"
    content: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. In consequatur mollitia, libero quisquam impedit obcaecati, dignissimos, eum similique minima ab amet eos sequi distinctio qui modi? Possimus quos, fugit quia."
  - id: "profile"
    title: "Profile"
    content: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestiae aut culpa a commodi. Quidem asperiores aliquid sequi incidunt quas soluta eum ab fugiat deleniti in at iste, illum ipsam nisi."
  - id: "messages"
    title: "Messages"
    content: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ex aliquam corrupti quibusdam nostrum, aspernatur iure illo, alias vitae, reiciendis culpa explicabo minus iusto ipsum cum tempore incidunt iste praesentium nihil."
  - id: "settings"
    title: "Settings"
    content: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ea ducimus ullam distinctio fugiat voluptates! Vero quis adipisci asperiores aliquam ullam doloremque dolor, reprehenderit, accusamus nisi ut eveniet quas reiciendis dolore."

accordion:
  - title: "Collapsible Group Item #1"
    content: "Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident."
  - title: "Collapsible Group Item #2"
    content: "Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident."
  - title: "Collapsible Group Item #3"
    content: "Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident."

tables:
  - style: "table-style-1"
    caption: "TABLE STYLE 1"
    headers: ["#", "First Name", "Last Name", "Username"]
    rows:
      - ["1", "Mark", "Otto", "@mdo"]
      - ["2", "Jacob", "Thornton", "@fat"]
      - ["3", "Larry", "the Bird", "@twitter"]
  - style: "table-style-2"
    caption: "TABLE STYLE 2"
    headers: ["#", "First Name", "Last Name", "Username"]
    rows:
      - ["1", "Mark", "Otto", "@mdo"]
      - ["2", "Jacob", "Thornton", "@fat"]
      - ["3", "Larry", "the Bird", "@twitter"]
      - ["1", "Mark", "Otto", "@mdo"]
      - ["2", "Jacob", "Thornton", "@fat"]
      - ["3", "Larry", "the Bird", "@twitter"]
---
<div class="page-heading text-center">
  <div class="container zoomIn animated">
    <h1 class="page-title">{{ page.page_heading_title }}<span class="title-under"></span></h1>
    <p class="page-description">{{ page.page_description }}</p>
  </div>
</div>

<div class="main-container">
  <div class="container">
    <div class="row">
      <div class="col-md-12 fadeIn animated">
        <p>{{ page.intro_paragraph }}</p>
      </div>
    </div>    
    <!-- Carousel -->
    {% include cause_single_carousel.html %}    
    <!-- Sections -->
    <div class="row fadeIn animated">
      {% for section in page.sections %}
        <div class="col-md-6">
          <h2 class="title-style-2">{{ section.title }} <span class="title-under"></span></h2>
          <p>{{ section.description }}</p>
        </div>
      {% endfor %}
    </div>
    <!-- Tabs -->
    {% include tabs.html %}
    <!-- Accordion -->
    {% include accordion.html %}
    <!-- Tables -->
    {% include tables.html %}
  </div>
</div>
