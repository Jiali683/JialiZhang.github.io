---
permalink: /
title: "👋Welcome to my Homepage😃"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


<span class='anchor' id='about-me'></span>
<style>
.about-hero-section {
  position: relative;
  margin-top: 35px;
  margin-bottom: 55px;
  padding: 34px 36px;
  border-radius: 26px;
  overflow: hidden;
  background: linear-gradient(135deg, rgba(255,255,255,0.92), rgba(244,249,255,0.92));
  border: 1px solid rgba(0, 53, 107, 0.14);
  box-shadow: 0 14px 36px rgba(0, 53, 107, 0.10);
  animation: aboutFadeUp 0.8s ease both;
}

.about-hero-section::before {
  content: "";
  position: absolute;
  top: -90px;
  right: -90px;
  width: 230px;
  height: 230px;
  background: radial-gradient(circle, rgba(0, 53, 107, 0.22), transparent 68%);
  transition: all 0.4s ease;
}

.about-hero-section::after {
  content: "";
  position: absolute;
  left: -80px;
  bottom: -80px;
  width: 210px;
  height: 210px;
  background: radial-gradient(circle, rgba(111, 66, 193, 0.16), transparent 70%);
}

.about-hero-section:hover::before {
  transform: scale(1.25);
}

.about-hero-content {
  position: relative;
  z-index: 1;
}

.about-eyebrow {
  display: inline-block;
  margin-bottom: 14px;
  padding: 5px 13px;
  font-size: 13px;
  font-weight: 800;
  letter-spacing: 0.4px;
  color: #00356b;
  background: #eaf3ff;
  border: 1px solid #c8ddff;
  border-radius: 999px;
}

.about-name {
  width: fit-content;
  max-width: 100%;
  margin-bottom: 20px;
  font-size: 30px;
  font-weight: 850;
  line-height: 1.3;
  color: #1f1f1f;
  overflow: hidden;
  white-space: nowrap;
  border-right: 3px solid #00356b;
  animation: typingName 2.2s steps(24, end), blinkCursor 0.8s step-end infinite;
}

.about-name span {
  background: linear-gradient(90deg, #00356b, #1f6feb, #7b2cbf);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.about-text {
  font-size: 16.5px;
  line-height: 1.75;
  color: #3f3f3f;
  margin-bottom: 14px;
}

.about-text a {
  font-weight: 800;
  color: #00356b;
  text-decoration: none;
  border-bottom: 2px solid rgba(0, 53, 107, 0.25);
  transition: all 0.25s ease;
}

.about-text a:hover {
  color: #1f6feb;
  border-bottom-color: #1f6feb;
}

.about-highlight {
  font-weight: 800;
  color: #111;
}

.research-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 9px;
  margin-top: 18px;
  margin-bottom: 22px;
}

.research-tag {
  display: inline-block;
  padding: 6px 12px;
  font-size: 13px;
  font-weight: 750;
  color: #00356b;
  background: rgba(234, 243, 255, 0.85);
  border: 1px solid rgba(0, 53, 107, 0.16);
  border-radius: 999px;
  transition: all 0.28s ease;
}

.research-tag:hover {
  transform: translateY(-3px);
  background: #00356b;
  color: #ffffff;
  box-shadow: 0 8px 18px rgba(0, 53, 107, 0.18);
}

.collab-line {
  margin-top: 16px;
  padding: 13px 16px;
  border-left: 4px solid #00356b;
  border-radius: 12px;
  background: rgba(234, 243, 255, 0.72);
  font-size: 16px;
  font-weight: 700;
  color: #2f2f2f;
}

.life-card {
  position: relative;
  z-index: 1;
  margin-top: 26px;
  padding: 22px 24px;
  border-radius: 22px;
  background: linear-gradient(135deg, #ffffff 0%, #fff8fd 100%);
  border: 1px solid rgba(111, 66, 193, 0.16);
  box-shadow: 0 10px 24px rgba(111, 66, 193, 0.08);
  overflow: hidden;
  transition: all 0.32s ease;
}

.life-card::before {
  content: "✦";
  position: absolute;
  right: 22px;
  top: 18px;
  font-size: 34px;
  color: rgba(111, 66, 193, 0.18);
  transition: all 0.35s ease;
}

.life-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 18px 36px rgba(111, 66, 193, 0.16);
}

