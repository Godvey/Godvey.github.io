---
permalink: /
# 這裡將標題留空，防止模板自動生成頂部大標題
title: "" 
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

<style>
  /* 隱藏可能殘留的頁面標題（針對某些模板） */
  .page__title {
    display: none !important;
  }

  /* 1. 寬幅佈局容器 */
  .main-wrapper {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
  }

  /* 2. 頂部兩欄 (Education & Biography) */
  .top-section {
    display: flex;
    justify-content: space-between;
    gap: 40px;
    margin-bottom: 30px;
  }

  .edu-column { flex: 1.1; }
  .bio-column { flex: 1; }

  .section-title {
    font-size: 1.35em;
    font-weight: bold;
    color: #2c3e50;
    border-bottom: 2px solid #e1e4e8;
    padding-bottom: 8px;
    margin-bottom: 20px;
  }

  /* 教育項樣式 */
  .edu-item {
    display: flex;
    align-items: center;
    margin-bottom: 15px;
  }

  .edu-logo {
    width: 60px;
    height: 60px;
    margin-right: 15px;
    object-fit: cover;
    border-radius: 4px;
    background: #f8f9fa;
  }

  .edu-info { line-height: 1.4; }
  .uni-name { font-weight: 700; color: #1a252f; font-size: 1.05em; }
  .deg-name { color: #5d6d7e; font-size: 0.92em; font-style: italic; }

  /* 簡介樣式 */
  .bio-text {
    line-height: 1.8;
    text-align: justify;
    color: #34495e;
  }

  /* 3. 研究興趣 (橫向四卡片) */
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

  .interest-card i {
    font-size: 1.5em;
    color: #3498db;
  }

  .interest-card span {
    font-size: 0.95em;
    font-weight: 600;
    color: #2c3e50;
  }

  /* 4. 新聞列表樣式 */
  .news-list {
    list-style-type: none;
    padding-left: 0;
  }

  .news-item {
    margin-bottom: 12px;
    padding-left: 10px;
    border-left: 3px solid #f1f1f1;
    transition: border-left 0.3s;
    line-height: 1.6;
  }

  .news-item:hover {
    border-left: 3px solid #2980b9;
  }

  .news-date {
    font-weight: bold;
    color: #2980b9;
    margin-right: 10px;
  }

  /* 響應式佈局 */
  @media (max-width: 900px) {
    .top-section { flex-direction: column; }
    .interests-grid { grid-template-columns: repeat(2, 1fr); }
  }
</style>

<div class="main-wrapper">

  <div class="top-section">
    <div class="edu-column">
      <div class="section-title">Education</div>
      
      <div class="edu-item">
        <img src="/images/SYSU.jpg" class="edu-logo" alt="SYSU">
        <div class="edu-info">
          <div class="uni-name">Sun Yat-sen University</div>
          <div class="deg-name">Ph.D. in Aerospace Science and Technology</div>
        </div>
      </div>
      
      <div class="edu-item">
        <img src="/images/SYSU.jpg" class="edu-logo" alt="SYSU">
        <div class="edu-info">
          <div class="uni-name">Sun Yat-sen University</div>
          <div class="deg-name">M.Sc. in Surveying and Mapping Engineering</div>
        </div>
      </div>
      
      <div class="edu-item">
        <img src="/images/CUG.jpg" class="edu-logo" alt="CUG">
        <div class="edu-info">
          <div class="uni-name">China University of Geosciences</div>
          <div class="deg-name">B.Sc. in Remote Sensing Science and Technology</div>
        </div>
      </div>
    </div>

    <div class="bio-column">
      <div class="section-title">Biography</div>
      <div class="bio-text">
        Dr. Wei Yu is an Assistant Professor at the Faculty of Data Science, City University of Macau. His research interests primarily focus on <b>UAV swarm coordination</b>, <b>robust and nonlinear control theory</b>, and autonomous navigation in complex environments. Prior to his current appointment, he conducted postdoctoral research at the <b>Oxford Robotics Institute, University of Oxford</b>.
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
    <li class="news-item"><span class="news-date">[Jan 2023]</span> News Item 5 (Visible)...</li>

    <li class="news-item extra-news"><span class="news-date">[Dec 2022]</span> News Item 6 (Hidden)...</li>
    <li class="news-item extra-news"><span class="news-date">[Nov 2022]</span> News Item 7 (Hidden)...</li>
    <li class="news-item extra-news"><span class="news-date">[Oct 2022]</span> News Item 8 (Hidden)...</li>
  </ul>

  <div class="btn-wrap">
    <label for="news-toggle" class="more-btn">Show More ↓</label>
    <label for="news-toggle" class="less-btn">Show Less ↑</label>
  </div>
</div>

<style>
  /* 列表基礎樣式 */
  .news-list { list-style: none; padding: 0; margin-bottom: 0; }
  .news-item { margin-bottom: 12px; padding-left: 10px; border-left: 3px solid #f1f1f1; line-height: 1.6; }
  .news-date { font-weight: bold; color: #2980b9; margin-right: 10px; }

  /* 初始狀態：隱藏多餘新聞 */
  .extra-news { display: none; }

  /* 當選取框被選中時：顯示所有 extra-news */
  #news-toggle:checked ~ .news-list .extra-news {
    display: block;
  }

  /* 按鈕容器：左對齊並與文字起始線保持一致 */
  .btn-wrap { 
    text-align: left; 
    margin-top: 15px; 
    padding-left: 10px; 
  }

  /* 按鈕樣式：更輕量、專業 */
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
  
  .more-btn:hover, .less-btn:hover { 
    background-color: #2980b9; 
    color: white; 
  }

  /* 切換按鈕文字顯示 */
  .less-btn { display: none; } /* 初始隱藏「收起」 */
  
  #news-toggle:checked ~ .btn-wrap .more-btn { display: none; }
  #news-toggle:checked ~ .btn-wrap .less-btn { display: inline-block; }
</style>

</div>
