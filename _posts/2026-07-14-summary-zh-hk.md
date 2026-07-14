---
layout: default
title: "Horizon Summary: 2026-07-14 (ZH-HK)"
date: 2026-07-14
lang: zh-hk
---

> 從 58 條內容中篩選出 22 條重要資訊。

---

1. [Apple SpeechAnalyzer API 與 Whisper 基準測試比較](#item-1) ⭐️ 8.0/10
2. [DOOMQL：完全由 SQLite 驅動嘅 Doom 風格遊戲](#item-2) ⭐️ 8.0/10
3. [防守者反用提示注入對付 AI 黑客](#item-3) ⭐️ 8.0/10
4. [世界模型：AI 模擬嘅承諾與限制](#item-4) ⭐️ 8.0/10
5. [控制意念，而非程式碼：Antirez 的軟體哲學](#item-5) ⭐️ 8.0/10
6. [以數據導向設計打造高效能解析器](#item-6) ⭐️ 8.0/10
7. [Git History 指令：被低估嘅強大工具](#item-7) ⭐️ 7.0/10
8. [唔開 Xcode 都可以建立同發佈 Apple App](#item-8) ⭐️ 7.0/10
9. [Sega CD《Silpheed》點樣用 FMV 模擬 3D 畫面](#item-9) ⭐️ 7.0/10
10. [Datasette 程式碼頻率圖表顯示 AI 代理的影響](#item-10) ⭐️ 7.0/10
11. [Codex 使用量激增 10 倍至 700 萬用戶，超越 Claude Code？](#item-11) ⭐️ 7.0/10
12. [美國警告俄羅斯國家黑客瞄準家用路由器](#item-12) ⭐️ 7.0/10
13. [蘋果起訴 OpenAI，指控前工程師竊取商業機密](#item-13) ⭐️ 7.0/10
14. [費曼反向灑水器謎題解開，延伸至「傻瓜灑水器」](#item-14) ⭐️ 7.0/10
15. [Lobste.rs 成功從 MariaDB 遷移至 SQLite](#item-15) ⭐️ 7.0/10
16. [早期 SunOS 在 NFS 之前嘅無碟工作站方案](#item-16) ⭐️ 7.0/10
17. [用 libdill 喺 C 語言實現 Go 風格並發](#item-17) ⭐️ 7.0/10
18. [函式庫應傳播錯誤，而非記錄日誌](#item-18) ⭐️ 7.0/10
19. [在純 IPv6 網絡上運行 IPv4 服務](#item-19) ⭐️ 7.0/10
20. [從編碼者到策展人：AI 重塑開發者角色](#item-20) ⭐️ 7.0/10
21. [唔好喺靜態文字元素上用 aria-label](#item-21) ⭐️ 7.0/10
22. [第二個中介軟體破壞 TypeScript 型別推斷](#item-22) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Apple SpeechAnalyzer API 與 Whisper 基準測試比較](https://get-inscribe.com/blog/apple-speech-api-benchmark.html) ⭐️ 8.0/10

Apple 在 WWDC 2025 推出的全新 SpeechAnalyzer API，已與 OpenAI 的 Whisper 及其前身進行基準測試，結果顯示在裝置端語音轉錄方面具有競爭力的速度和準確度。 此 API 可能顛覆依賴雲端模型的現有轉錄應用程式，因為它提供原生串流支援和裝置端處理，可能令第三方包裝程式變得過時。 基準測試將 SpeechAnalyzer 與 Whisper-Large-V2 及 Apple 先前的語音框架進行比較，在數學講座測試中顯示速度大幅提升，準確度僅略遜一籌。SpeechAnalyzer 亦支援串流轉錄，這是相對於批次處理模型的一大用戶體驗改進。

hackernews · get-inscribe · 7月13日 16:06 · [社群討論](https://news.ycombinator.com/item?id=48894752)

**背景**: Whisper 是 OpenAI 於 2022 年發布的開源自動語音識別（ASR）模型，以跨多種語言的穩健轉錄能力聞名。Apple 的 SpeechAnalyzer 於 WWDC 2025 推出，是一個模組化的裝置端語音識別 API，旨在現代化 Apple 的語音框架。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://www.callstack.com/blog/on-device-speech-transcription-with-apple-speechanalyzer">On-Device Speech Transcription with Apple SpeechAnalyzer and AI SDK</a></li>
<li><a href="https://www.argmaxinc.com/blog/apple-and-argmax">Apple SpeechAnalyzer and Argmax WhisperKit - Argmax</a></li>
<li><a href="https://news.ycombinator.com/item?id=48894752">Apple&#x27;s new SpeechAnalyzer API, benchmarked against Whisper and its predecessor | Hacker News</a></li>

</ul>
</details>

**社群討論**: 社群評論指出 Whisper 已非最先進模型，Nvidia 的 Nemotron 和 Parakeet、Mistral 的 Voxtral 以及 Cohere Transcribe 等新模型才是更好的基準。有用戶讚揚 SpeechAnalyzer 的串流支援是一大用戶體驗改進，亦有預測 Apple 將推出原生錄音應用程式，令付費的 Whisper 包裝程式變得過時。

**標籤**: `#speech recognition`, `#Apple`, `#benchmark`, `#ASR`, `#machine learning`

---

<a id="item-2"></a>
## [DOOMQL：完全由 SQLite 驅動嘅 Doom 風格遊戲](https://simonwillison.net/2026/Jul/13/doomql/#atom-everything) ⭐️ 8.0/10

開發者 Peter Gostev 創建咗 DOOMQL，一個以 SQLite 作為核心遊戲引擎嘅 Doom 風格第一人稱射擊遊戲，以 Python 終端腳本實現。遊戲嘅移動、碰撞、敵人、戰鬥同渲染完全透過 SQL 查詢處理，包括一個用遞歸 CTE 構建嘅完整光線追蹤器。 DOOMQL 展示咗 SQLite（傳統上係數據庫引擎）作為完整遊戲引擎嘅前所未有同創意用途，突破咗 SQL 可以做到嘅界限。呢個項目展示咗 SQLite 嘅力量同靈活性，啟發開發者探索數據庫技術嘅非傳統應用。 呢個遊戲係一個 Python 終端腳本，會建立一個 SQLite 數據庫檔案，可以用 Datasette 探索。渲染係由一個大型 SQL 查詢完成，使用遞歸 CTE 執行光線追蹤，為每個像素產生一行帶有 RGB 值嘅數據。

rss · Simon Willison · 7月13日 22:34

**背景**: SQLite 係一個輕量級、嵌入式嘅關聯式數據庫引擎，廣泛用於應用程式同流動裝置。DOOMQL 嘅靈感來自經典嘅 1993 年遊戲 Doom，一個以 3D 圖形同快節奏玩法聞名嘅標誌性第一人稱射擊遊戲。呢個項目將所有遊戲邏輯同渲染卸載到 SQL 查詢，徹底偏離傳統遊戲引擎，重新構想遊戲開發。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://github.com/petergpt/doomql">GitHub - petergpt/ doomql : A playable terminal FPS whose simulation...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Doom_game">Doom game</a></li>
<li><a href="https://www.sqlite.org/">SQLite Home Page</a></li>

</ul>
</details>

**標籤**: `#SQLite`, `#game development`, `#Python`, `#creative coding`

---

<a id="item-3"></a>
## [防守者反用提示注入對付 AI 黑客](https://arstechnica.com/security/2026/07/now-defenders-are-embracing-the-prompt-injection-too/) ⭐️ 8.0/10

Tracebit 的研究人員開發了一種名為「context bombing」的防禦技術，透過提示注入觸發 AI 黑客代理的內建安全拒絕機制，使其在造成損害前自動關閉。 這標誌著 AI 安全領域的範式轉移，將以往僅用於攻擊的技術轉變為針對自主黑客代理的主動防禦，有望大幅降低 AI 驅動的網絡攻擊威脅。 在五個模型及 152 次攻擊測試中，context bombing 成功降低了黑客代理的成功率。該技術透過在 AWS 環境中與機密資料並列植入特製提示，誘使代理自動關閉。

rss · Ars Technica AI · 7月13日 15:06

**背景**: 提示注入是一種漏洞，攻擊者透過精心設計的輸入覆蓋 LLM 的原始指令，常用於越獄或數據竊取。Context bombing 則重新利用此技術，嵌入防禦性提示以觸發模型自身的安全機制，使其拒絕執行有害操作。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://arstechnica.com/security/2026/07/now-defenders-are-embracing-the-prompt-injection-too/">Now, defenders are embracing the prompt injection, too</a></li>
<li><a href="https://github.com/SecureNexusLab/llm-prompt-injection-security-handbook">SecureNexusLab/llm-prompt-injection-security-handbook - GitHub Prompt Injection Attacks: Examples and Defences Prompt Injection | OWASP Foundation Now, defenders are embracing the prompt injection, too Prompt Injection &amp; Context Poisoning - emergentmind.com Prompt-Based Context Injection - emergentmind.com</a></li>

</ul>
</details>

**標籤**: `#AI security`, `#prompt injection`, `#cybersecurity`, `#defensive techniques`

---

<a id="item-4"></a>
## [世界模型：AI 模擬嘅承諾與限制](https://arstechnica.com/ai/2026/07/simulating-everything-sort-of-the-promise-and-limits-of-world-models/) ⭐️ 8.0/10

Ars Technica 發表咗一篇專題文章，邀請專家評論世界模型喺 AI 領域嘅現狀、能力同限制，指出主要參與者正專注於機械人、研究等特定應用場景，而非通用介面。 世界模型代表從簡單模式識別到能夠模擬物理同因果關係嘅 AI 系統嘅範式轉移，有望實現更安全嘅機械人訓練、更佳嘅自動駕駛同更逼真嘅影片生成。 文章指出，大型語言模型係先有聊天介面再尋找應用場景，而世界模型開發者則相反——從特定應用出發，但缺乏清晰嘅介面標準。此外，部分世界模型使用潛在動作，無法對應具體嘅現實世界移動，削弱咗佢哋作為真正世界模型嘅說服力。

rss · Ars Technica AI · 7月13日 11:00

**背景**: 世界模型係一種 AI 系統，能夠建立環境嘅內部表徵，並預測環境隨時間同動作而變化嘅情況。與傳統嘅分類或生成式 AI 唔同，世界模型模擬物理、物體互動同因果關係等動態。佢哋應用於機械人、自動駕駛同互動影片生成等領域。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_%28artificial_intelligence%29">World model (artificial intelligence)</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/world-models/">What Is a World Model? | NVIDIA Glossary</a></li>
<li><a href="https://rohitbandaru.github.io/blog/World-Models/">World Models | Rohit Bandaru</a></li>

</ul>
</details>

**標籤**: `#world models`, `#AI`, `#machine learning`, `#simulation`

---

<a id="item-5"></a>
## [控制意念，而非程式碼：Antirez 的軟體哲學](https://antirez.com/news/169) ⭐️ 8.0/10

Redis 創作者 Salvatore Sanfilippo（antirez）發表文章，主張軟體項目應透過控制背後的理念而非程式碼本身來管理，以達到更佳效果。 此觀點挑戰了嚴格程式碼擁有權及繁重流程執行等常見做法，為軟體工程管理提供更靈活、基於信任的替代方案。 Antirez 強調理念才是軟體品質的真正驅動力；透過清晰溝通、共享願景及輕量治理來控制理念，可減少摩擦並促進創新。

rss · Lobsters · 7月13日 15:35

**背景**: 這篇文章是軟體工程界關於流程與自主權平衡的長期討論之一。以 Redis 聞名的 Antirez 經常撰寫關於軟體開發實用智慧的文章。

**社群討論**: 文章連結的 Lobsters 討論中，有評論探討在大型團隊中控制理念的可行性；部分人讚揚此方法適合小型項目，但對其可擴展性提出質疑。

**標籤**: `#software engineering`, `#project management`, `#philosophy`, `#antirez`

---

<a id="item-6"></a>
## [以數據導向設計打造高效能解析器](https://arshad.fyi/writings/engineering-high-performance-parsers) ⭐️ 8.0/10

Arshad Yaseen 發表了一篇詳細文章，解釋如何應用數據導向設計原則，透過優化記憶體佈局和快取使用，大幅提升解析器效能。 這很重要，因為解析器效能對編譯器、數據處理管線等許多軟體系統至關重要，而數據導向設計提供了一種系統化方法，可實現數量級的加速。 文章強調，解析器的效能早在首次基準測試之前，就由其樹狀結構在記憶體中的佈局決定。文中涵蓋了結構陣列（struct-of-arrays）和快取友好遍歷等技術。

rss · Lobsters · 7月13日 13:20

**背景**: 數據導向設計是一種程式最佳化方法，專注於高效使用 CPU 快取，常用於遊戲開發。傳統物件導向設計可能導致快取局部性差，而數據導向設計則按存取模式組織數據，以減少快取未命中。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data-oriented_design">Data - oriented design - Wikipedia</a></li>
<li><a href="https://www.arshad.fyi/writings/engineering-high-performance-parsers">Engineering High - Performance Parsers with... - Arshad Yaseen</a></li>

</ul>
</details>

**標籤**: `#performance`, `#parsing`, `#data-oriented design`, `#software engineering`

---

<a id="item-7"></a>
## [Git History 指令：被低估嘅強大工具](https://lalitm.com/post/git-history/) ⭐️ 7.0/10

Lalit Maganti 嘅一篇網誌文章指出 \`git history\` 指令係一個強大但被低估嘅工具，用嚟瀏覽同理解提交歷史，並引發社群討論 Git 工作流程同替代工具如 \`jj\`。 呢個好重要，因為好多開發者只依賴基本 Git 指令，錯過咗可以大幅提升生產力同程式碼審查質素嘅進階功能。討論亦反映版本控制工作流程嘅持續演變。 \`git history\` 指令係 \`git log --graph --oneline --all\` 嘅別名，提供緊湊嘅提交圖形視覺化。社群留言指出可以用 \`git rebase --abort\` 同標籤安全地復原失敗嘅 rebase，而部分用戶更偏好 \`jj\` 嘅內置歷史編輯功能。

hackernews · Lobsters · 7月14日 00:57 · [社群討論](https://news.ycombinator.com/item?id=48901010)

**背景**: Git 係一個廣泛用於軟件開發嘅分散式版本控制系統。\`git log\` 指令顯示提交歷史，但好多開發者只用基本選項。\`git history\` 別名結合多個選項，顯示清晰嘅圖形化歷史視圖，尤其有助理解分支同合併。

**社群討論**: 社群討論普遍正面，用戶分享技巧同替代工具。部分用戶對互動式 rebase 感到恐懼，但其他人指出 \`git rebase --abort\` 等安全網。一個值得注意嘅反對意見係，有開發者傾向合併前壓縮所有提交，認為整理歷史無必要。

**標籤**: `#git`, `#version control`, `#developer tools`, `#workflow`

---

<a id="item-8"></a>
## [唔開 Xcode 都可以建立同發佈 Apple App](https://scottwillsey.com/building-and-shipping-mac-and-ios-apps-without-ever-opening-xcode/) ⭐️ 7.0/10

一篇詳細指南展示如何完全透過命令列工具（例如 xcodebuild 同 notarytool）嚟建立、簽署同發佈 Mac 同 iOS App，完全唔需要打開 Xcode 圖像界面。 呢種方法支援 AI 輔助編碼工作流程同持續整合管道，令開發者可以自動化 Apple 平台開發，唔需要手動操作 GUI，從而大幅加快迭代速度同減少人為錯誤。 呢個工作流程依賴 xcodebuild 進行編譯、notarytool 進行公證，以及 altool 或 Transporter 上傳到 App Store，全程唔需要啟動 Xcode。不過仍然需要一部 Mac 嚟執行呢啲工具，而且部分功能例如 SwiftUI 預覽係用唔到嘅。

hackernews · speckx · 7月13日 18:22 · [社群討論](https://news.ycombinator.com/item?id=48896665)

**背景**: Xcode 係 Apple 嘅整合開發環境（IDE），用嚟建立 Apple 平台嘅 App。傳統上開發者需要打開 Xcode 先可以編譯、簽署同上載 App。命令列工具例如 xcodebuild 已經存在多年，但通常只係輔助用途，而唔係完全取代。呢篇指南展示一個完全用 CLI 工具嘅完整流程，對喺終端環境運作嘅 AI 編碼代理尤其有用。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://aitoolly.com/ai-news/article/2026-07-14-how-to-build-and-ship-mac-and-ios-apps-without-ever-opening-the-xcode-gui">Build Mac and iOS Apps Without the Xcode GUI | AIToolly</a></li>
<li><a href="https://developer.apple.com/documentation/xcode/command-line-tools">Command-line tools | Apple Developer Documentation</a></li>
<li><a href="https://github.com/xtool-org/xtool">GitHub - xtool-org/xtool: Cross-platform Xcode replacement ...</a></li>

</ul>
</details>

**社群討論**: 留言者對喺冇沙箱嘅 Mac 上執行 AI 代理表示安全疑慮，提及憑證洩露嘅風險。有人推薦替代工具，例如用 xtool 喺 Linux 上開發，同埋用 Axiom 提供對 LLM 友善嘅工具。亦有其他人認為保持 Xcode 開啟並使用其 MCP 伺服器，比純 CLI 方法更快同功能更豐富。

**標籤**: `#iOS development`, `#macOS`, `#automation`, `#CI/CD`, `#Xcode alternatives`

---

<a id="item-9"></a>
## [Sega CD《Silpheed》點樣用 FMV 模擬 3D 畫面](https://fabiensanglard.net/silpheed/index.html) ⭐️ 7.0/10

Fabien Sanglard 發表咗一篇詳細嘅技術分析，講解 Sega CD 版《Silpheed》點樣利用預先渲染嘅全動態影像（FMV）同巧妙嘅工程設計，喺冇 3D 能力嘅硬件上模擬出 3D 圖像。 呢篇分析揭示咗 90 年代初開發者點樣突破硬件限制嘅創新技術，為懷舊遊戲愛好者同對有限環境感興趣嘅現代開發者提供咗寶貴見解。 遊戲從 CD-ROM 串流預先渲染嘅 3D 場景作為 FMV，然後喺上面疊加玩家控制嘅精靈，營造出實時 3D 嘅錯覺。Sega CD 嘅硬件縮放同旋轉 ASIC 有助於令效果更流暢。

hackernews · ibobev · 7月13日 14:52 · [社群討論](https://news.ycombinator.com/item?id=48893639)

**背景**: Sega CD 係 Sega Genesis 嘅 CD-ROM 附加配件，提供比卡帶大得多嘅儲存空間，但缺乏 3D 多邊形硬件。全動態影像（FMV）遊戲使用預先錄製嘅影片片段，而非實時渲染。《Silpheed》巧妙地將 FMV 背景同基於精靈嘅遊戲玩法結合，模擬出 3D 太空射擊遊戲嘅效果。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sega_CD">Sega CD - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Silpheed">Silpheed - Wikipedia</a></li>
<li><a href="https://retrosix.wiki/wiki/hardware-overview-sega-mega-cd">Hardware Overview (Sega Mega CD) - retrosix.wiki</a></li>

</ul>
</details>

**社群討論**: 留言者讚賞文章嘅深度，並分享咗相關嘅演示場景例子，例如將 Mega Drive 硬件推向極限嘅《Overdrive 2》。有人指出關於 Sega CD 音頻設置嘅小錯誤，顯示出參與者嘅技術審查精神。

**標籤**: `#retro gaming`, `#game development`, `#Sega CD`, `#technical deep-dive`, `#graphics`

---

<a id="item-10"></a>
## [Datasette 程式碼頻率圖表顯示 AI 代理的影響](https://simonwillison.net/2026/Jul/13/datasette-code-frequency/#atom-everything) ⭐️ 7.0/10

Simon Willison 分享了他開源項目 Datasette 的 GitHub 程式碼頻率圖表，顯示 2026 年程式碼新增和刪除出現驚人高峰，他將此歸因於編碼代理及 Opus 4.8、GPT-5.5、Fable 5 和 GPT-5.6 Sol 等先進 AI 模型。 這提供了具體的視覺證據，顯示 AI 輔助開發工具如何顯著提升開發者的生產力，尤其是對開源項目而言。它突顯了一個趨勢：編碼代理能夠實現以前不可行的快速迭代和大規模程式碼更改。 圖表顯示 2026 年某一週內新增 37,022 行、刪除 9,528 行，遠超自 2018 年項目開始以來的任何活動。貼文提到 Opus 4.8、GPT-5.5、Fable 5 和 GPT-5.6 Sol 等模型是關鍵推動因素。

rss · Simon Willison · 7月13日 21:45

**背景**: Datasette 是一個用於探索和發布數據的開源工具，用戶可將任何 CSV 或 SQLite 數據庫轉化為互動式網站和 API。GitHub 的程式碼頻率圖表以每週新增和刪除行數可視化開發活動歷史。編碼代理是能夠根據自然語言指令自主編寫、修改和除錯程式碼的 AI 系統。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://simonwillison.net/2026/jul/13/datasette-code-frequency/">datasette code - frequency chart on GitHub | Simon Willison’s Weblog</a></li>
<li><a href="https://github.com/simonw/datasette">GitHub - simonw/ datasette : An open source multi-tool for exploring and...</a></li>
<li><a href="https://datasette.io/">Datasette : An open source multi-tool for exploring and publishing data</a></li>

</ul>
</details>

**標籤**: `#AI-assisted development`, `#coding agents`, `#productivity`, `#open source`, `#data visualization`

---

<a id="item-11"></a>
## [Codex 使用量激增 10 倍至 700 萬用戶，超越 Claude Code？](https://www.latent.space/p/ainews-codex-usage-up-10x-in-6-months) ⭐️ 7.0/10

Codex 的使用量在六個月內增長超過 10 倍，達到 700 萬用戶，其中過去一天內增加了 100 萬，引發了與 Claude Code 採用情況的比較。 這種快速增長意味著 AI 編碼工具正變得主流，而 Codex 與 Claude Code 之間的競爭可能會推動開發者獲得更快創新。 OpenAI 於 2025 年 4 月 16 日發布了 Codex CLI 作為開源編碼代理，它在終端機中本地運行，並將語言模型與編碼任務連接起來。

rss · Latent Space · 7月14日 01:22

**背景**: Codex 是 OpenAI 的 AI 編碼代理，幫助開發者編寫和編輯程式碼、執行命令以及與檔案互動。Claude Code 是 Anthropic 的競爭性代理編碼工具。兩者都旨在通過自然語言互動加速軟體開發。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Codex_%28AI_agent%29">Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://openai.com/codex/">Codex in ChatGPT | AI Coding Agents for Software Engineering</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**社群討論**: 社群正在討論 Codex 的增長是自然增長還是受 OpenAI 營銷推動，以及 Claude Code 較低調的報告是否表明採用速度較慢或策略不同。

**標籤**: `#AI coding tools`, `#Codex`, `#Claude Code`, `#developer tools`, `#usage metrics`

---

<a id="item-12"></a>
## [美國警告俄羅斯國家黑客瞄準家用路由器](https://arstechnica.com/security/2026/07/the-us-government-warns-that-russia-state-hackers-are-coming-after-your-router/) ⭐️ 7.0/10

美國網絡安全與基礎設施安全局（CISA）發出警告，指俄羅斯國家支持的黑客正積極針對家用路由器，呼籲用戶採取防護措施。 這次警告突顯了國家級行為者利用被入侵的家用代理進行間諜活動和網絡攻擊的趨勢，對個人私隱和國家安全構成威脅。 警告特別指出，黑客利用住宅代理（即真實家用設備的 IP 地址）來隱藏惡意活動，令偵測更加困難。

rss · Ars Technica AI · 7月13日 21:03

**背景**: CISA 是美國負責網絡安全及基礎設施保護的聯邦機構。住宅代理通過真實的家用 IP 地址路由流量，常用於合法用途如網頁抓取，但亦可能被攻擊者濫用以逃避偵測。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cybersecurity_and_Infrastructure_Security_Agency">Cybersecurity and Infrastructure Security Agency - Wikipedia</a></li>
<li><a href="https://grokipedia.com/page/Residential_proxy">Residential proxy</a></li>

</ul>
</details>

**標籤**: `#cybersecurity`, `#routers`, `#CISA`, `#state-sponsored hacking`, `#Russia`

---

<a id="item-13"></a>
## [蘋果起訴 OpenAI，指控前工程師竊取商業機密](https://arstechnica.com/tech-policy/2026/07/apple-sues-openai-after-ex-engineer-allegedly-used-bug-to-steal-trade-secrets/) ⭐️ 7.0/10

蘋果公司對 OpenAI 提起訴訟，指控一名前蘋果工程師利用軟件漏洞竊取商業機密，並與 OpenAI 合謀使用這些機密。 這宗訴訟凸顯了主要科技公司在人工智能人才和知識產權方面的緊張局勢加劇，可能改變企業在競爭激烈的人工智能領域保護商業機密的方式。 訴訟指控該前工程師利用蘋果內部系統的漏洞存取並竊取專有資訊，然後與 OpenAI 分享。蘋果要求賠償並申請禁制令。

rss · Ars Technica AI · 7月13日 19:17

**背景**: 商業機密盜竊是科技行業中嚴重的法律問題，企業在研發上投入巨大。蘋果和 OpenAI 都是人工智能領域的領導者，此案凸顯了員工流動的風險以及加強安全措施的必要性。

**標籤**: `#Apple`, `#OpenAI`, `#trade secrets`, `#legal`, `#AI`

---

<a id="item-14"></a>
## [費曼反向灑水器謎題解開，延伸至「傻瓜灑水器」](https://arstechnica.com/science/2026/07/solution-to-feynmans-reverse-sprinkler-puzzle-also-applies-to-silly-sprinklers/) ⭐️ 7.0/10

2026 年 7 月發表的一項新研究證實了 2024 年的動量通量理論，該理論解釋了費曼反向灑水器的旋轉，並顯示相同理論也適用於其他形狀的「傻瓜灑水器」。 這解決了由理查德·費曼首次提出的數十年物理謎題，提供了對反向灑水器中水流角動量如何驅動旋轉的統一理解，對流體動力學和工程學具有啟示意義。 該研究使用不同形狀的定制灑水器進行實驗，驗證了動量通量理論，顯示旋轉方向和速度取決於進入裝置的水的淨角動量通量。

rss · Ars Technica AI · 7月13日 19:00

**背景**: 費曼反向灑水器謎題是問：如果水流入而非流出 S 形草坪灑水器，它會朝哪個方向旋轉？幾十年來，實驗結果互相矛盾。2024 年提出的動量通量理論將水的角動量通量視為旋轉的關鍵驅動力。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://physics.aps.org/articles/v17/15">Physics - Feynman ’s Reversed Sprinkler Puzzle Solved</a></li>
<li><a href="https://www.nyu.edu/about/news-publications/news/2026/july/researchers-put--silly-sprinklers--in-reverse-to-further-unravel.html">Researchers Put “Silly Sprinklers ” in Reverse to Further Unravel...</a></li>

</ul>
</details>

**標籤**: `#physics`, `#fluid dynamics`, `#research`

---

<a id="item-15"></a>
## [Lobste.rs 成功從 MariaDB 遷移至 SQLite](https://lobste.rs/s/ko1ji1/lobste_rs_is_now_running_on_sqlite) ⭐️ 7.0/10

Lobste.rs，一個基於 Rails 的社交新聞網站，已於上星期六成功將生產數據庫從 MariaDB 遷移至 SQLite，結果降低了 CPU 和記憶體使用量、減少了託管成本，並提升了網站響應速度。 這次遷移證明了 SQLite 能夠在生產環境中處理中等流量的網絡應用程式，挑戰了只有 MariaDB 或 PostgreSQL 等客戶端-伺服器數據庫才適合此類工作負載的假設。 遷移過程包括自訂的數據庫遷移腳本、兩次失敗的部署嘗試，以及第三次最終成功部署。該網站在星期一流量高峰期間經歷了「平靜的星期一」，沒有出現任何問題。

rss · Lobsters · 7月13日 20:03

**背景**: Lobste.rs 是一個類似 Hacker News 的社區運作連結聚合網站，使用 Ruby on Rails 構建。它最初使用 MariaDB，但由於 K1 收購後對數據庫未來的擔憂，促使團隊探索替代方案，最終選擇了 SQLite。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://medium.com/@peymaan.abedinpour/mariadb-vs-mysql-vs-postgresql-vs-sqlite-a-comprehensive-comparison-for-web-applications-0523cc3bc9d8">MariaDB vs MySQL vs PostgreSQL vs SQLite ... | Medium</a></li>
<li><a href="https://calvin.my/posts/migrating-a-rails-app-from-mysql-to-sqlite-database">Migrating a Rails App from MySQL to SQLite database</a></li>

</ul>
</details>

**社群討論**: Lobste.rs 上的社區討論氣氛正面，用戶注意到這項技術成就和幽默的「平靜的星期一」評論。部分用戶詢問具體的遷移挑戰和性能比較。

**標籤**: `#SQLite`, `#Rails`, `#database migration`, `#web performance`

---

<a id="item-16"></a>
## [早期 SunOS 在 NFS 之前嘅無碟工作站方案](https://utcc.utoronto.ca/~cks/space/blog/solaris/SunOSDisklessWithoutNFS) ⭐️ 7.0/10

一篇歷史技術文章揭示，早期 SunOS 使用名為 Network Disk \(nd\) 嘅自訂協定嚟支援無碟工作站，直到 1989 年左右 SunOS 4.1.x 先改用 NFS。 呢篇文章揭示咗一段鮮為人知但影響深遠嘅系統歷史，展示 Sun 喺 NFS 出現之前點樣解決關鍵問題。對理解網絡儲存同無碟運算嘅演變好重要。 nd 協定受限於 SunOS 每個物理磁碟最多八個分割區嘅限制，影響咗無碟工作站嘅配置。呢個協定喺 SunOS 3.5 嘅 man page 有記載，並已由開源項目 ndd 逆向工程重現。

rss · Lobsters · 7月13日 15:23

**背景**: 1980 年代，Sun Microsystems 銷售無碟工作站，呢啲工作站完全經由網絡啟動同運作。喺 NFS（網絡檔案系統）成為標準之前，Sun 開發咗一個專有協定叫 Network Disk \(nd\)，用嚟提供遠端區塊級磁碟存取。咁樣無碟客戶端就可以好似有本地儲存咁讀寫磁碟區塊。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://www.osnews.com/story/145511/how-early-sunos-did-diskless-workstations-before-nfs/">How early SunOS did diskless workstations before NFS – OSnews</a></li>
<li><a href="https://github.com/senjan/ndd">GitHub - senjan/ndd: ndd is a Sun&#x27;s Network Disk (ND) protocol ...</a></li>

</ul>
</details>

**社群討論**: Lobste.rs 嘅討論（文章中有連結）可能包含技術懷舊同早期 SunOS 用家嘅見解。不過，輸入中冇提供具體留言。

**標籤**: `#SunOS`, `#diskless workstations`, `#NFS`, `#history`, `#systems`

---

<a id="item-17"></a>
## [用 libdill 喺 C 語言實現 Go 風格並發](https://antonz.org/concurrency-in-c/) ⭐️ 7.0/10

一篇文探討用 libdill 庫喺 C 語言實現類似 goroutine 嘅並發原語，展示咗帶有 channel 同 select 陳述式嘅結構化並發。 呢個方法將 Go 優雅嘅並發模型帶到 C 語言，令系統程式設計師可以寫出更簡單、更安全嘅並發代碼，同時唔會犧牲效能。 Libdill 提供咗模仿 Go 嘅 goroutine 同 channel 嘅協程同 channel，但係有明確嘅資源管理同結構化並發原則。

rss · Lobsters · 7月13日 17:59

**背景**: Go 嘅並發模型使用 goroutine（輕量級線程）同 channel 進行通訊，令並發程式設計更容易。Libdill 係一個 C 庫，實現咗類似嘅原語，令 C 開發者可以使用結構化並發模式。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://sustrik.github.io/libdill/index.html">libdill</a></li>
<li><a href="https://steemit.com/programming/@boucaron/libmill-and-libdill">libmill and libdill — Steemit</a></li>

</ul>
</details>

**社群討論**: Lobste.rs 嘅討論強調咗結構化並發喺 C 語言嘅價值，有啲留言指出 libdill 嘅成熟度，亦有啲討論咗同其他並發庫相比嘅取捨。

**標籤**: `#concurrency`, `#C`, `#Go`, `#systems programming`

---

<a id="item-18"></a>
## [函式庫應傳播錯誤，而非記錄日誌](https://lobste.rs/s/v3avrp/should_libraries_log_propagate_errors) ⭐️ 7.0/10

一位開發者在 Lobsters 上質疑在函式庫內部記錄錯誤的常見做法，認為函式庫應該傳播錯誤，讓應用程式處理日誌記錄，引發了關於設計取捨的討論，特別是在 Go 的 slog 套件的背景下。 這次討論突顯了軟體工程中的一個基本設計矛盾：函式庫應該為了方便而記錄錯誤，還是為了靈活性而傳播錯誤。結果會影響開發者如何構建可靠且可維護的系統，特別是在 Go 生態系統中，slog 正成為標準的日誌記錄介面。 作者驚訝地發現，許多生態系統優先考慮在函式庫中記錄日誌，甚至讓靜音日誌成為一項重要任務。他們認為錯誤應該被傳播和豐富，日誌記錄留給應用層，這與 Go 的 slog 設計一致，後者允許向日誌記錄添加上下文。

rss · Lobsters · 7月13日 21:43

**背景**: 在軟體開發中，函式庫是可重複使用的程式碼模組，提供特定功能。錯誤處理和日誌記錄是橫切關注點：函式庫可以自行記錄錯誤，或將錯誤返回給調用應用程式。Go 的 slog 套件提供了一個結構化日誌記錄介面，可通過處理器進行自訂，讓應用程式控制日誌輸出和級別。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://betterstack.com/community/guides/logging/logging-in-go/">Logging in Go with Slog : The Ultimate Guide | Better Stack Community</a></li>
<li><a href="https://stackoverflow.com/questions/77304845/how-to-log-errors-with-log-slog">go - How to log errors with `log/ slog ` - Stack Overflow</a></li>
<li><a href="https://pkg.go.dev/log/slog">slog package - log/ slog - Go Packages</a></li>

</ul>
</details>

**社群討論**: Lobsters 上的討論反映了意見分歧：一些人同意函式庫不應記錄日誌，理由是關注點分離和靈活性；而另一些人則指出，在函式庫中記錄日誌對於除錯和監控可能很實用，尤其是當錯誤不易傳播時。這場辯論強調了正確的方法取決於函式庫的目的和受眾。

**標籤**: `#error handling`, `#logging`, `#software design`, `#Go`

---

<a id="item-19"></a>
## [在純 IPv6 網絡上運行 IPv4 服務](https://labs.ripe.net/author/remco-van-mook/a-farewell-to-arps-ipv4-service-on-ipv6-only-networks/) ⭐️ 7.0/10

RIPE Labs 發表了一篇文章，探討在純 IPv6 網絡上提供 IPv4 服務的方法，以應對從 IPv4 過渡到 IPv6 的挑戰。 這很重要，因為它為網絡營運商提供了在遷移到純 IPv6 基礎設施時保持 IPv4 服務兼容性的實用方法，這對最終全球採用 IPv6 至關重要。 該文章可能討論了 NAT64/DNS64、464XLAT 或其他過渡機制，這些技術允許僅支援 IPv4 的應用程式在沒有原生 IPv4 支援的網絡上運行。

rss · Lobsters · 7月13日 18:47

**背景**: IPv4 地址幾乎耗盡，推動了 IPv6 的採用。然而，許多舊有服務仍然依賴 IPv4。雙協議棧、隧道和翻譯等過渡機制允許共存，並最終遷移到純 IPv6 網絡。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/List_of_IPv6_transition_mechanisms">List of IPv6 transition mechanisms - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/computer-networks/transition-from-ipv4-to-ipv6-address/">Transition From IPv4 to IPv6 Address - GeeksforGeeks</a></li>
<li><a href="https://www.geeksforgeeks.org/computer-networks/ipv6-transition-mechanisms/">IPv6 Transition Mechanisms: 6to4, Teredo, ISATAP</a></li>

</ul>
</details>

**標籤**: `#IPv6`, `#IPv4`, `#networking`, `#transition`, `#ARPs`

---

<a id="item-20"></a>
## [從編碼者到策展人：AI 重塑開發者角色](https://staltz.com/from-coder-to-curator) ⭐️ 7.0/10

André Staltz 提出，開發者應從撰寫程式碼轉變為策展 AI 生成的程式碼，強調未來軟體工程需要的新技能組合。 這種轉變可能重新定義軟體工程專業，要求開發者專注於監督、品質保證和倫理考量，而非手動編碼。 Staltz 認為，隨著 AI 編碼工具進步，手動編碼的價值下降，而評估、改進和整合 AI 輸出的能力變得至關重要。

rss · Lobsters · 7月14日 02:29

**背景**: GitHub Copilot 和 ChatGPT 等 AI 輔助編碼工具迅速發展，讓開發者能透過自然語言提示生成程式碼。這引發了關於人類程式設計師在日益自動化的開發過程中未來角色的討論。

**標籤**: `#software engineering`, `#AI`, `#developer roles`, `#future of coding`

---

<a id="item-21"></a>
## [唔好喺靜態文字元素上用 aria-label](https://benmyers.dev/blog/dont-use-aria-label-on-static-text-elements/) ⭐️ 7.0/10

Ben Myers 喺 2024 年發表文章，提醒開發者唔好喺 div、span 等靜態文字元素上用 aria-label 或 aria-labelledby，因為咁會干擾屏幕閱讀器嘅朗讀，導致無障礙問題。 呢個建議糾正咗網頁開發者常見嘅 ARIA 標籤誤用，避免令屏幕閱讀器使用者更難存取內容。跟從呢個指引可以提升網頁無障礙程度，符合 WCAG 最佳實踐。 文章指明 aria-label 只應該用喺互動元素或者有明確角色嘅元素上，而唔係靜態文字。如果需要為靜態文字提供無障礙名稱，可以考慮用 aria-labelledby 或者可見文字。

rss · Lobsters · 7月13日 15:29

**背景**: ARIA（Accessible Rich Internet Applications）屬性例如 aria-label 係為咗提供替代標籤，增強屏幕閱讀器使用者嘅無障礙體驗。但係如果將佢哋用喺靜態文字元素上，可能會覆蓋元素本身嘅文字內容，令屏幕閱讀器忽略可見文字而只讀標籤，造成混淆或者資訊唔完整。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://web.archive.org/web/20241230231954/https://benmyers.dev/blog/dont-use-aria-label-on-static-text-elements/">Don’t Use aria -label on Static Text Elements | Ben Myers</a></li>
<li><a href="https://andycarter.dev/blog/why-aria-label-can-be-bad-for-accessibility">Why aria - label can be bad for accessibility – Andy Carter</a></li>

</ul>
</details>

**標籤**: `#accessibility`, `#web development`, `#ARIA`, `#best practices`

---

<a id="item-22"></a>
## [第二個中介軟體破壞 TypeScript 型別推斷](https://www.inngest.com/blog/adding-a-second-middleware-broke-our-typescript-types) ⭐️ 7.0/10

Inngest 發表了一篇詳細的網誌，解釋在 TypeScript 應用程式中加入第二個中介軟體如何悄悄地破壞型別推斷，並提供實用的解決方案。 這個問題影響許多在 TypeScript 中使用中介軟體模式的開發者，因為型別推斷失敗可能導致難以察覺的執行期錯誤。該文章為建立型別安全的中介軟體鏈提供了寶貴見解。 問題源於 TypeScript 在組合多個中介軟體函數時無法正確推斷型別，經常導致 \`any\` 型別。該文章用具體程式碼範例展示問題，並提供使用明確型別註解或重構中介軟體組合的解決方法。

rss · Lobsters · 7月13日 21:28

**背景**: 中介軟體是網頁框架中常見的模式，透過串聯函數來處理請求。TypeScript 的型別推斷通常對單一中介軟體運作良好，但多個中介軟體的組合可能混淆型別系統，導致型別安全喪失。

<details><summary>參考連結</summary>
<ul>
<li><a href="https://www.inngest.com/blog/adding-a-second-middleware-broke-our-typescript-types">Adding a second middleware broke our typescript types</a></li>
<li><a href="https://www.typescriptlang.org/docs/handbook/type-inference.html">TypeScript: Documentation - Type Inference</a></li>
<li><a href="https://middy.js.org/docs/writing-middlewares/with-typescript">With TypeScript | Middy.js</a></li>

</ul>
</details>

**社群討論**: 在 Lobsters 上，評論者確認了這個問題，並分享類似的中介軟體型別推斷經驗。有人建議使用 branded types 或明確型別斷言作為替代修復，其他人則討論不同方法的取捨。

**標籤**: `#TypeScript`, `#middleware`, `#type inference`, `#software engineering`

---