.life-card:hover::before {
  transform: rotate(18deg) scale(1.2);
  color: rgba(111, 66, 193, 0.34);
}

.life-title {
  margin-bottom: 14px;
  font-size: 20px;
  font-weight: 850;
  color: #1f1f1f;
}

.life-title i {
  margin-right: 8px;
  color: #7b2cbf;
}

.life-intro {
  margin-bottom: 12px;
  font-size: 15.5px;
  color: #444;
}

.life-highlight {
  font-weight: 900;
  background: linear-gradient(90deg, #00356b, #1f6feb, #7b2cbf);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.hobby-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 9px;
  margin-top: 10px;
}

.hobby-tag {
  display: inline-block;
  padding: 7px 12px;
  font-size: 13.5px;
  font-weight: 750;
  color: #4b2a63;
  background: #f5ecff;
  border: 1px solid #dfc8ff;
  border-radius: 999px;
  transition: all 0.28s ease;
}

.hobby-tag:hover {
  transform: translateY(-3px) rotate(-1deg);
  background: #7b2cbf;
  color: #ffffff;
  box-shadow: 0 8px 18px rgba(111, 66, 193, 0.22);
}

@keyframes aboutFadeUp {
  from {
    opacity: 0;
    transform: translateY(22px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes typingName {
  from {
    width: 0;
  }
  to {
    width: 100%;
  }
}

@keyframes blinkCursor {
  50% {
    border-color: transparent;
  }
}

@media screen and (max-width: 768px) {
  .about-hero-section {
    padding: 26px 20px;
  }

  .about-name {
    font-size: 24px;
    white-space: normal;
    border-right: none;
    animation: aboutFadeUp 0.8s ease both;
  }

  .about-text {
    font-size: 15.5px;
  }

  .life-card {
    padding: 20px 18px;
  }
}
</style>

<div class="about-hero-section">

  <div class="about-hero-content">

    <div class="about-eyebrow">About Me</div>

    <div class="about-name">
      Hi, I am <span>Jiali Zhang</span>.
    </div>

    <p class="about-text">
      My name is <span class="about-highlight">Jiali Zhang</span>, and I am currently a postgraduate researcher in the
      <span class="about-highlight">Department of Pathology at Yale School of Medicine</span>, under the supervision of
      <a href="https://medicine.yale.edu/profile/wonjae-huh/" target="_blank">Dr. Won Jae Huh</a>.
    </p>

    <p class="about-text">
      Prior to this, I completed my master’s degree in
      <span class="about-highlight">Veterinary Medicine</span> at
      <span class="about-highlight">China Agricultural University</span> in 2024 and obtained the
      <span class="about-highlight">Veterinary Qualification Certificate</span>.
    </p>

    <p class="about-text">
      My research interests include the mechanisms underlying gastrointestinal diseases and their therapeutic strategies,
      stem cell therapy, drug delivery system development, and organoids.
    </p>

    <div class="research-tags">
      <span class="research-tag">Gastrointestinal Diseases</span>
      <span class="research-tag">Therapeutic Strategies</span>
      <span class="research-tag">Stem Cell Therapy</span>
      <span class="research-tag">Drug Delivery Systems</span>
      <span class="research-tag">Organoids</span>
    </div>

    <div class="collab-line">
      Feel free to reach out if you'd like to discuss research or explore potential collaboration!
    </div>

    <div class="life-card">
      <div class="life-title">
        <i class="fas fa-pen-fancy"></i> Life Experiencer
      </div>

      <div class="life-intro">
        Enjoy spending my <span class="life-highlight">spare time</span> on:
      </div>

      <div class="hobby-tags">
        <span class="hobby-tag">Dancing 💃</span>
        <span class="hobby-tag">Resistance Training 🏋️</span>
        <span class="hobby-tag">Snorkeling 🤿</span>
        <span class="hobby-tag">Climbing 🧗‍♀️</span>
        <span class="hobby-tag">Yoga 🧘‍♀️</span>
        <span class="hobby-tag">Movies 🎬</span>
        <span class="hobby-tag">Games 🎮</span>
        <span class="hobby-tag">Music 🎵</span>
        <span class="hobby-tag">Traveling the World 🌏</span>
      </div>
    </div>

  </div>

</div>
      
<span class='anchor' id='-news'></span>
# News🔥
<style>
.news-section {
  margin-top: 35px;
  margin-bottom: 45px;
}

.news-title {
  font-size: 28px;
  font-weight: 700;
  margin-bottom: 25px;
  color: #2b2b2b;
}

.news-timeline {
  position: relative;
  margin-left: 10px;
  padding-left: 28px;
  border-left: 3px solid #d8e6ff;
}

.news-item {
  position: relative;
  margin-bottom: 18px;
  padding: 16px 20px;
  background: #ffffff;
  border-radius: 14px;
  box-shadow: 0 4px 14px rgba(0, 0, 0, 0.06);
  transition: all 0.28s ease;
  animation: fadeInUp 0.6s ease both;
}

.news-item:hover {
  transform: translateX(8px);
  box-shadow: 0 8px 24px rgba(0, 80, 180, 0.16);
  background: linear-gradient(135deg, #ffffff 0%, #f5f9ff 100%);
}

.news-item::before {
  content: "";
  position: absolute;
  left: -39px;
  top: 22px;
  width: 15px;
  height: 15px;
  background: #1f6feb;
  border: 3px solid #ffffff;
  border-radius: 50%;
  box-shadow: 0 0 0 4px #d8e6ff;
}

.news-date {
  display: inline-block;
  min-width: 90px;
  font-weight: 700;
  color: #00356b;
  margin-right: 8px;
}

.news-text {
  color: #444;
  font-size: 16px;
  line-height: 1.55;
}

.news-highlight {
  font-weight: 700;
  color: #111;
}

.news-badge {
  display: inline-block;
  margin-left: 8px;
  padding: 2px 8px;
  font-size: 12px;
  font-weight: 700;
  color: #ffffff;
  background: #ff8a00;
  border-radius: 999px;
  vertical-align: middle;
}

.news-item:nth-child(1) { animation-delay: 0.05s; }
.news-item:nth-child(2) { animation-delay: 0.10s; }
.news-item:nth-child(3) { animation-delay: 0.15s; }
.news-item:nth-child(4) { animation-delay: 0.20s; }
.news-item:nth-child(5) { animation-delay: 0.25s; }
.news-item:nth-child(6) { animation-delay: 0.30s; }
.news-item:nth-child(7) { animation-delay: 0.35s; }
.news-item:nth-child(8) { animation-delay: 0.40s; }
.news-item:nth-child(9) { animation-delay: 0.45s; }
.news-item:nth-child(10) { animation-delay: 0.50s; }

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(18px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@media screen and (max-width: 768px) {
  .news-timeline {
    padding-left: 22px;
  }

  .news-item {
    padding: 14px 16px;
  }

  .news-date {
    display: block;
    margin-bottom: 5px;
  }

  .news-item::before {
    left: -33px;
  }
}
</style>

<div class="news-section">

  <div class="news-timeline">

    <div class="news-item">
      <span class="news-date">2026.02</span>
      <span class="news-text">
        Our work has been accepted by <span class="news-highlight">DDW, 2026</span> 🎉
        <span class="news-badge">Accepted</span>
      </span>
    </div>

    <div class="news-item">
      <span class="news-date">2025.11</span>
      <span class="news-text">
        Our work has been accepted by <span class="news-highlight">The Journal of Pathology</span> 🎉
        <span class="news-badge">Accepted</span>
      </span>
    </div>

    <div class="news-item">
      <span class="news-date">2025.08</span>
      <span class="news-text">
        Our work was presented at the <span class="news-highlight">5th Annual Yale Postgraduate Symposium, 2025</span> 🎉
        <span class="news-badge">Presentation</span>
      </span>
    </div>

    <div class="news-item">
      <span class="news-date">2024.10</span>
      <span class="news-text">
        Joined <span class="news-highlight">Dr. Huh's lab at Yale School of Medicine</span> as a postgraduate researcher.
      </span>
    </div>

    <div class="news-item">
      <span class="news-date">2024.06</span>
      <span class="news-text">
        Graduated from <span class="news-highlight">China Agricultural University</span> as a merit student.
      </span>
    </div>

    <div class="news-item">
      <span class="news-date">2023.10</span>
      <span class="news-text">
        Our work has been accepted by <span class="news-highlight">The 22nd Academic Symposium of the Animal Anatomy and Histology & Embryology Branch of the Chinese Association of Animal Science and Veterinary Medicine</span> 🎉
        <span class="news-badge">Accepted</span>
      </span>
    </div>

    <div class="news-item">
      <span class="news-date">2023.08</span>
      <span class="news-text">
        Our work has been accepted by <span class="news-highlight">BMC Cell Communication and Signaling</span> 🎉
        <span class="news-badge">Accepted</span>
      </span>
    </div>

    <div class="news-item">
      <span class="news-date">2021.09</span>
      <span class="news-text">
        Started my Master's program at <span class="news-highlight">China Agricultural University</span>.
      </span>
    </div>

    <div class="news-item">
      <span class="news-date">2020.05</span>
      <span class="news-text">
        Participated in the <span class="news-highlight">China Agricultural University Summer Camp</span> and was granted exemption-based admission to the master's program.
      </span>
    </div>

    <div class="news-item">
      <span class="news-date">2017.09</span>
      <span class="news-text">
        Started my Bachelor's program at <span class="news-highlight">Jilin Agricultural University</span>.
      </span>
    </div>

  </div>

</div>

<span class='anchor' id='educations-training'></span>
# Educations & Training📚
<style>
.edu-glass-section {
  margin-top: 40px;
  margin-bottom: 55px;
}

.edu-glass-title {
  font-size: 28px;
  font-weight: 800;
  margin-bottom: 28px;
  color: #2b2b2b;
}

.edu-glass-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 22px;
}

.edu-glass-card {
  position: relative;
  overflow: hidden;
  min-height: 230px;
  padding: 24px 22px;
  border-radius: 22px;
  background: rgba(255, 255, 255, 0.78);
  border: 1px solid rgba(0, 53, 107, 0.14);
  box-shadow: 0 10px 28px rgba(0, 53, 107, 0.10);
  transition: all 0.35s ease;
  animation: eduPopIn 0.7s ease both;
}

.edu-glass-card::before {
  content: "";
  position: absolute;
  top: -80px;
  right: -80px;
  width: 170px;
  height: 170px;
  background: radial-gradient(circle, rgba(0, 53, 107, 0.20), transparent 65%);
  transition: all 0.35s ease;
}

.edu-glass-card::after {
  content: "";
  position: absolute;
  inset: 0;
  border-radius: 22px;
  padding: 1.5px;
  background: linear-gradient(135deg, rgba(0, 53, 107, 0.55), rgba(31, 111, 235, 0.15), rgba(111, 66, 193, 0.35));
  -webkit-mask: 
    linear-gradient(#fff 0 0) content-box, 
    linear-gradient(#fff 0 0);
  -webkit-mask-composite: xor;
          mask-composite: exclude;
  opacity: 0;
  transition: opacity 0.35s ease;
}

.edu-glass-card:hover {
  transform: translateY(-10px) scale(1.02);
  box-shadow: 0 18px 40px rgba(0, 53, 107, 0.20);
}

.edu-glass-card:hover::before {
  transform: scale(1.35);
  opacity: 0.9;
}

.edu-glass-card:hover::after {
  opacity: 1;
}

.edu-glass-icon {
  position: relative;
  z-index: 1;
  font-size: 34px;
  margin-bottom: 14px;
}

.edu-glass-date {
  position: relative;
  z-index: 1;
  display: inline-block;
  margin-bottom: 16px;
  padding: 5px 12px;
  font-size: 13px;
  font-weight: 800;
  color: #00356b;
  background: #eaf3ff;
  border-radius: 999px;
}

.edu-glass-degree {
  position: relative;
  z-index: 1;
  font-size: 20px;
  font-weight: 800;
  color: #1f1f1f;
  margin-bottom: 10px;
  line-height: 1.3;
}

.edu-glass-school {
  position: relative;
  z-index: 1;
  font-size: 15.5px;
  line-height: 1.6;
  color: #4a4a4a;
}

.edu-glass-highlight {
  font-weight: 900;
  background: linear-gradient(90deg, #00356b, #1f6feb, #7b2cbf);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.edu-glass-status {
  position: relative;
  z-index: 1;
  display: inline-block;
  margin-top: 14px;
  padding: 4px 10px;
  font-size: 12px;
  font-weight: 800;
  color: #ffffff;
  background: #00356b;
  border-radius: 999px;
}

.edu-glass-card:nth-child(1) {
  animation-delay: 0.05s;
}

.edu-glass-card:nth-child(2) {
  animation-delay: 0.15s;
}

.edu-glass-card:nth-child(3) {
  animation-delay: 0.25s;
}

@keyframes eduPopIn {
  from {
    opacity: 0;
    transform: translateY(18px) scale(0.96);
  }
  to {
    opacity: 1;
    transform: translateY(0) scale(1);
  }
}

@media screen and (max-width: 900px) {
  .edu-glass-grid {
    grid-template-columns: 1fr;
  }

  .edu-glass-card {
    min-height: auto;
  }
}
</style>

<div class="edu-glass-section">

  <div class="edu-glass-grid">

    <div class="edu-glass-card">
      <div class="edu-glass-icon">🔬</div>
      <div class="edu-glass-date">2024.10 - Present</div>
      <div class="edu-glass-degree">Postgraduate Researcher</div>
      <div class="edu-glass-school">
        Yale School of Medicine<br>
        Yale University
      </div>
      <div class="edu-glass-status">Current</div>
    </div>

    <div class="edu-glass-card">
      <div class="edu-glass-icon">🎓</div>
      <div class="edu-glass-date">2021.09 - 2024.06</div>
      <div class="edu-glass-degree">Master of Science</div>
      <div class="edu-glass-school">
        College of Veterinary Medicine<br>
        <span class="edu-glass-highlight">with Distinction</span><br>
        China Agricultural University
      </div>
    </div>

    <div class="edu-glass-card">
      <div class="edu-glass-icon">📘</div>
      <div class="edu-glass-date">2017.09 - 2021.06</div>
      <div class="edu-glass-degree">Bachelor of Science</div>
      <div class="edu-glass-school">
        College of Veterinary Medicine<br>
        <span class="edu-glass-highlight">with Distinction</span><br>
        Jilin Agricultural University
      </div>
    </div>

  </div>

</div>

<span class='anchor' id='-publications'></span>
# Publications📖
<style>
.publications-section {
  margin-top: 40px;
}

.publications-title {
  font-size: 30px;
  font-weight: 700;
  margin-bottom: 20px;
  border-bottom: 1px solid #e5e5e5;
  padding-bottom: 15px;
}

.publication-item {
  display: flex;
  align-items: center;
  gap: 35px;
  padding: 40px 0;
  border-bottom: 1px solid #e5e5e5;
}

.publication-image-box {
  position: relative;
  flex: 0 0 42%;
}

.publication-image {
  width: 100%;
  border-radius: 2px;
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.25);
}

.conference-label {
  position: absolute;
  top: 10px;
  left: -10px;
  background-color: #003f9e;
  color: white;
  font-weight: 700;
  font-size: 15px;
  padding: 5px 18px;
}

.publication-content {
  flex: 1;
}

.publication-title {
  font-size: 21px;
  font-weight: 700;
  line-height: 1.35;
  margin-bottom: 12px;
}

.publication-title a {
  color: #0645ad;
  text-decoration: underline;
}

.publication-authors {
  font-size: 17px;
  font-weight: 700;
  color: #555;
  margin-bottom: 12px;
}

.publication-description {
  font-size: 17px;
  line-height: 1.55;
  color: #444;
}

.publication-description ul {
  margin-top: 8px;
  padding-left: 24px;
}

/* Mobile responsive */
@media screen and (max-width: 768px) {
  .publication-item {
    flex-direction: column;
    align-items: flex-start;
    gap: 20px;
  }

  .publication-image-box {
    flex: 0 0 100%;
    width: 100%;
  }

  .conference-label {
    left: 0;
    font-size: 14px;
  }

  .publication-title {
    font-size: 19px;
  }

  .publication-authors,
  .publication-description {
    font-size: 16px;
  }
}
</style>

<div class="publications-section">

  <!-- Publication 1 -->
  <div class="publication-item">

    <div class="publication-image-box">
      <img class="publication-image" src="{{ site.baseurl }}/images/Publication 1.png" alt="Publication figure">
    </div>

    <div class="publication-content">
      <div class="publication-title">
        <a href="https://pathsocjournals.onlinelibrary.wiley.com/doi/abs/10.1002/path.6488">
          M-BRe: Transcriptomic profiling reveals the role of Hedgehog signaling as a biomarker and in the pathogenesis of Ménétrier's disease
        </a>
      </div>

      <div class="publication-authors">
        Miyoung Shin, Tryston T Gabriel, Fred Kwame Ofosu, Jiali Zhang, Tricia T Wang, Matthew E Bechard, Robert J Coffey, Won Jae Huh<sup>*</sup>
      </div>

      <div class="publication-description">
        <ul>
          <li>
            This study provides valuable insights into the potential mechanisms underlying the similar clinico-pathologic features observed in MD and JPS. We also identified GLI1 and HHIP as diagnostic markers that can help distinguish MD from JPS. Furthermore, Hh signaling was shown to play an important role in the pathogenesis of MD and can function as a potential therapeutic target.
          </li>
        </ul>
      </div>
    </div>

  </div>

  <!-- Publication 2 -->
  <div class="publication-item">

    <div class="publication-image-box">
      <img class="publication-image" src="{{ site.baseurl }}/images/Publication 2.png" alt="Publication figure">
    </div>

    <div class="publication-content">
      <div class="publication-title">
        <a href="https://link.springer.com/article/10.1186/s12964-023-01292-0">
          Extracellular vesicle therapy for obesity-induced NAFLD: a comprehensive review of current evidence
        </a>
      </div>

      <div class="publication-authors">
        Jiali Zhang, Baochen Ma, Zixu Wang, Yaoxing Chen, Chengzhong Li, Yulan Dong<sup>*</sup>
      </div>

      <div class="publication-description">
        <ul>
          <li>
            We highlight therapeutic approaches using exosomes in the clinical treatment of NAFLD, which provide valuable insights into targeting NAFLD in the clinical setting.
          </li>
        </ul>
      </div>
    </div>

  </div>

</div>

<span class='anchor' id='-talks'></span>
# Talks🗣️
  
<span class='anchor' id='awards-honors'></span>
# Awards & Honors🏆
<style>
.honor-section {
  margin-top: 40px;
  margin-bottom: 55px;
}

.honor-title {
  font-size: 28px;
  font-weight: 800;
  margin-bottom: 26px;
  color: #2b2b2b;
}

.honor-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 18px;
}

.honor-card {
  position: relative;
  overflow: hidden;
  padding: 18px 20px 18px 22px;
  border-radius: 18px;
  background: linear-gradient(135deg, #ffffff 0%, #fffaf0 100%);
  border: 1px solid rgba(205, 155, 35, 0.22);
  box-shadow: 0 8px 22px rgba(80, 60, 10, 0.08);
  transition: all 0.32s ease;
  animation: honorFadeUp 0.65s ease both;
}

.honor-card::before {
  content: "";
  position: absolute;
  top: -55px;
  right: -55px;
  width: 130px;
  height: 130px;
  background: radial-gradient(circle, rgba(255, 199, 44, 0.32), transparent 68%);
  transition: all 0.35s ease;
}

.honor-card::after {
  content: "✦";
  position: absolute;
  right: 18px;
  bottom: 12px;
  font-size: 28px;
  color: rgba(205, 155, 35, 0.20);
  transition: all 0.35s ease;
}

.honor-card:hover {
  transform: translateY(-7px);
  box-shadow: 0 16px 34px rgba(180, 125, 20, 0.20);
  border-color: rgba(205, 155, 35, 0.55);
}

.honor-card:hover::before {
  transform: scale(1.35);
  opacity: 1;
}

.honor-card:hover::after {
  transform: rotate(18deg) scale(1.15);
  color: rgba(205, 155, 35, 0.42);
}

.honor-year {
  position: relative;
  z-index: 1;
  display: inline-block;
  margin-bottom: 10px;
  padding: 4px 11px;
  font-size: 13px;
  font-weight: 800;
  color: #7a4b00;
  background: linear-gradient(135deg, #fff1b8, #ffd76a);
  border-radius: 999px;
  box-shadow: 0 3px 8px rgba(205, 155, 35, 0.22);
}

.honor-name {
  position: relative;
  z-index: 1;
  font-size: 16.5px;
  font-weight: 700;
  line-height: 1.48;
  color: #333;
}

.honor-name strong {
  color: #111;
}

.honor-card.featured {
  background: linear-gradient(135deg, #fffdf5 0%, #fff3c4 100%);
  border-color: rgba(205, 155, 35, 0.45);
}

.honor-card.featured .honor-year {
  color: #ffffff;
  background: linear-gradient(135deg, #b8860b, #f0b429);
}

.honor-card:nth-child(1) { animation-delay: 0.04s; }
.honor-card:nth-child(2) { animation-delay: 0.08s; }
.honor-card:nth-child(3) { animation-delay: 0.12s; }
.honor-card:nth-child(4) { animation-delay: 0.16s; }
.honor-card:nth-child(5) { animation-delay: 0.20s; }
.honor-card:nth-child(6) { animation-delay: 0.24s; }
.honor-card:nth-child(7) { animation-delay: 0.28s; }
.honor-card:nth-child(8) { animation-delay: 0.32s; }
.honor-card:nth-child(9) { animation-delay: 0.36s; }
.honor-card:nth-child(10) { animation-delay: 0.40s; }
.honor-card:nth-child(11) { animation-delay: 0.44s; }
.honor-card:nth-child(12) { animation-delay: 0.48s; }
.honor-card:nth-child(13) { animation-delay: 0.52s; }

@keyframes honorFadeUp {
  from {
    opacity: 0;
    transform: translateY(18px) scale(0.98);
  }
  to {
    opacity: 1;
    transform: translateY(0) scale(1);
  }
}

@media screen and (max-width: 768px) {
  .honor-grid {
    grid-template-columns: 1fr;
  }

  .honor-card {
    padding: 17px 18px;
  }

  .honor-name {
    font-size: 15.5px;
  }
}
</style>

<div class="honor-section">

  <div class="honor-grid">

    <div class="honor-card featured">
      <div class="honor-year">2024</div>
      <div class="honor-name"><strong>Beijing Outstanding Graduates</strong></div>
    </div>

    <div class="honor-card featured">
      <div class="honor-year">2024</div>
      <div class="honor-name"><strong>Outstanding Graduate of the University</strong></div>
    </div>

    <div class="honor-card">
      <div class="honor-year">2024 & 2021</div>
      <div class="honor-name">Second-class Academic Scholarship</div>
    </div>

    <div class="honor-card featured">
      <div class="honor-year">2023</div>
      <div class="honor-name"><strong>National Scholarship</strong></div>
    </div>

    <div class="honor-card">
      <div class="honor-year">2023</div>
      <div class="honor-name">Xiong Dashi Dean’s Scholarship</div>
    </div>

    <div class="honor-card">
      <div class="honor-year">2023</div>
      <div class="honor-name">First-class Academic Scholarship</div>
    </div>

    <div class="honor-card">
      <div class="honor-year">2021</div>
      <div class="honor-name">Second-class Major Scholarship</div>
    </div>

    <div class="honor-card">
      <div class="honor-year">2020 & 2018</div>
      <div class="honor-name">Jilin Province Scholarship</div>
    </div>

    <div class="honor-card">
      <div class="honor-year">2020 & 2019 & 2018 & 2017</div>
      <div class="honor-name">First-class Major Scholarship</div>
    </div>

    <div class="honor-card">
      <div class="honor-year">2019</div>
      <div class="honor-name">Excellence Award at the 6th Shengtai’er Cup Veterinary Medicine Professional Skills Competition</div>
    </div>

    <div class="honor-card">
      <div class="honor-year">2018</div>
      <div class="honor-name">DNB Encouragement Scholarship</div>
    </div>

    <div class="honor-card">
      <div class="honor-year">2018</div>
      <div class="honor-name">College Merit Student</div>
    </div>

    <div class="honor-card">
      <div class="honor-year">2018</div>
      <div class="honor-name">University Model Student in Learning</div>
    </div>

  </div>

</div>
  
<span class='anchor' id='-internships'></span>
# Internships💼
<style>
.internship-section {
  margin-top: 40px;
  margin-bottom: 55px;
}

.internship-title {
  font-size: 28px;
  font-weight: 800;
  margin-bottom: 26px;
  color: #2b2b2b;
}

.internship-list {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.internship-card {
  position: relative;
  overflow: hidden;
  padding: 22px 24px 22px 26px;
  border-radius: 20px;
  background: linear-gradient(135deg, #ffffff 0%, #f6fbff 100%);
  border: 1px solid rgba(0, 53, 107, 0.14);
  box-shadow: 0 8px 24px rgba(0, 53, 107, 0.08);
  transition: all 0.32s ease;
  animation: internshipSlideIn 0.65s ease both;
}

.internship-card::before {
  content: "";
  position: absolute;
  left: 0;
  top: 18px;
  bottom: 18px;
  width: 5px;
  border-radius: 999px;
  background: linear-gradient(180deg, #00356b, #1f6feb, #6f42c1);
}

.internship-card::after {
  content: "💼";
  position: absolute;
  right: 22px;
  bottom: 16px;
  font-size: 38px;
  opacity: 0.10;
  transition: all 0.35s ease;
}

.internship-card:hover {
  transform: translateY(-7px) translateX(6px);
  box-shadow: 0 16px 36px rgba(0, 53, 107, 0.18);
  border-color: rgba(0, 53, 107, 0.32);
}

.internship-card:hover::after {
  opacity: 0.22;
  transform: rotate(-8deg) scale(1.12);
}

.internship-date {
  display: inline-block;
  margin-bottom: 12px;
  padding: 5px 12px;
  font-size: 13px;
  font-weight: 800;
  color: #ffffff;
  background: #00356b;
  border-radius: 999px;
}

.internship-place {
  font-size: 19px;
  font-weight: 800;
  color: #1f1f1f;
  line-height: 1.35;
  margin-bottom: 8px;
  padding-right: 45px;
}

.internship-location {
  display: inline-block;
  padding: 4px 10px;
  font-size: 13px;
  font-weight: 700;
  color: #00356b;
  background: #eaf3ff;
  border: 1px solid #c8ddff;
  border-radius: 999px;
}

.internship-type {
  display: inline-block;
  margin-left: 8px;
  padding: 4px 10px;
  font-size: 13px;
  font-weight: 700;
  color: #5b2b82;
  background: #f3eaff;
  border: 1px solid #dcc6ff;
  border-radius: 999px;
}

.internship-card:nth-child(1) {
  animation-delay: 0.06s;
}

.internship-card:nth-child(2) {
  animation-delay: 0.16s;
}

@keyframes internshipSlideIn {
  from {
    opacity: 0;
    transform: translateX(-18px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@media screen and (max-width: 768px) {
  .internship-card {
    padding: 20px 18px 20px 22px;
  }

  .internship-place {
    font-size: 17px;
    padding-right: 35px;
  }

  .internship-type {
    margin-left: 0;
    margin-top: 7px;
  }
}
</style>

<div class="internship-section">

  <div class="internship-list">

    <div class="internship-card">
      <div class="internship-date">2023.03</div>
      <div class="internship-place">
        Beijing Elk Ecological Experimental Animal Center
      </div>
      <span class="internship-location">Beijing, China</span>
      <span class="internship-type">Experimental Animal Center</span>
    </div>

    <div class="internship-card">
      <div class="internship-date">2020.04</div>
      <div class="internship-place">
        Ruipai Pet Hospital
      </div>
      <span class="internship-location">Changsha, Hunan, China</span>
      <span class="internship-type">Veterinary Clinical Internship</span>
    </div>

  </div>

</div>

# CV
please see the attachment


