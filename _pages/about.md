---
permalink: /
title: "About"
description: "Keigo Hojo is a Ph.D. student at Toyohashi University of Technology, researching automatic speech recognition and speech processing."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<div class="language-switcher" role="group" aria-label="Language selector">
  <button type="button" class="language-switcher__button is-active" data-lang-switch="en" aria-pressed="true">English</button>
  <button type="button" class="language-switcher__button" data-lang-switch="ja" aria-pressed="false">日本語</button>
</div>

<div data-lang-content="en" markdown="1">

I am a Ph.D. student in the Department of Computer Science and Engineering at Toyohashi University of Technology, supervised by Prof. Norihide Kitaoka.  
I'm interested in speech processing, deep learning, and automatic speech recognition.  


Education
------
- <span class="date-range">2025.04 - Present</span> : Ph.D., Department of Computer Science and Engineering, Toyohashi University of Technology
- <span class="date-range">2023.04 - 2025.03</span> : M.E., Department of Computer Science and Engineering, Toyohashi University of Technology
- <span class="date-range">2021.04 - 2023.03</span> : B.E., Department of Computer Science and Engineering, Toyohashi University of Technology
- <span class="date-range">2016.04 - 2021.03</span> : Associate Degree, Department of Intelligent Systems Engineering, National Institute of Technology, Ichinoseki College


Work Experience
------
- <span class="date-range">2026.11 - Present</span> : Sony Group Corporation, Graduate Internship
- <span class="date-range">2024.08 - 2024.08</span> : National Institute of Advanced Industrial Science and Technology (AIST), Research Assistant
- <span class="date-range">2023.08 - 2023.09</span> : NTT Human Informatics Laboratories, Research Internship
- <span class="date-range">2023.01 - 2025.09</span> : Internship, Poetics Inc.
- <span class="date-range">2022.09 - 2025.03</span> : NTT Communication Science Laboratories, Collaborative research


Awards
------
- Student Poster Award, Speech Committee on Sound Symposium, June 2024
- 1st Place, INTERSPEECH Speech Accessibility Project Challenge, Feb 2025  


Grants
------
- <span class="date-range">2027.04 - 2029.03</span> : JSPS Research Fellow (DC2)
- <span class="date-range">2025.04 - 2027.03</span> : TUT-DC Fellowship (JST-SPRING)
- <span class="date-range">2023.04 - 2025.03</span> : Repayment Exemption for Outstanding Achievements, JASSO

</div>

<div data-lang-content="ja" markdown="1" hidden>

豊橋技術科学大学 音声言語処理研究室（北岡研究室）に所属する博士後期課程の学生です。 \\
音声処理、特に音声認識に興味があります。


学歴
------
- <span class="date-range">2025.04 - 現在</span> : 豊橋技術科学大学 工学研究科 情報・知能工学専攻 博士後期課程在学
- <span class="date-range">2023.04 - 2025.03</span> : 豊橋技術科学大学 工学研究科 情報・知能工学専攻 博士前期課程 修了
- <span class="date-range">2021.04 - 2023.03</span> : 豊橋技術科学大学 工学部 情報・知能工学課程 卒業
- <span class="date-range">2016.04 - 2021.03</span> : 一関工業高等専門学校 制御情報工学科 卒業


職歴
------
- <span class="date-range">2026.11 - 現在</span> : ソニーグループ会社, 長期有給インターンシップ
- <span class="date-range">2024.08 - 2024.08</span> : 産業技術総合研究所 知的メディア処理研究チーム, リサーチアシスタント
- <span class="date-range">2023.08 - 2023.09</span> : NTT人間情報研究所, インターンシップ
- <span class="date-range">2023.01 - 2025.09</span> : 株式会社Poetics, インターンシップ
- <span class="date-range">2022.09 - 2025.03</span> : NTTコミュニケーション科学基礎研究所, 共同研究


受賞等
------
- 学生優秀ポスター発表賞, 音学シンポジウム 音声研究会, 2024年6月
- 1位, INTERSPEECH Speech Accessibility Project Challenge, 2025年2月


助成
------
- <span class="date-range">2027.04 - 2029.03</span> : 日本学術振興会特別研究員-DC2
- <span class="date-range">2025.04 - 2027.03</span> : TUT-DC Fellowship (JST-SPRING)
- <span class="date-range">2023.04 - 2025.03</span> : 日本学生支援機構（JASSO）第一種奨学金 特に優れた業績による返還免除


<!-- 資格
------
- 情報セキュリティマネジメント試験
- 基本情報技術者試験  -->


</div>

<style>
  .date-range {
    display: inline-block;
    width: var(--date-range-width, auto);
    text-align: left;
    white-space: nowrap;
    font-variant-numeric: tabular-nums;
  }

  .language-switcher {
    display: flex;
    gap: 0.5rem;
    margin-bottom: 1.5rem;
  }

  .language-switcher__button {
    border: 1px solid #7a8288;
    border-radius: 4px;
    background: transparent;
    color: inherit;
    cursor: pointer;
    font: inherit;
    line-height: 1.2;
    padding: 0.35rem 0.75rem;
  }

  .language-switcher__button.is-active {
    background: #494e52;
    border-color: #494e52;
    color: #fff;
  }
</style>

<script>
  (function () {
    var buttons = document.querySelectorAll("[data-lang-switch]");
    var contents = document.querySelectorAll("[data-lang-content]");

    function alignDateRanges() {
      contents.forEach(function (content) {
        if (content.hidden) return;

        var dates = content.querySelectorAll(".date-range");
        var maxWidth = 0;
        content.style.removeProperty("--date-range-width");

        dates.forEach(function (date) {
          maxWidth = Math.max(maxWidth, date.getBoundingClientRect().width);
        });

        if (maxWidth > 0) {
          content.style.setProperty("--date-range-width", Math.ceil(maxWidth) + "px");
        }
      });
    }

    function setLanguage(language) {
      buttons.forEach(function (button) {
        var active = button.getAttribute("data-lang-switch") === language;
        button.classList.toggle("is-active", active);
        button.setAttribute("aria-pressed", active ? "true" : "false");
      });

      contents.forEach(function (content) {
        content.hidden = content.getAttribute("data-lang-content") !== language;
      });

      alignDateRanges();
    }

    buttons.forEach(function (button) {
      button.addEventListener("click", function () {
        setLanguage(button.getAttribute("data-lang-switch"));
      });
    });

    alignDateRanges();
    window.addEventListener("resize", alignDateRanges);
    if (document.fonts) {
      document.fonts.ready.then(alignDateRanges);
    }
  })();
</script>
