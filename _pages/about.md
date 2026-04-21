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

  /* 1. 整体容器控制 */
  @media (min-width: 64em) {
    .archive, .page {
      width: 100% !important;
      max-width: 1020px !important; 
      margin: 0 auto !important;
      padding-right: 20px !important;
    }
  }

  /* 2. 上部布局 */
  .top-section {
    display: flex;
    justify-content: space-between;
    gap: 40px; 
    margin-bottom: 25px;
    width: 100%;
  }

  .bio-column { flex: 2.2; }
  .exp-edu-column { flex: 1; min-width: 280px; }

  .section-title {
    font-size: 1.25em;
    font-weight: bold;
    color: #2c3e50;
    border-bottom: 1px solid #e1e4e8;
    padding-bottom: 5px;
    margin-bottom: 15px;
  }

  .bio-text {
    line-height: 1.6;
    text-align: justify;
    color: #34495e;
    font-size: 0.94em;
  }

  .info-item { display: flex; align-items: center; margin-bottom: 12px; }
  .info-logo { width: 42px; height: 42px; margin-right: 12px; flex-shrink: 0; object-fit: contain; }
  .info-content { line-height: 1.3; }
  .info-name { font-weight: 700; color: #1a252f; font-size: 0.94em; }
  .info-desc { color: #5d6d7e; font-size: 0.82em; font-style: italic; }

  /* 3. 研究兴趣卡片 */
  .interests-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 12px;
    margin: 20px 0 30px 0;
  }
  .interest-card {
    border: 1px solid #d1d9e0;
    border-radius: 6px;
    padding: 12px 5px;
    text-align: center;
    background: #fafafa;
  }
  .interest-card i { font-size: 1.3em; color: #3498db; margin-bottom: 6px; display: block; }
  .interest-card span { font-size: 0.85em; font-weight: 600; color: #2c3e50; line-height: 1.1; }

  /* 4. News 样式与折叠逻辑 - 已调小字体 */
  .news-list { list-style: none; padding: 0; margin-bottom: 0; }
  .news-item { 
    margin-bottom: 10px; 
    padding-left: 10px; 
    border-left: 3px solid #f1f1f1; 
    line-height: 1.6;
    transition: border-left 0.3s;
    /* 调小 News 字体至 0.88em */
    font-size: 0.88em; 
    color: #455a64;
  }
  .news-item:hover { border-left: 3px solid #2980b9; }
  .news-date { font-weight: bold; color: #2980b9; margin-right: 10px; white-space: nowrap; }
  
  .extra-news { display: none; }
  #news-toggle:checked ~ .news-list .extra-news { display: list-item; }
  
  .btn-wrap { text-align: left; margin-top: 15px; padding-left: 10px; }
  .more-btn, .less-btn {
    display: inline-block;
    border: 1px solid #2980b9;
    color: #2980b9;
    padding: 4px 15px;
    border-radius: 15px;
    cursor: pointer;
    font-weight: 500;
    font-size: 0.8em;
    transition: all 0.3s ease;
  }
  .more-btn:hover, .less-btn:hover { background-color: #2980b9; color: white; }
  .less-btn { display: none; }
  #news-toggle:checked ~ .btn-wrap .more-btn { display: none; }
  #news-toggle:checked ~ .btn-wrap .less-btn { display: inline-block; }

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
        My research focuses on <b>cooperative algorithm design</b> and their practical applications in <b>intelligent robotics</b>. I am particularly interested in developing <b>information-augmented strategies</b> to enhance the control performance of autonomous systems. My work has been published in several journals and conferences, such as <i>IEEE RAL</i>, <i>IJRNC</i>, <i>IJMAV</i>, <i>DDCLS</i>, and <i>ICGNC</i>. I actively contribute to the academic community as a reviewer for <i>IEEE RAL</i>, <i>ICRA</i>, and <i>IROS</i>.
      </div>
    </div>

    <div class="exp-edu-column">
      <div class="section-title">Work Experience</div>
      <div class="info-item">
        <img src="/images/CITYU1.jpg" class="info-logo">
        <div class="info-content">
          <div class="info-name">City University of Macau</div>
          <div class="info-desc">Faculty of Data Science</div>
        </div>
      </div>

      <div class="section-title" style="margin-top: 50px;">Education Experience</div>
      <div class="info-item">
        <img src="/images/SYSU.jpg" class="info-logo">
        <div class="info-content">
          <div class="info-name">Sun Yat-sen University</div>
          <div class="info-desc">Ph.D. (2024)</div>
        </div>
      </div>
      <div class="info-item">
        <img src="/images/SYSU.jpg" class="info-logo">
        <div class="info-content">
          <div class="info-name">Sun Yat-sen University</div>
          <div class="info-desc">M.Sc. (2020)</div>
        </div>
      </div>
      <div class="info-item">
        <img src="/images/CUG.jpg" class="info-logo">
        <div class="info-content">
          <div class="info-name">CUG</div>
          <div class="info-desc">B.Sc. (2017)</div>
        </div>
      </div>
    </div>
  </div>

  <div class="section-title">Research Interests</div>
  <div class="interests-grid">
    <div class="interest-card"><i class="fas fa-robot"></i><span>Cooperative Control<br>and Applications of UAVs</span></div>
    <div class="interest-card"><i class="fas fa-microchip"></i><span>Swarm Decision-making,<br>Planning and Control</span></div>
    <div class="interest-card"><i class="fas fa-search-location"></i><span>Low-altitude<br>Situational Awareness</span></div>
    <div class="interest-card"><i class="fas fa-cogs"></i><span>Spatial Information<br>Intelligence</span></div>
  </div>

<h2 style="border-bottom: 2px solid #2c3e50; color: #2c3e50; padding-bottom: 8px; margin-top: 40px; font-size: 1.2em;">News</h2>

<div class="news-wrapper">
  <input type="checkbox" id="news-toggle" style="display: none;">
  
  <ul class="news-list" style="font-size: 1em !important;">
    <li class="news-item"><span class="news-date">Apr 2026</span> Our work has been accepted by the <b>International Conference on Guidance, Navigation, and Control (ICGNC)</b>.</li>
    <li class="news-item"><span class="news-date">Apr 2026</span> Our work has been accepted by the <b>International Journal of Micro Air Vehicles (IJMAV)</b>.</li>
    <li class="news-item"><span class="news-date">Mar 2026</span> Another research paper has been accepted by the <b>IEEE Data Driven Control and Learning Systems Conference (DDCLS)</b>.</li>
    <li class="news-item"><span class="news-date">Mar 2026</span> Our work has been accepted by the <b>IEEE Data Driven Control and Learning Systems Conference (DDCLS)</b>.</li>
    <li class="news-item"><span class="news-date">Mar 2026</span> The initial construction of our <b>Indoor Motion Capture Experimental Environment</b> has been completed.</li>

    <li class="news-item extra-news"><span class="news-date">Nov 2025</span> Our research project has been officially funded by the <b>Science and Technology Development Fund (FDCT)</b>, Macau.</li>
    <li class="news-item extra-news"><span class="news-date">Aug 2024</span> Joined the Faculty of Data Science at <b>City University of Macau</b> as an Assistant Professor.</li>
    <li class="news-item extra-news"><span class="news-date">Feb 2024</span> Our work has been accepted by <b>IEEE Robotics and Automation Letters (RAL)</b>.</li>
    <li class="news-item extra-news"><span class="news-date">Sep 2023</span> Our work has been accepted by <b>IEEE Robotics and Automation Letters (RAL)</b>.</li>
    <li class="news-item extra-news"><span class="news-date">Aug 2023</span> Our work has been accepted by the <b>International Journal of Robust and Nonlinear Control (IJRNC)</b>.</li>
    <li class="news-item extra-news"><span class="news-date">Nov 2022</span> Our work was accepted for presentation at the <b>Youth Academic Annual Conference of the Chinese Association of Automation</b>.</li>
    <li class="news-item extra-news"><span class="news-date">Jun 2021</span> Our work has been published in <b>Biodiversity Science</b>.</li>
  </ul>

  <div class="btn-wrap">
    <label for="news-toggle" class="more-btn">Show More ↓</label>
    <label for="news-toggle" class="less-btn">Show Less ↑</label>
  </div>
</div>

<style>
  /* 强制覆盖可能的冲突样式 */
  .news-item { 
    font-size: 0.85em !important; 
    margin-bottom: 10px; 
    padding-left: 10px; 
    border-left: 3px solid #f1f1f1; 
    line-height: 1.5;
  }
  .extra-news { display: none; }
  #news-toggle:checked ~ .news-list .extra-news { display: list-item; }
  .btn-wrap { text-align: left; margin-top: 15px; }
  .more-btn, .less-btn {
    border: 1px solid #2980b9;
    color: #2980b9;
    padding: 3px 12px;
    border-radius: 12px;
    cursor: pointer;
    font-size: 0.75em; /* 按钮也相应调小一点 */
  }
  #news-toggle:checked ~ .btn-wrap .more-btn { display: none; }
  #news-toggle:checked ~ .btn-wrap .less-btn { display: inline-block; }
  .less-btn { display: none; }
</style>

</div>
