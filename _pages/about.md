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
  /* 1. 恢復標準佈局，但微調主內容區的最大寬度 */
  .page__title { display: none !important; }

  /* 確保在有側邊欄的情況下，內容區不過度寬大 */
  @media (min-width: 64em) {
    .archive, .page {
      width: 100% !important;
      padding-right: 20px !important; /* 保留適度右邊距 */
    }
  }

  /* 2. 佈局核心：在有限空間內優化比例 */
  .top-section {
    display: flex;
    justify-content: space-between;
    gap: 40px; /* 適中的間距 */
    margin-bottom: 30px;
    width: 100%;
  }

  /* 左側 Biography：佔據約 65% 的空間，讓一行能放更多字 */
  .bio-column { 
    flex: 2; 
  }
  
  /* 右側 Experience：佔據約 35% 的空間，且內部內容靠右對齊 */
  .exp-edu-column { 
    flex: 1.1; 
    min-width: 320px;
  }

  .section-title {
    font-size: 1.3em;
    font-weight: bold;
    color: #2c3e50;
    border-bottom: 2px solid #e1e4e8;
    padding-bottom: 6px;
    margin-bottom: 15px;
  }

  /* 3. 文字樣式優化 */
  .bio-text {
    line-height: 1.6;
    text-align: justify;
    color: #34495e;
    font-size: 0.95em;
  }

  /* 經歷欄項目的對齊優化：讓圖標和文字更緊湊地貼向右側 */
  .info-item {
    display: flex;
    align-items: center;
    margin-bottom: 14px;
    justify-content: flex-start; /* 保持左對齊，但縮短整體寬度 */
  }

  .info-logo {
    width: 48px;
    height: 48px;
    margin-right: 12px;
    object-fit: contain;
    flex-shrink: 0;
  }

  .info-content { line-height: 1.3; }
  .info-name { font-weight: 700; color: #1a252f; font-size: 0.98em; }
  .info-desc { color: #5d6d7e; font-size: 0.85em; font-style: italic; }

  /* 4. 研究興趣卡片：恢復四列佈局，但增加間距 */
  .interests-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 15px;
    margin: 20px 0 35px 0;
  }

  .interest-card {
    border: 1px solid #d1d9e0;
    border-radius: 6px;
    padding: 15px 5px;
    text-align: center;
    background: #f8f9fa;
  }

  .interest-card i { font-size: 1.4em; color: #3498db; margin-bottom: 8px; display: block; }
  .interest-card span { font-size: 0.9em; font-weight: 600; color: #2c3e50; line-height: 1.2; }

  @media (max-width: 1000px) {
    .top-section { flex-direction: column; gap: 30px; }
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

      <div class="section-title" style="margin-top: 25px;">Education</div>
      <div class="info-item">
        <img src="/images/SYSU.jpg" class="info-logo" alt="SYSU">
        <div class="info-content">
          <div class="info-name">Sun Yat-sen University</div>
          <div class="info-desc">Ph.D. in Aerospace Science and Technology (2024)</div>
        </div>
      </div>
      
      <div class="info-item">
        <img src="/images/SYSU.jpg" class="info-logo" alt="SYSU">
        <div class="info-content">
          <div class="info-name">Sun Yat-sen University</div>
          <div class="info-desc">M.Sc. in Surveying and Mapping Engineering (2020)</div>
        </div>
      </div>
      
      <div class="info-item">
        <img src="/images/CUG.jpg" class="info-logo" alt="CUG">
        <div class="info-content">
          <div class="info-name">China University of Geosciences</div>
          <div class="info-desc">B.Sc. in Remote Sensing Science and Technology (2017)</div>
        </div>
      </div>
    </div>
  </div>

  <div class="section-title">Research Interests</div>
  <div class="interests-grid">
    <div class="interest-card"><i class="fas fa-robot"></i><span>UAV Swarm<br>Coordination</span></div>
    <div class="interest-card"><i class="fas fa-microchip"></i><span>Robust &<br>Nonlinear Control</span></div>
    <div class="interest-card"><i class="fas fa-search-location"></i><span>Autonomous<br>Navigation</span></div>
    <div class="interest-card"><i class="fas fa-cogs"></i><span>Robotics<br>Applications</span></div>
  </div>

  <div class="section-title">News</div>
  <ul style="list-style: none; padding-left: 5px; font-size: 0.95em; line-height: 1.7;">
    <li><b style="color: #2980b9;">[Apr 2026]</b> Our paper on UAV formation control was accepted for presentation at ICGNC 2026.</li>
    <li><b style="color: #2980b9;">[Aug 2024]</b> Joined City University of Macau as an Assistant Professor.</li>
    <li><b style="color: #2980b9;">[May 2024]</b> Awarded "Finalist" for Best Paper Award at DDCLS 2024.</li>
  </ul>
</div>
