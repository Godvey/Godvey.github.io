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
        <img src="/images/bio-photo.jpg" class="edu-logo" alt="SYSU">
        <div class="edu-info">
          <div class="uni-name">Sun Yat-sen University</div>
          <div class="deg-name">Ph.D. in Aerospace Science and Technology</div>
        </div>
      </div>
      
      <div class="edu-item">
        <img src="/images/bio-photo.jpg" class="edu-logo" alt="SYSU">
        <div class="edu-info">
          <div class="uni-name">Sun Yat-sen University</div>
          <div class="deg-name">M.Sc. in Surveying and Mapping Engineering</div>
        </div>
      </div>
      
      <div class="edu-item">
        <img src="/images/bio-photo.jpg" class="edu-logo" alt="CUG">
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

<ul class="news-list" id="auto-news-list">
  <li class="news-item"><span class="news-date">[Apr 2026]</span> Our paper on UAV formation control was accepted for presentation at ICGNC 2026.</li>
  <li class="news-item"><span class="news-date">[Aug 2024]</span> Joined the Faculty of Data Science at City University of Macau as an Assistant Professor.</li>
  <li class="news-item"><span class="news-date">[May 2024]</span> Awarded "Finalist" for the Best Paper Award at the DDCLS 2024 conference.</li>
  <li class="news-item"><span class="news-date">[Feb 2023]</span> Commenced Postdoctoral Research at the Oxford Robotics Institute, University of Oxford.</li>
  <li class="news-item"><span class="news-date">[Jan 2023]</span> Example news 5...</li>
  <li class="news-item"><span class="news-date">[Dec 2022]</span> Example news 6...</li>
  <li class="news-item"><span class="news-date">[Nov 2022]</span> Example news 7...</li>
</ul>

<div id="btn-container" style="text-align: center; margin-top: 20px; display: none;">
  <button id="show-more-btn" onclick="toggleNews()" style="background: none; border: 1px solid #2980b9; color: #2980b9; padding: 8px 24px; border-radius: 20px; cursor: pointer; font-weight: 600; transition: all 0.3s; font-size: 0.95em;">
    Show More ↓
  </button>
</div>

<style>
  /* 默認樣式 */
  .news-list { list-style-type: none; padding-left: 0; }
  .news-item { 
    margin-bottom: 12px; 
    padding-left: 10px; 
    border-left: 3px solid #f1f1f1; 
    line-height: 1.6;
  }
  .news-date { font-weight: bold; color: #2980b9; margin-right: 10px; }
  #show-more-btn:hover { background-color: #2980b9; color: white; }
  
  /* 初始強制隱藏多餘新聞，防止頁面閃爍 */
  .news-item:nth-child(n+6) {
    display: none;
  }
</style>

<script>
  function initNews() {
    const list = document.getElementById('auto-news-list');
    if (!list) return;
    
    const items = list.getElementsByTagName('li');
    const btnContainer = document.getElementById('btn-container');

    // 如果總量大於 5 條，則顯示按鈕
    if (items.length > 5) {
      btnContainer.style.display = 'block';
    }
  }

  function toggleNews() {
    const list = document.getElementById('auto-news-list');
    const items = list.getElementsByTagName('li');
    const btn = document.getElementById('show-more-btn');
    
    // 檢查目前第 6 條是否隱藏
    const isHidden = window.getComputedStyle(items[5]).display === 'none';

    if (isHidden) {
      // 展開：顯示所有項目
      for (let i = 5; i < items.length; i++) {
        items[i].style.display = 'block';
      }
      btn.innerHTML = 'Show Less ↑';
    } else {
      // 收起：隱藏 5 條之後的所有項目
      for (let i = 5; i < items.length; i++) {
        items[i].style.display = 'none';
      }
      btn.innerHTML = 'Show More ↓';
    }
  }

  // 雙重保險：確保頁面加載完成後執行初始化
  window.onload = initNews;
  // 針對某些跳轉情況
  document.addEventListener("DOMContentLoaded", initNews);
</script>

</div>
