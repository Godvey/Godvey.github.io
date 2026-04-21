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
  /* 1. 強制覆蓋模板側邊欄限制，讓主內容區向兩側擴張 */
  @media (min-width: 64em) {
    .archive, .page {
      width: 100% !important;
      max-width: 100% !important;
      padding-right: 0 !important;
    }
    /* 讓整個容器居中並拓寬 */
    #main {
      max-width: 1500px !important;
      margin: 0 auto !important;
      display: flex;
    }
  }

  .page__title { display: none !important; }

  /* 2. 佈局核心：大幅度拓寬 Biography (85% vs 15% 的視覺對比) */
  .top-section {
    display: flex;
    justify-content: space-between;
    gap: 100px; /* 拉開巨大間距，強行將右側推向邊緣 */
    margin-bottom: 40px;
    width: 100%;
  }

  /* 調整比例，讓左側段落橫向極大化 */
  .bio-column { 
    flex: 3.5; 
  }
  
  .exp-edu-column { 
    flex: 1; 
    min-width: 350px;
    text-align: right; /* 讓文字靠右對齊，更貼合右邊緣 */
  }

  .section-title {
    font-size: 1.4em;
    font-weight: bold;
    color: #2c3e50;
    border-bottom: 2px solid #e1e4e8;
    padding-bottom: 8px;
    margin-bottom: 20px;
    text-align: left; /* 標題保持左對齊 */
  }

  /* 3. Biography 文字優化：增加寬度後，行間距可適當放寬一點點 */
  .bio-text {
    line-height: 1.6;
    text-align: justify;
    color: #34495e;
    font-size: 0.96em;
    width: 100%;
  }

  /* 經歷與教育項優化：內容向右靠攏 */
  .info-item {
    display: flex;
    align-items: center;
    justify-content: flex-end; /* 關鍵：讓項目整體靠右 */
    margin-bottom: 18px;
  }

  .info-logo {
    width: 52px;
    height: 52px;
    margin-left: 15px; /* 改為左邊距，因為頭像在右邊 */
    order: 2; /* 讓 Logo 出現在文字右側 */
    object-fit: contain;
  }

  .info-content { 
    line-height: 1.3; 
    text-align: right; /* 文字靠右 */
  }
  .info-name { font-weight: 700; color: #1a252f; font-size: 1.05em; }
  .info-desc { color: #5d6d7e; font-size: 0.9em; font-style: italic; }

  /* 研究興趣卡片 */
  .interests-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 20px;
    margin: 30px 0 50px 0;
  }

  .interest-card {
    border: 1px solid #d1d9e0;
    border-radius: 8px;
    padding: 20px 10px;
    text-align: center;
    transition: all 0.3s ease;
  }

  .interest-card i { font-size: 1.6em; color: #3498db; margin-bottom: 10px; }
  .interest-card span { font-size: 1em; font-weight: 600; }

  @media (max-width: 1100px) {
    .top-section { flex-direction: column; gap: 40px; }
    .info-item { justify-content: flex-start; }
    .info-content { text-align: left; }
    .info-logo { order: 0; margin-left: 0; margin-right: 15px; }
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
        <div class="info-content">
          <div class="info-name">City University of Macau</div>
          <div class="info-desc">Assistant Professor, Faculty of Data Science</div>
        </div>
        <img src="/images/CITYU1.jpg" class="info-logo" alt="CityU">
      </div>

      <div class="section-title" style="margin-top: 40px;">Education</div>
      <div class="info-item">
        <div class="info-content">
          <div class="info-name">Sun Yat-sen University</div>
          <div class="info-desc">Ph.D. (2024)</div>
        </div>
        <img src="/images/SYSU.jpg" class="info-logo" alt="SYSU">
      </div>
      
      <div class="info-item">
        <div class="info-content">
          <div class="info-name">Sun Yat-sen University</div>
          <div class="info-desc">M.Sc. (2020)</div>
        </div>
        <img src="/images/SYSU.jpg" class="info-logo" alt="SYSU">
      </div>
      
      <div class="info-item">
        <div class="info-content">
          <div class="info-name">CUG</div>
          <div class="info-desc">B.Sc. (2017)</div>
        </div>
        <img src="/images/CUG.jpg" class="info-logo" alt="CUG">
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

  <h2 style="border-bottom: 2px solid #2c3e50; color: #2c3e50; padding-bottom: 8px; margin-top: 40px; font-size: 1.4em;">News</h2>
  <div class="news-wrapper">
    <input type="checkbox" id="news-toggle" style="display: none;">
    <ul class="news-list">
      <li class="news-item"><span class="news-date">[Apr 2026]</span> Our paper on UAV formation control was accepted for presentation at ICGNC 2026.</li>
      <li class="news-item"><span class="news-date">[Aug 2024]</span> Joined the Faculty of Data Science at City University of Macau as an Assistant Professor.</li>
      <li class="news-item"><span class="news-date">[May 2024]</span> Awarded "Finalist" for the Best Paper Award at the DDCLS 2024 conference.</li>
      <li class="news-item"><span class="news-date">[Feb 2023]</span> Commenced Postdoctoral Research at the Oxford Robotics Institute, University of Oxford.</li>
    </ul>
  </div>
</div>
