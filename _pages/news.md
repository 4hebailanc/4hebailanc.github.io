---
layout: page
title: News
permalink: /news/
nav: true
nav_order: 7
---

<style>
h1 {
  display: none !important;
}
</style>

<div class="news-filter" style="margin-bottom: 2rem;">
  <div style="text-align: center;">
    <button onclick="filterNews('all')" class="filter-btn active" id="btn-all">All</button>
    <button onclick="filterNews('2025')" class="filter-btn" id="btn-2025">2025</button>
  </div>
</div>

<style>
.filter-btn {
  background: #f8f9fa;
  border: 2px solid #e9ecef;
  padding: 8px 16px;
  margin: 0 5px;
  border-radius: 20px;
  cursor: pointer;
  transition: all 0.3s ease;
  font-weight: 500;
}

.filter-btn:hover {
  background: #e9ecef;
  transform: translateY(-2px);
}

.filter-btn.active {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  border-color: #667eea;
}

.news-item {
  transition: all 0.3s ease;
}
</style>

<div id="news-container">
  {% include news.liquid %}
</div>

<script>
function filterNews(year) {
  // Remove active class from all buttons
  document.querySelectorAll('.filter-btn').forEach(btn => {
    btn.classList.remove('active');
  });
  
  // Add active class to clicked button
  event.target.classList.add('active');
  
  // Filter news items
  const newsItems = document.querySelectorAll('.news-item');
  newsItems.forEach(item => {
    if (year === 'all') {
      item.style.display = 'block';
    } else {
      const itemYear = item.getAttribute('data-year');
      if (itemYear === year) {
        item.style.display = 'block';
      } else {
        item.style.display = 'none';
      }
    }
  });
}

// Set default filter to 2025
document.addEventListener('DOMContentLoaded', function() {
  filterNews('2025');
});
</script>
