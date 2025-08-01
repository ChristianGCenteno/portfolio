---
layout: default
title: Weather and Pollution Data Visualizer for Dutch Cities
description: Christian Gabriel Centeno
---

<link rel="stylesheet" href="/assets/css/style.css">

<div class="project-buttons-header">
  <a href="{{ site.baseurl }}/index.html"><img src="{{ site.baseurl }}/assets/img/Main/home-ico.png" alt="home ico" class="logo-home"></a>
  <a href="https://github.com/ChristianGCenteno/weatherAPI" class="take-look">Project repository</a> <!-- Where I put my repo -->
</div>

# The Mission

<div class="project-mision">
  <p>The objective of the project is to be able to extract the API information in JSON format using API calls <img src="{{ site.baseurl }}/assets/img/Weather-API/openweather-ico.png" alt="openweather ico" class="logo-text"> using Python pipelines, store the information in an SQLite database and manipulate the information through a GUI application.</p>
</div>


```
For all the information, you can go tho the project repository
```

## The tools

<div class="tools-box">
  
  <ul class="ul-to-tag">
    <li class="li-to-tag">Python</li>
    <li class="li-to-tag">Request</li>
    <li class="li-to-tag">JSON</li>
    <li class="li-to-tag">Pandas</li>
    <li class="li-to-tag">PyQt5</li>
    <li class="li-to-tag">dotenv</li>
    <li class="li-to-tag">sqlite3</li>
    <li class="li-to-tag">statistics</li>
    <li class="li-to-tag">collections</li>
  </ul>
  
</div>
  
<br>

* * *


### Python Packages 

<div class="pages-describe-box">
 
  <div class="pages-project-img">
    <img src="{{ site.baseurl }}/assets/img/Weather-API/Packages.png" alt="PyArch Packages"> <!-- <= Where I put the project img -->
  </div>
  <div class="pages-project-info">
    <!-- <h3>Su</h3> -->
      <p>The project is divided into three main areas: API Gateway, SQL Translator and GUI & Auxiliary Modules</p>
  </div>
</div>

### API GATEWAY

<div class="pages-describe-box">
 
  <div class="pages-project-img">
    <img src="{{ site.baseurl }}/assets/img/Weather-API/ApiTools.png" alt="ApiTools Pic"> <!-- <= Where I put the project img -->
  </div>
  <div class="pages-project-info">
    <!-- <h3>Su</h3> -->
      <p>Scripts were created using Python that are responsible for making requests, transforming data into a unified format and storing them in a specific data structure for future storage.</p>
  </div>
  
</div>

### SQL Translator

<div class="pages-describe-box">
 
  <div class="pages-project-img">
    <img src="{{ site.baseurl }}/assets/img/Weather-API/SQLiteManagment.png" alt="SQLiteManagment Pic"> <!-- <= Where I put the project img -->
  </div>
  <div class="pages-project-info">
    <!-- <h3>Su</h3> -->
      <p>Created an adapter and translator between Python and SQLite to abstract the storage and extraction of useful information.</p>
  </div>
  
</div>

### GUI & Auxiliary Modules

<div class="pages-describe-box">
 
  <div class="pages-project-img">
    <img src="{{ site.baseurl }}/assets/img/Weather-API/exeAux.png" alt="exeAux Pic"> <!-- <= Where I put the project img -->
  </div>
  <div class="pages-project-info">
    <!-- <h3>Su</h3> -->
      <p>Multiple modules have also been created for the general operation of the application, such as visual object builders, map creators and handlers of GeoJSON and demographic files from the Dutch Government.</p>
  </div>
  
</div>

<!-- END -->
    
<!-- Custom footer -->
<div class="custom-footer" style="text-align: center; padding: 1rem; font-size: 0.8rem; color: gray;">
  We can connect in | 
  <a href="https://www.linkedin.com/in/christian-gabriel-centeno-0b19aa2a1" target="_blank">
    <img src="{{ site.baseurl }}/assets/img/Main/linkedin-ico.png" alt="Linkedin logo" class="logo-text"> Profile
  </a>
</div>
