---
layout: about
title: Home
permalink: /
subtitle: 

profile:
  align: right
  image: bailan_he.png
  image_circular: false # crops the image to make it circular
  more_info: >
selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false # disable blog posts on homepage
  scrollable: true
  limit: 3
---


I am a third-year PhD student in Computer Science at [**Ludwig Maximilian University of Munich (LMU Munich)**](https://www.lmu.de/de/index.html) and [**Siemens AG**](https://www.siemens.com/global/en.html), jointly supervised by [Prof. Dr. Volker Tresp](https://www.dbs.ifi.lmu.de/~tresp/) and Dr. Yushan Liu. My research centers on developing trustworthy, interpretable, and knowledge-aware generative foundation models, with particular emphasis on **vision-language modeling**, **model safety & red-teaming**, and **hallucination**. Prior to my PhD, I earned an M.Sc. in Statistics from LMU Munich and a B.Sc. in Statistics from the Southwestern University of Finance and Economics, China. I am affiliated with [TRESP Lab](https://tresp-lab.github.io/), [MCML](https://mcml.ai/), and [relAI](https://zuseschoolrelai.de/).

<div style="margin: 20px 0; padding: 15px; background: #f8f9fa; border-radius: 8px; border-left: 4px solid #007bff;">
  <p style="margin: 0; font-size: 14px; color: #666;">
    <strong>Find me also in:</strong>
    <a href="https://scholar.google.com/citations?user=n5zUQtAAAAAJ&hl=en" target="_blank" style="margin-left: 10px; color: #4285f4; text-decoration: none;">
      <i class="ai ai-google-scholar" style="font-size: 18px;"></i>
    </a>
    <a href="https://www.linkedin.com/in/bailan-he-6031461a5/" target="_blank" style="margin-left: 10px; color: #0077b5; text-decoration: none;">
      <i class="fab fa-linkedin" style="font-size: 18px;"></i>
    </a>
    <a href="https://x.com/BailanHe" target="_blank" style="margin-left: 10px; color: #000; text-decoration: none;">
      <i class="fab fa-x-twitter" style="font-size: 18px;"></i>
    </a>
  </p>
</div>

<div style="margin: 20px 0; padding: 15px; background: linear-gradient(135deg, #e3f2fd 0%, #f0f8ff 100%); border-radius: 8px; border-left: 4px solid #2196f3;">
  <p style="margin: 0; font-size: 15px; color: #1565c0; line-height: 1.5;">
    <strong>🔥 Always Hiring!</strong><br>
    Always actively seeking motivated students for both research and master thesis projects. If you're interested in working on the topic of LLMs/MLLMs/Agents/Safety/Diffusion Model, feel free to email me your CV and transcript. Previous supervisions have led to high-quality publications in top venues such as ICLR, COLM, and ACL.<br>
    <strong>Contact:</strong> <a href="mailto:bailan.he.de@gmail.com" style="color: #1976d2; text-decoration: none; font-weight: 500;">bailan.he.de@gmail.com</a>
  </p>
</div>

<style>
.news-title, .publications-title {
  background: linear-gradient(135deg, #2196f3 0%, #1976d2 100%);
  color: white;
  padding: 6px 12px;
  border-radius: 15px;
  font-weight: bold;
  font-size: 14px;
  display: inline-block;
  margin-bottom: 10px;
  box-shadow: 0 2px 4px rgba(33, 150, 243, 0.3);
}

/* Hide original titles */
.news h2, .publications h2 {
  display: none !important;
}

/* Hide any other original section titles */
h2:contains("News"), h2:contains("Publications") {
  display: none !important;
}

/* More aggressive hiding */
h2 {
  display: none !important;
}

/* Show only our custom titles */
.news-title, .publications-title {
  display: inline-block !important;
}

/* Make social media icons smaller */
.social-icons a {
  font-size: 0.8em !important;
}

.social-icons i {
  font-size: 0.8em !important;
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function() {
  // Hide ALL original titles
  const allH2Titles = document.querySelectorAll('h2');
  allH2Titles.forEach(title => {
    title.style.display = 'none';
    title.style.visibility = 'hidden';
  });
  
  // Add title to announcements section
  const announcementsSection = document.querySelector('.news');
  if (announcementsSection) {
    const title = document.createElement('div');
    title.className = 'news-title';
    title.innerHTML = '🥳 Recent News';
    announcementsSection.parentNode.insertBefore(title, announcementsSection);
  }
  
  // Add title to selected papers section
  const selectedPapersSection = document.querySelector('.publications');
  if (selectedPapersSection) {
    const title = document.createElement('div');
    title.className = 'publications-title';
    title.innerHTML = '📄 Selected Publications';
    selectedPapersSection.parentNode.insertBefore(title, selectedPapersSection);
  }
  
});
</script>

<!-- ## 🥳 Recent News

* **09 / 2025** 🏆 We are the winneres of the Red‑Teaming Challenge hosted by <img src="https://img.shields.io/badge/OpenAI-412991?logo=openai&logoColor=white" alt="OpenAI" style="height: 20px; vertical-align: middle; margin: 0 4px;"> and <img src="https://img.shields.io/badge/Kaggle-20BEFF?logo=kaggle&logoColor=white" alt="Kaggle" style="height: 20px; vertical-align: middle; margin: 0 4px;"> (**Top 0.3%** among a total of 5911 international participants)! Stay tuned for our detailed reports!
* **07 / 2025** 🎉 One papers got accepted at **COLM 2025**! One on Multimodal In-context Learning and the other is on Fact Asymmetry. Congrats to all co-authors!

<div style="text-align: center; margin-top: 1rem;">
  <a href="/news/" style="color: #666; text-decoration: none; font-size: 0.9em;">Previous News →</a>
</div> -->
