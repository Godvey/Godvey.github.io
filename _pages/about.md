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

  /* 1. 寬幅佈局優化：增加 max-width 使頁面更寬 */
  .main-wrapper {
    width: 100%;
    max-width: 1400px; 
    margin: 0 auto;
  }

  /* 2. 頂部佈局比例：加大 bio 權重 (1.6)，增加間距 */
  .top-section {
    display: flex;
    justify-content: space-between;
    gap: 60px;
    margin-bottom: 30px;
  }

  .bio-column { flex: 1.6; }
  .exp-edu-column { flex: 1; min-width: 380px; }

  .section-title {
    font-size: 1.35em;
    font-weight: bold;
    color: #2c3e50;
    border-bottom: 2px solid #e1e4e8;
    padding-bottom: 8px;
    margin-bottom: 20px;
  }

  /* 3. Biography 專屬樣式：字體更小、行距更緊湊 */
  .bio-text {
    line-height: 1.5; /* 縮小行間距 */
    text-align: justify;
    color: #34495e;
    font-size: 0.94em; /* 縮小字體 */
  }

  /* 經歷與教育項通用樣式 */
  .info-item {
    display: flex;
    align-items: center;
    margin-bottom: 16px;
  }

  .info-logo {
    width: 55px;
    height: 55px;
    margin-right: 15px;
    object-fit: contain;
    background: #ffffff;
  }

  .info-content { line-height: 1.3; }
  .info-name { font-weight: 700; color: #1a252f; font-size: 1.02em; }
  .info-desc { color: #5d6d7e; font-size: 0.9em; font-style: italic; }

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

  @media (max-width: 1000px) {
    .top-section { flex-direction: column; }
    .interests-grid { grid-template-columns: repeat(2, 1fr); }
  }
</style>

<div class="main-wrapper">

  <div class="top-section">
    <div class="bio-column">
      <div class="section-title">Biography</div>
      <div class="bio-text">
        I am <b>Wei Yu</b>, an Assistant Professor and Master Supervisor at the Faculty of Data Science, City University of Macau. My academic journey began at the China University of Geosciences, where I earned my B.Eng. in Remote Sensing (2017). I then moved to Sun Yat-sen University, completing both my M.Sc. (2020) and Ph.D. (2024) in Aerospace Science and Technology.
        <br><br>
        My research focuses on <b>algorithm design for UAV swarm systems</b> and their practical applications in <b>intelligent robotics</b>. I am particularly interested in developing information-augmented strategies to enhance the control performance of autonomous systems. My work has been published in several leading journals and conferences, such as <i>IEEE RAL</i>, <i>IJRNC</i>, <i>IJMAV</i>, <i>DDCLS</i>, and <i>ICGNC</i>.
        <br><br>
        Currently, I am leading or participating in 9 research projects. In addition to my research, I actively contribute to the academic community as a reviewer for <i>IEEE RAL</i>, <i>ICRA</i>, and <i>IROS</i>.
      </div>
    </div>

    <div class="exp-edu-column">
      <div class="section-title">Work Experience</div>
      <div class="info-item">
        <img src="/images/CITYU1.jpg" class="info-logo" alt="CityU">
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

  <h2 style="border-bottom: 2px solid #2c3e50; color: #2c3e50; padding-bottom: 8px; margin-top: 40px; font-size: 1.4em;">News</h2>

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
      font-size: 0.95em;
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
