---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Click this <button id="toggleButton" class="btn btn-primary" onclick="toggleCV()">切换中文简历</button> button to change the language between Chinese and English: 

<iframe id="englishCV" src="/files/Zhichuan MA_CV_EN.pdf" style="width:100%; height:1414px;" frameborder="0"></iframe>
<iframe id="chineseCV" src="/files/Zhichuan MA_CV_CN.pdf" style="width:100%; height:1414px; display:none;" frameborder="0"></iframe>

<script>
function toggleCV() {
  var englishCV = document.getElementById("englishCV");
  var chineseCV = document.getElementById("chineseCV");
  var button = document.getElementById("toggleButton");

  if (englishCV.style.display === "none") {
    englishCV.style.display = "block";
    chineseCV.style.display = "none";
    button.innerHTML = "切换中文简历";
  } else {
    englishCV.style.display = "none";
    chineseCV.style.display = "block";
    button.innerHTML = "Show English CV";
  }
}
</script>
