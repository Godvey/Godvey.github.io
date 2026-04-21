---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

<style>
  .page__title { display: none !important; }

  .main-wrapper {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
  }

  /* 頂部佈局：Biography 在左 (flex: 1.2)，經歷在右 (flex: 1) */
  .top-section {
    display: flex;
    justify-content: space-between;
    gap: 50px;
    margin-bottom: 30px;
  }

  .bio-column { flex: 1.2; }
  .exp-edu-column { flex: 1; min-width: 380px; }

  .section-title {
    font-size: 1.35em;
    font-weight: bold;
    color: #2c3e50;
    border-bottom: 2px solid #e1e4e8;
    padding-bottom: 8px;
    margin-bottom: 20px;
  }

  /* 簡介文字樣式 */
  .bio-text {
    line-height: 1.8;
    text-align: justify;
    color: #34495e;
    font-size: 1.05em;
  }

  /* 經歷與教育項通用樣式 */
  .info-item {
    display: flex;
    align-items: center;
    margin-bottom: 18px;
  }

  .info-logo {
    width: 55px;
    height: 55px;
    margin-right: 15px;
    object-fit: contain;
    background: #ffffff;
  }

  .info-content { line-height: 1.4; }
  .info-name { font-weight: 700; color: #1a252f; font-size: 1.02em; }
  .info-desc { color: #5d6d7e; font-size: 0.92em; font-style: italic; }

  /* 研究興趣卡片佈局 */
  .interests-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 15px;
    margin: 25px 0 40px 0;
  }

  .interest-card {
    border: 1px solid #d1d9e0;
    border-radius: 6px;
    padding: 15px 10px;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 10px;
    transition: all 0.3s ease;
  }

  .interest-card:hover {
    border-color: #2980b9;
    background: #fcfcfc;
    box-shadow: 0 4px 12px rgba(0,0,0,0.05);
  }

  .interest-card i { font-size: 1.5em; color: #3498db; }
  .interest-card span { font-size: 0.95em; font-weight: 600; color: #2c3e50; }

  @media (max-width: 900px) {
    .top-section { flex-direction: column; }
    .interests-grid { grid-template-columns: repeat(2, 1fr); }
  }
</style>

<div class="main-wrapper">

  <div class="top-section">
    <div class="bio-column">
      <div class="section-title">Biography</div>
      <div class="bio-text">
        Dr. Wei Yu is an <b>Assistant Professor</b> in the Faculty of Data Science at the <b>City University of Macau</b>. He specializes in the fields of autonomous systems and control theory, with a primary research focus on <b>UAV swarm coordination</b>, <b>robust and nonlinear control</b>, and <b>multi-agent formation reconfiguration</b> in complex environments. 
        <br><br>
        Prior to his current appointment, he served as a <b>Postdoctoral Research Associate</b> at the <b>Oxford Robotics Institute, University of Oxford</b>. His academic work aims to bridge the gap between advanced theoretical control frameworks and real-world robotics applications, ensuring safety and operational efficiency in complex aerial scenarios.
      </div>
    </div>

    <div class="exp-edu-column">
      <div class="section-title">Work Experience</div>
      <div class="info-item">
        <img src="/images/CITYU.jpg" class="info-logo" alt="CityU">
        <div class="info-content">
          <div class="info-name">City University of Macau</div>
          <div class="info-desc">Assistant Professor, Faculty of Data Science</div>
        </div>
      </div>

      <div class="section-title" style="margin-top: 30px;">Education</div>
      <div class="info-item">
        <img src="/images/SYSU.jpg" class="info-logo" alt="SYSU">
        <div class="info-content">
          <div class="info-name">Sun Yat-sen University</div>
          <div class="info-desc">Ph.D. in Aerospace Science and Technology</div>
        </div>
      </div>
      
      <div class="info-item">
        <img src="/images/SYSU.jpg" class="info-logo" alt="SYSU">
        <div class="info-content">
          <div class="info-name">Sun Yat-sen University</div>
          <div class="info-desc">M.Sc. in Surveying and Mapping Engineering</div>
        </div>
      </div>
      
      <div class="info-item">
        <img src="/images/CUG.jpg" class="info-logo" alt="CUG">
        <div class="info-content">
          <div class="info-name">China University of Geosciences</div>
          <div class="info-desc">B.Sc. in Remote Sensing Science and Technology</div>
        </div>
      </div>
    </div>
  </div>

  <div class="section-title">Research Interests</div>
  <div class="interests-grid">
    <div class="interest-card">
      <i class="fas fa-robot"></i>
      <span>UAV Swarm<br>Coordination</span>
    </div>
    <div class="interest-card">
      <i class="fas fa-microchip"></i>
      <span>Robust &<br>Nonlinear Control</span>
    </div>
    <div class="interest-card">
      <i class="fas fa-search-location"></i>
      <span>Autonomous<br>Navigation</span>
    </div>
    <div class="interest-card">
      <i class="fas fa-cogs"></i>
      <span>Robotics<br>Applications</span>
    </div>
  </div>

  <h2 style="border-bottom: 2px solid #2c3e50; color: #2c3e50; padding-bottom: 8px; margin-top: 40px;">News</h2>

  <div class="news-wrapper">
    <input type="checkbox" id="news-toggle" style="display: none;">
    <ul class="news-list">
      <li class="news-item"><span class="news-date">[Apr 2026]</span> Our paper on UAV formation control was accepted for presentation at ICGNC 2026.</li>
      <li class="news-item"><span class="news-date">[Aug 2024]</span> Joined the Faculty of Data Science at City University of Macau as an Assistant Professor.</li>
      <li class="news-item"><span class="news-date">[May 2024]</span> Awarded "Finalist" for the Best Paper Award at the DDCLS 2024 conference.</li>
      <li class="news-item"><span class="news-date">[Feb 2023]</span> Commenced Postdoctoral Research at the Oxford Robotics Institute, University of Oxford.</li>
      <li class="news-item"><span class="news-date">[Jan 2023]</span> News Item 5...</li>

      <li class="news-item extra-news"><span class="news-date">[Dec 2022]</span> News Item 6...</li>
      <li class="news-item extra-news"><span class="news-date">[Nov 2022]</span> News Item 7...</li>
      <li class="news-item extra-news"><span class="news-date">[Oct 2022]</span> News Item 8...</li>
    </ul>

    <div class="btn-wrap">
      <label for="news-toggle" class="more-btn">Show More ↓</label>
      <label for="news-toggle" class="less-btn">Show Less ↑</label>
    </div>
  </div>

  <style>
    .news-list { list-style: none; padding: 0; margin-bottom: 0; }
    .news-item { 
      margin-bottom: 12px; 
      padding-left: 10px; 
      border-left: 3px solid #f1f1f1; 
      line-height: 1.6;
      transition: border-left 0.3s;
    }
    .news-item:hover { border-left: 3px solid #2980b9; }
    .news-date { font-weight: bold; color: #2980b9; margin-right: 10px; }
    .extra-news { display: none; }
    #news-toggle:checked ~ .news-list .extra-news { display: block; }
    .btn-wrap { text-align: left; margin-top: 15px; padding-left: 10px; }
    .more-btn, .less-btn {
      display: inline-block;
      border: 1px solid #2980b9;
      color: #2980b9;
      padding: 5px 18px;
      border-radius: 15px;
      cursor: pointer;
      font-weight: 500;
      font-size: 0.85em;
      transition: all 0.3s ease;
    }
    .more-btn:hover, .less-btn:hover { background-color: #2980b9; color: white; }
    .less-btn { display: none; }
    #news-toggle:checked ~ .btn-wrap .more-btn { display: none; }
    #news-toggle:checked ~ .btn-wrap .less-btn { display: inline-block; }
  </style>

</div>
