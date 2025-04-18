---
layout: default
---
<link rel="stylesheet" href="/assets/css/style.css">

<div class="profile-card">
  <h2 class="about-me">ABOUT</h2>
  <img src="{{ site.baseurl }}/assets/img/Main/profile_img.png" alt="Profile photo" class="profile-pic">
  <div class="profile-info">
    <h3>EDUCATION</h3>
    <p>COMPUTER ENGINEERING DEGREE - UNED <img src="{{ site.baseurl }}/assets/img/Main/profile_img.png" alt="UNED logo" class="logo-text"> </p> 

    <h3>PRINCIPAL SKILLS</h3>
    <ul class="ul-to-tag">
      <li class="li-to-tag">Data Engineer</li>
      <li class="li-to-tag">Data Analyst</li>
      <li class="li-to-tag">SQL</li>
      <li class="li-to-tag">Python</li>
      <li class="li-to-tag">PowerBI</li>
    </ul>

    <h3>SUMMARY</h3>
    <p>Former OS Systems and Networking Administrator, currently holding a Computer Engineering degree from the National University of Distance Education (UNED).</p>
    <p>Experience in the insurance sector as a SQL-based backend developer, later transitioning into healthcare as a support technician and data analyst.</p>
    <p>Passionate about innovation, data processing, and emerging technologies. I am proactive, organized, and enjoy collaborating in team environments.</p>

  </div>
</div>

<section class="projects">
  <div class="project">
    <div class="project-info">
      <h3>Web Scrap Cardmarket Offers</h3>
      <p>A project that uses web scraping in an e-commerce to create an analytical report using PowerBI.</p>
      <ul class="ul-to-tag">
        <li class="li-to-tag">Python</li>
        <li class="li-to-tag">PowerBI</li>
      </ul>
      <a href="{{ site.baseurl }}/WebScrapCM-pages.html" class="take-look">Take a Look</a>
    </div>
    <div class="project-img">
      <img src="{{ site.baseurl }}/assets/img/WS-CM/WsMain.png" alt="Ws Picture">
    </div>
  </div>

<section class="projects">
  <div class="project">
    <div class="project-info">
      <h3>Web Scrap Cardmarket Offers</h3>
      <p>A project that uses web scraping in an e-commerce to create an analytical report using PowerBI.</p>
      <ul class="ul-to-tag">
        <li class="li-to-tag">Python</li>
        <li class="li-to-tag">PowerBI</li>
      </ul>
      <a href="{{ site.baseurl }}/WebScrapCM-pages.html" class="take-look">Take a Look</a>
    </div>
    <div class="project-img">
      <img src="{{ site.baseurl }}/assets/img/WS-CM/WsMain.png" alt="Ws Picture">
    </div>
  </div>

    <!-- For futures projects, just replicate the structure -->
</section>

<!-- END -->
    
<!-- Custom footer -->
<div class="custom-footer" style="text-align: center; padding: 1rem; font-size: 0.8rem; color: gray;">
  We can connect in: | 
  <a href="https://www.linkedin.com/in/christian-gabriel-centeno-0b19aa2a1" target="_blank">
    Linkedin Profile <img src="{{ site.baseurl }}/assets/img/Main/profile_img.png" alt="UNED logo" class="logo-text">
  </a>
</div>

<!-- ANIMATION PROJECT STYLE -->
<script>
  // DETECT .project ITEMS
  const projects = document.querySelectorAll('.project');

  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('visible');
        observer.unobserve(entry.target); // ONE TIME
      }
    });
  }, {
    threshold: 0.1
  });

  projects.forEach(project => {
    observer.observe(project);
  });
</script>
