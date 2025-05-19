---
title: Tianlin Fu Resume
---

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tianlin Fu Resume</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css">
  <style>
    body { padding-top: 70px; }
    .lang-selector { margin-left: auto; }
  </style>
</head>
<body>
  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Tianlin Fu</a>
      <div class="lang-selector">
        <select id="langSelect" class="form-select form-select-sm">
          <option value="en">English</option>
          <option value="zh-CN">简体中文</option>
          <option value="zh-TW">繁體中文</option>
        </select>
      </div>
    </div>
  </nav>

  <!-- Main content -->
  <div class="container mt-4" id="content-en">
    <h2>Contact</h2>
    <p>+86 15960935014 | <a href="mailto:futianlinedu@163.com">futianlinedu@163.com</a> | Fujian Province, 366300, China</p>

    <h2>Education Background</h2>
    <ul>
      <li><strong>City University of Hong Kong</strong> (09/2025 - 06/2026): MSc in Business Information Systems (Financial and Intelligent Technology Stream)</li>
      <li><strong>Minjiang University</strong> (09/2021 - 06/2025): B.Eng. in Software Engineering; Minor in Finance; GPA: 89.03/100; Rank: 1/63</li>
    </ul>

    <h2>Work and Professional Experience</h2>
    <ul>
      <li><strong>Industrial Digital Financial Services Co., Ltd.</strong> (03/2025 - Present): Fintech Intern - Content Management Platform</li>
      <li><strong>Industrial Digital Financial Services Co., Ltd.</strong> (07/2024 - 11/2024): Fintech Intern - CRM Platform</li>
      <li><strong>Industrial Digital Financial Services Co., Ltd.</strong> (07/2023 - 08/2023): Fintech Intern - HR Department</li>
    </ul>

    <h2>Research Experience</h2>
    <ul>
      <li><strong>Benchmarking Single Image Dedusting</strong> (Accepted, 2025)</li>
      <li><strong>Medical AI for ECG Image Recognition</strong> (06/2023 - 12/2023)</li>
      <li><strong>EEG Denoising via HRTS</strong> (01/2023 - 09/2023)</li>
      <li><strong>Personalized Image Aesthetics</strong> (06/2022 - 12/2022)</li>
      <li><strong>3D Reconstruction via GIRAFFE</strong> (06/2022 - 12/2022)</li>
      <li><strong>Fast Encryption of EHR</strong> (05/2022 - 11/2022)</li>
    </ul>

    <h2>Technical Skills</h2>
    <p>Languages: C, Java, Python<br>
    Frontend: Vue.js, HTML, CSS, JS<br>
    Backend: Spring Cloud, Django<br>
    DB: MySQL, Oracle, Neo4J</p>

    <h2>Leadership and Activities</h2>
    <ul>
      <li>Vice President, Organizational Dept, Math & Data Sci College (2022-2023)</li>
      <li>Student Assistant, Party Branch (2023-2024)</li>
    </ul>

    <h2>Other Information</h2>
    <p>Mandarin (Native), English (IELTS 6.0); CET-4: 519 | CET-6: 511 | Mandarin Level 2A</p>
  </div>

  <!-- Placeholder for zh-CN and zh-TW content -->
  <div class="container mt-4 d-none" id="content-zh-CN">
    <p>（这里是简体中文版本内容，请在后续完善）</p>
  </div>

  <div class="container mt-4 d-none" id="content-zh-TW">
    <p>（這裡是繁體中文版本內容，請在後續完善）</p>
  </div>

  <script>
    const langSelect = document.getElementById('langSelect');
    const contents = {
      'en': document.getElementById('content-en'),
      'zh-CN': document.getElementById('content-zh-CN'),
      'zh-TW': document.getElementById('content-zh-TW'),
    };
    langSelect.addEventListener('change', () => {
      for (let key in contents) contents[key].classList.add('d-none');
      contents[langSelect.value].classList.remove('d-none');
    });
  </script>
</body>
</html>
