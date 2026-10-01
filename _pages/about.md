---
permalink: /
title: "About"
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
- 2025.04 - Present: Ph.D., Department of Computer Science and Engineering, Toyohashi University of Technology 
- 2023.04 - 2025.03: M.E., Department of Computer Science and Engineering, Toyohashi University of Technology 
- 2021.04 - 2023.03: B.E., Department of Computer Science and Engineering, Toyohashi University of Technology
- 2016.04 - 2021.03: Associate Degree, Department of Intelligent Systems Engineering, National Institute of Technology, Ichinoseki College


Work Experience
------
- 2023.09 - Present: Collaborative research, NTT Communication Science Laboratories
- 2023.01 - 2025.09: Internship, Poetics Inc.  
- 2024.08 - 2024.08: Research Assistant, National Institute of Advanced Industrial Science and Technology (AIST)
- 2023.08 - 2023.09: Research Intern, NTT Human Informatics Laboratories


Awards
------
- Student Poster Award, Speech Committee on Sound Symposium, June 2024
- 1st Place, INTERSPEECH Speech Accessibility Project Challenge, Feb 2025  


Grants
------
- 2025.04 - 2028.03: TUT-DC Fellowship (JST-SPRING)

</div>

<div data-lang-content="ja" markdown="1" hidden>

豊橋技術科学大学 音声言語処理研究室（北岡研究室）に所属する博士後期課程の学生です。 \\
音声処理、特に音声認識に興味があります。


学歴
------
- 2025.04 - 現在: 豊橋技術科学大学 工学研究科 情報・知能工学専攻 博士後期課程在学
- 2023.04 - 2025.03: 豊橋技術科学大学 工学研究科 情報・知能工学専攻 博士前期課程 修了 
- 2021.04 - 2023.03: 豊橋技術科学大学 工学部 情報・知能工学課程 卒業
- 2016.04 - 2021.03: 一関工業高等専門学校 制御情報工学科 卒業


職歴
------
- 2023.09 - 現在: NTTコミュニケーション科学基礎研究所, 共同研究
- 2023.01 - 2025.09: 株式会社Poetics, インターンシップ
- 2024.08 - 2024.08: 産業技術総合研究所 知的メディア処理研究チーム, リサーチアシスタント
- 2023.08 - 2023.09: NTT人間情報研究所, インターンシップ


受賞等
------
- 学生優秀ポスター発表賞, 音学シンポジウム 音声研究会, 2024年6月
- 1位, INTERSPEECH Speech Accessibility Project Challenge, 2025年2月


助成
------
- 2025.04 - 2028.03: TUT-DC Fellowship (JST-SPRING)


<!-- 資格
------
- 情報セキュリティマネジメント試験
- 基本情報技術者試験  -->


</div>

<style>
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

    function setLanguage(language) {
      buttons.forEach(function (button) {
        var active = button.getAttribute("data-lang-switch") === language;
        button.classList.toggle("is-active", active);
        button.setAttribute("aria-pressed", active ? "true" : "false");
      });

      contents.forEach(function (content) {
        content.hidden = content.getAttribute("data-lang-content") !== language;
      });
    }

    buttons.forEach(function (button) {
      button.addEventListener("click", function () {
        setLanguage(button.getAttribute("data-lang-switch"));
      });
    });
  })();
</script>
