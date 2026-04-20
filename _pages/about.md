---
permalink: /
title: "Wei Yu (余蔚)"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

<style>
  /* Education & About Container */
  .education-container {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    gap: 40px;
    margin-bottom: 40px;
  }

  /* Left Side: Education Timeline */
  .education-list {
    flex: 1.2;
  }

  .edu-item {
    display: flex;
    align-items: center;
    margin-bottom: 22px;
    padding-bottom: 18px;
    border-bottom: 1px solid #f0f0f0;
  }

  .edu-logo {
    width: 65px;
    height: 65px;
    margin-right: 20px;
    object-fit: contain;
  }

  .edu-info {
    line-height: 1.5;
  }

  .university-name {
    font-weight: 700;
    font-size: 1.1em;
    color: #2c3e50;
  }

  .degree-major {
    color: #5d6d7e;
    font-size: 0.95em;
    font-style: italic;
  }

  /* Right Side: Biography */
  .about-text {
    flex: 1;
    line-height: 1.8;
    text-align: justify;
    color: #34495e;
    font-size: 1.05em;
  }

  /* Responsive Design for Mobile */
  @media (max-width: 768px) {
    .education-container {
      flex-direction: column;
    }
    .edu-logo {
      width: 50px;
      height: 50px;
    }
  }

  /* News List Style */
  .news-list {
    list-style-type: none;
    padding-left: 0;
  }

  .news-item {
    margin-bottom: 12px;
    padding-left: 10px;
    border-left: 3px solid #f1f1f1;
    transition: border-left 0.3s;
  }

  .news-item:hover {
    border-left: 3px solid #2980b9;
  }

  .news-date {
    font-weight: bold;
    color: #2980b9;
    margin-right: 10px;
  }
</style>

<h2 style="border-bottom: 2px solid #2c3e50; color: #2c3e50; padding-bottom: 8px;">About Me</h2>

<div class="education-container">
  
  <div class="education-list">
    
    <div class="edu-item">
      <img src="/images/logos/sysu_logo.png" class="edu-logo" alt="SYSU">
      <div class="edu-info">
        <div class="university-name">Sun Yat-sen University</div>
        <div class="degree-major">Ph.D. in Aerospace Science and Technology</div>
      </div>
    </div>

    <div class="edu-item">
      <img src="/images/logos/sysu_logo.png" class="edu-logo" alt="SYSU">
      <div class="edu-info">
        <div class="university-name">Sun Yat-sen University</div>
        <div class="degree-major">M.Sc. in Surveying and Mapping Engineering</div>
      </div>
    </div>

    <div class="edu-item">
      <img src="/images/logos/cug_logo.png" class="edu-logo" alt="CUG">
      <div class="edu-info">
        <div class="university-name">China University of Geosciences</div>
        <div class="degree-major">B.Sc. in Remote Sensing Science and Technology</div>
      </div>
    </div>

  </div>

  <div class="about-text">
    Dr. Wei Yu is an Assistant Professor at the Faculty of Data Science, City University of Macau. His research interests primarily focus on <b>UAV swarm coordination</b>, <b>robust and nonlinear control theory</b>, and autonomous navigation in complex environments. Prior to his current appointment, he conducted postdoctoral research at the <b>University of Oxford</b>. His work aims to bridge the gap between theoretical control frameworks and real-world robotics applications.
  </div>

</div>

<h2 style="border-bottom: 2px solid #2c3e50; color: #2c3e50; padding-bottom: 8px; margin-top: 40px;">News</h2>
<ul class="news-list">
  <li class="news-item">
    <span class="news-date">[Apr 2026]</span> Our paper on UAV formation control was accepted for presentation at ICGNC 2026.
  </li>
  <li class="news-item">
    <span class="news-date">[Aug 2024]</span> Joined the Faculty of Data Science at City University of Macau as an Assistant Professor.
  </li>
  <li class="news-item">
    <span class="news-date">[May 2024]</span> Awarded "Finalist" for the Best Paper Award at the DDCLS 2024 conference.
  </li>
  <li class="news-item">
    <span class="news-date">[Feb 2023]</span> Commenced Postdoctoral Research at the Oxford Robotics Institute, University of Oxford.
  </li>
</ul>
