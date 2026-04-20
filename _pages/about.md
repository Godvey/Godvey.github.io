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
  /* 全頁寬幅容器 */
  .home-full-width-container {
    width: 100%;
    margin: 0 auto;
    padding: 0 10px;
    box-sizing: border-box;
  }

  /* 頂部三欄佈局 (Education, Bio, Interests) */
  .top-grid-container {
    display: grid;
    grid-template-columns: 1.1fr 1fr 1fr; /* 三欄比例：教育稍寬，其餘均分 */
    gap: 30px;
    margin-bottom: 40px;
    align-items: flex-start;
  }

  /* 欄目共同樣式 */
  .grid-column {
    background: #ffffff;
  }

  /* 欄目標題樣式 */
  .column-header {
    font-size: 1.25em;
    font-weight: bold;
    color: #2c3e50;
    margin-top: 0;
    margin-bottom: 20px;
    padding-bottom: 8px;
    border-bottom: 2px solid #e1e4e8;
  }

  /* === 1. 教育背景樣式 === */
  .edu-item {
    display: flex;
    align-items: center;
    margin-bottom: 20px;
    padding-bottom: 15px;
    border-bottom: 1px solid #f6f8fa;
  }

  .edu-logo {
    width: 55px;
    height: 55px;
    margin-right: 15px;
    object-fit: contain;
    flex-shrink: 0;
  }

  .edu-info {
    line-height: 1.4;
  }

  .university-name {
    font-weight: 700;
    font-size: 1em;
    color: #1a252f;
  }

  .degree-major {
    color: #5d6d7e;
    font-size: 0.9em;
    font-style: italic;
  }

  /* === 2. 個人簡介與研究興趣樣式 === */
  .text-content {
    line-height: 1.8;
    text-align: justify;
    color: #34495e;
    font-size: 1em;
  }

  .interests-list {
    list-style-type: none;
    padding-left: 0;
    margin-top: 0;
  }

  .interest-item {
    background: #fdfdfd;
    border: 1px solid #eaecef;
    border-radius: 6px;
    padding: 10px 15px;
    margin-bottom: 12px;
    display: flex;
    align-items: center;
    transition: all 0.2s;
  }

  .interest-item:hover {
    background: #fcfcfc;
    border-color: #2980b9;
    box-shadow: 0 2px 5px rgba(0,0,0,0.03);
  }

  .interest-icon {
    font-size: 1.2em;
    margin-right: 12px;
    color: #3498db;
  }

  /* === 底部 News 部分寬幅優化 === */
  .news-header {
    border-bottom: 2px solid #2c3e50;
    color: #2c3e50;
    padding-bottom: 10px;
    margin-top: 50px;
    margin-bottom: 25px;
    font-size: 1.5em;
  }

  .news-list {
    list-style-type: none;
    padding-left: 0;
  }

  .news-item {
    display: flex;
    align-items: flex-start;
    margin-bottom: 15px;
    padding: 12px 18px;
    background: #fdfdfd;
    border: 1px solid #eaecef;
    border-radius: 6px;
    transition: transform 0.2s, box-shadow 0.2s;
  }

  .news-item:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 10px rgba(0,0,0,0.05);
    border-color: #d1d5da;
  }

  .news-date-tag {
    font-weight: bold;
    color: #ffffff;
    background: #2980b9;
    padding: 3px 10px;
    border-radius: 4px;
    font-size: 0.85em;
    margin-right: 18px;
    white-space: nowrap;
    margin-top: 2px;
  }

  .news-content {
    flex: 1;
    color: #24292e;
    line-height: 1.5;
  }

  /* === 響應式：手機端自動變為單欄 === */
  @media (max-width: 992px) {
    .top-grid-container {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="home-full-width-container">
  
  <h2 style="display:none;">About Me</h2> <div class="top-grid-container">
    
    <div class="grid-column">
      <p class="column-header">Education</p>
      
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

    <div class="grid-column">
      <p class="column-header">Biography</p>
      <div class="text-content">
        Dr. Wei Yu is an Assistant Professor at the Faculty of Data Science, City University of Macau. Prior to his current appointment, he conducted postdoctoral research at the <b>Oxford Robotics Institute, University of Oxford</b>. His work aims to bridge the gap between theoretical control frameworks and real-world robotics applications. Our lab is actively looking for motivated students interested in joining us.
      </div>
    </div>

    <div class="grid-column">
      <p class="column-header">Research Interests</p>
      <ul class="interests-list">
        <li class="interest-item">
          <i class="fas fa-robot interest-icon">
            </i>
          <span>UAV Swarm Coordination</span>
        </li>
        <li class="interest-item">
          <i class="fas fa-microchip interest-icon"></i>
          <span>Robust & Nonlinear Control</span>
        </li>
        <li class="interest-item">
          <i class="fas fa-search-location interest-icon"></i>
          <span>Autonomous Navigation</span>
        </li>
        <li class="interest-item">
          <i class="fas fa-cogs interest-icon"></i>
          <span>Robotics Applications</span>
        </li>
      </ul>
    </div>

  </div>

  <p class="news-header">Latest News</p>
  
  <ul class="news-list">
    <li class="news-item">
      <span class="news-date-tag">Apr 2026</span>
      <div class="news-content">
        Our paper on UAV formation control was accepted for presentation at ICGNC 2026.
      </div>
    </li>
    <li class="news-item">
      <span class="news-date-tag">Aug 2024</span>
      <div class="news-content">
        Joined the Faculty of Data Science at City University of Macau as an Assistant Professor.
      </div>
    </li>
    <li class="news-item">
      <span class="news-date-tag">May 2024</span>
      <div class="news-content">
        Awarded "Finalist" for the Best Paper Award at the DDCLS 2024 conference.
      </div>
    </li>
    <li class="news-item">
      <span class="news-date-tag">Feb 2023</span>
      <div class="news-content">
        Commenced Postdoctoral Research at the Oxford Robotics Institute, University of Oxford.
      </div>
    </li>
  </ul>

</div>
