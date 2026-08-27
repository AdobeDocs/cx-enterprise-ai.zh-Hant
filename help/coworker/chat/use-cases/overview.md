---
description: 瀏覽同事聊天使用案例和範例提示，依資料深入分析、受眾、歷程和平台操作的區域進行整理。
title: 同事聊天使用案例
feature_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 6d2ed4b1ab956faf844ab3f517b52c6a2bd2b2dd
workflow-type: tm+mt
source-wordcount: 3344
ht-degree: 7%

---

# 同事聊天使用案例{#use-cases}

Co-worker Chat可讓您使用自然語言來查詢、分析和處理您的[!DNL Experience Platform]資料，而不需手動導覽多個UI或撰寫查詢。 此頁面提供從業人員最仰賴的使用案例目錄，並按工作區域整理：資料深入分析、對象、歷程、基本元素和沙箱工具。 每個專案都包含它叫用的技能、它使用的應用程式，以及範例提示，您可以複製、調整您自己的資料，並透過對話調整內容。

>[!NOTE]
>
>即將推出：
>
>透過CX Enterprise Co-worker提供全新的AEM代理功能，可協助您更快完成更多工作。
>
>所有符合資格的客戶將可輪流在Co-worker中存取Adobe Experience Manager代理功能。
>
>另請參閱AEM中的[AI - AEM代理功能概觀](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/overview)。

## 品牌體驗

### 體驗生產 — Sites使用案例

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| 更新AEM頁面 | 執行更新、移除、取代或新增內容元素等動作，讓體驗保持精確且最新。 輸入內容可以是自然語言或視覺化註解，例如PDF或熒幕擷圖。 | `aem-sites-pages-update` | Adobe Experience Manager (AEM) | 在&lt;URL>將標題更新為Hello World<br><br>在&lt;URL>上將「參加我們的咖啡測驗」按鈕變更為更吸引人的版本<br><br>根據附加的<br><br>在&lt;URL>上更新&lt;URL>我想在頁面底部新增新的Teaser區段，說明我們在8月份進行的促銷活動，購買咖啡機並免費取得2袋咖啡。 同時尋找喝咖啡的朋友的影像，並在Teaser中使用 |
| 大量更新AEM | 同時跨多個頁面執行大量動作，例如移除、取代或新增內容元素，以保持體驗正確且最新。 | `aem-sites-pages-bulkreplace` | Adobe Experience Manager (AEM) | 在&lt;aem path>上，將包含複製「MyBarista\」的所有頁面更新為「BrewPass」 |
| 從圖表移至視覺內容片段 | 使用自然語言，直接從Figma將設計匯入Adobe Experience Manager。 此技能會自動建立所需的內容模型、內容片段、資產和視覺效果範本，讓業務使用者在數分鐘內從設計移至網頁就緒內容，無需手動設定。 | `aem-sites-visualcontentfragments-create` | Adobe Experience Manager (AEM) | 從&lt;Figma_URL>匯入 |

**相關資訊**

* [AEM中的代理程式功能：品牌體驗 — 體驗生產 — 網站](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-sites)

### 體驗生產 — Forms使用案例

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| 建立表單 | 從純語言說明、附加的簡報、影像或PDF產生新的調適型表單 | `aem-forms-adaptiveform-create` | Adobe Experience Manager (AEM) | 「建立員工入門表單」<br><br>「使用附加的簡報（影像或pdf）建立表單」<br><br>「建立&lt;form type>最適化表單」 |
| 編輯/更新表單 | 修改現有表單 — 新增/編輯欄位、調整簡單版面、設定提交動作，或套用附加准則檔案的變更 | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) | 「在名字欄位下方新增中間名欄位」<br><br>「將名字和姓氏欄位放在2欄佈局中，50/50」<br><br>「設定表單以傳送資料到REST端點」<br><br>「更新此表單以符合附加的准則檔案」<br><br>「在&lt;現有欄位>欄位下方新增&lt;欄位名稱>欄位」 |
| 新增商業邏輯 | 建立簡單規則，例如根據其他欄位的值顯示或隱藏欄位 | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) | 「僅在員工型別為承包商時顯示公司欄位」<br><br>「僅在&lt;其他欄位>為&lt;值>時顯示&lt;欄位>欄位」 |
| 內嵌表單 | 將現有或新建立的表單放置在指定的AEM Sites頁面上（僅支援Edge Delivery Services頁面） | `aem-forms-adaptiveform-embed` | Adobe Experience Manager (AEM) | &quot;將此表單內嵌到我們網站的首頁上&quot;<br><br>&quot;將此表單內嵌到&lt;page path>&quot; |

**相關資訊**

* [AEM的代理程式功能：品牌體驗 — 體驗生產 — Forms](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-forms)

### 開發

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| 診斷和修復失敗的Cloud Manager管道 | 調查失敗的管道執行，找出根本原因，並產生修正（包含差異）以供審查 | `cloud-manager-pipeline-troubleshooting` | Adobe Experience Manager (AEM) | 「為什麼我的組建管道失敗？」<br><br>「建議修正我中斷的生產管道」 |
| 管理Cloud Manager管道 | 建立、執行和監視AEM Cloud Manager管道，包括記錄、成品、變數和設定 | `cloud-manager-pipeline-management` | Adobe Experience Manager (AEM) | 「列出方案12345的管道」<br><br>「為什麼我的開發管道執行失敗？」 |
| 管理Cloud Manager環境 | 建立、設定和維護AEM Cloud Manager環境，包括RDE、環境變數、記錄檔和備份 | `cloud-manager-environment-management` | Adobe Experience Manager (AEM) | 列出我的計畫12345環境&quot;<br><br>&quot;重設我的RDE&quot; |
| 管理Cloud Manager計畫 | 列出、檢查和刪除AEM Cloud Manager程式，包括其管道和環境 | `cloud-manager-program-management` | Adobe Experience Manager (AEM) | 「列出我的Cloud Manager程式」<br><br>「取得程式12345的詳細資料」 |
| 管理AEM版本更新排程 | 設定每日無訊息時間和無更新期間以進行自動維護，並檢視Adobe的全域程式碼凍結視窗 | `cloud-manager-release-management` | Adobe Experience Manager (AEM) | 「我目前的無訊息時間視窗是多少？」<br><br>「排程從12月20日至1月2日的無更新期間」 |

**相關資訊**

* [AEM的代理程式功能：品牌體驗 — 開發](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/development/use-cases)

### 入門 — AEM Assets使用案例

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| 引導式端對端上線 | 協調完整的入門生命週期、存放庫選擇、委派到資料夾、標籤、中繼資料、匯入和搜尋子技能（如果您不知道您需要的特定入門任務）。 | `aem-onboarding-workflow` | Adobe Experience Manager (AEM) Assets | 「將我們的團隊加入AEM Assets」<br><br>「帶我瞭解AEM DAM加入」 |
| 設計和建立資料夾階層 | 根據業務需求或CSV輸入，在AEM Assets （在`/content/dam`下）中建議並建立可擴充的資料夾結構。 | `aem-folder-management` | Adobe Experience Manager (AEM) Assets | 「建議我們生活方式行銷資產的資料夾結構」<br><br>「根據此CSV檔案建立資料夾」 |
| 設計和建立標籤 | 在`/content/cq:tags`下設計和建立控制標籤辭彙 — 名稱空間、階層標籤和批次標籤作業。 | `aem-tag-taxonomy` | Adobe Experience Manager (AEM) Assets | 「使用我們產品類別的名稱空間設計標籤分類法」<br><br>「從此CSV匯入標籤」<br><br>「在AEM中建立這些階層式標籤」 |
| 建立及指派中繼資料表單 | 從CSV、表格、需求檔案或說明設計並建立作者使用的自訂中繼資料表單（製作UI內容），然後選擇性地將其指派給資料夾。 | `aem-metadata-form` | Adobe Experience Manager (AEM) Assets | 「從這個欄位清單建立中繼資料表單」<br><br>「將此表單指派到`campaigns`資料夾」 |

**相關資訊**

* [AEM的代理功能：品牌體驗 — 入門](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/onboarding/use-cases)

## 內容顧問 — AEM Assets使用案例

### 內容探索

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| 依語意主題搜尋 | 使用AI支援的語意比對功能，依概念、心情或視覺主題尋找資產。 | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | 「尋找我晨間咖啡生活方式影像」 |
| 依自訂中繼資料搜尋 | 依自訂中繼資料欄位篩選資產（例如Coffee Blend、Brand、Roast Level）。 | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | 「尋找`Coffee Blend`為`Morning Muse`的資產」<br><br>「取得授權未過期的資產」<br><br>「尋找未設定行銷活動名稱的資產（屬性必須針對適當結果編制索引）。」 |
| 依核准狀態搜尋 | 根據核准狀態篩選資產。 例如，已核准、稽核中、已拒絕或缺少狀態。 | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | 「顯示`Campaign`資料夾中所有已核准的資產」 |
| 依資料夾/路徑搜尋 | 透過解譯參考AEM中資料夾名稱的自然語言提示來識別資產。 您只需在提示中提及資料夾，無需手動導覽存放庫，即可顯著減少尋找正確內容所需的點按次數。 | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | 「資料夾`WKND`中是否有任何svg」？<br><br>「在資料夾`WKND`中顯示在2025年11月1日之後修改的資產」 |

**相關資訊**

* [AEM的代理程式功能：內容顧問 — 內容探索](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/discovery/use-cases)

### 內容最佳化

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| 高解析度轉譯建立和通道最佳化的轉譯 | 以指定的解析度和品質等級產生資產的新轉譯，讓您無需手動編輯即可輕鬆準備通道就緒的變數。 您也可以根據平台特定需求量身打造轉譯，例如Instagram故事，確保資產自動符合格式、比例和品質准則。 | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) Assets | 「使用`80% quality`建立`2000px`轉譯為`JPEG`」<br><br>「為Instagram故事建立轉譯」 |
| 品牌覆蓋圖與複合圖產生 | 透過精確放置將促銷圖形、覆蓋圖或徽章套用至現有資產，可支援快速建立適用於行銷活動的複合專案。 | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) Assets | 「將含有`30%`折扣圖片的影像覆蓋在促銷橫幅上，從中心放置`100px`」 |
| 影像增強功能、背景色彩調整、方向轉換 | 套用視覺改善（銳利化影像）、取代背景顏色，以及執行方向轉換。 | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) Assets | 「將`PNG`的背景顏色變更為`#ff8932`」<br><br>「銳利化影像」<br><br>「水準映象影像」 |

**相關資訊**

* [AEM中的代理程式功能：內容警告器 — 內容最佳化](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/content-optimization/use-cases)

## 品牌控管

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| 指引和區段查閱 | 擷取詳細的品牌指引，依區段、市場或類別設定範圍 | enterprise-context | Adobe Experience Manager (AEM) | 「這個品牌的聲調准則是什麼？」<br>「列出健康情況垂直領域使用的索賠類別」 |
| 根據品牌准則評估內容 | 根據已設定的品牌檢查評估已發佈/編寫的頁面、文字區塊或影像 | aem治理 | Adobe Experience Manager (AEM) | 「根據SecurBank准則評估此登陸頁面」<br>「此標語是否通過我們的語調檢查？」 |
| 偵錯AEM許可權 | 偵錯/瞭解許可權原則、ACL和繼承規則。 | aem治理 | Adobe Experience Manager (AEM) | 「為何主體管理員可以在`https://author/`上寫入`/content/folder/us`？」<br>「為何無法在`https://author`上的`/content/dam`上取樣作者寫入」 |

**相關資訊**

* [AEM的代理程式功能：品牌控管](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-governance/use-cases)

## 資料深入分析

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| [提取CJA報告與量度](data-insights/analytics-chat.md) | 即時查詢CJA以提取量度、維度、區段和資料檢視 | `cja` | Customer Journey Analytics (CJA) | 「顯示過去30天的頁面檢視」 · 「在主資料檢視中列出排名最前的區段」 |
| 比較分析 | 並排比較不同管道、時段或區段的量度 | `cja-root-cause-analysis`, `cja`, `dx-api`, `knowledge-graph` | Customer Journey Analytics (CJA) | 「按管道月份比較每月收入」 · 「本季行動與桌上型電腦轉換看起來如何？」 |
| 行銷活動績效 | 測量在指定期間內行銷活動、管道和Web屬性的執行情形。 | `cja`, `dx-api`, `knowledge-graph` | | 「上個月我們的Acrobat網路行銷活動表現如何？」 |
| funnel分析 | 逐步瞭解每個階段都有流失的多步驟轉換漏斗 | `cja` | Customer Journey Analytics (CJA) | 「帶我瀏覽funnel結帳」 · 「顯示從PDP到購買的轉換funnel」 |
| 預測 | 根據歷史CJA資料預測未來的量度值 | `cja` | Customer Journey Analytics (CJA) | 「未來30天的預測工作階段」 · 「我們是否可望達成收入目標？」 |
| [根本原因分析](data-insights/root-cause-analysis.md) | 調查量度變更的原因：診斷下降、尖峰和異常 | `cja-root-cause-analysis` | Customer Journey Analytics (CJA) | 「為什麼上週轉換率下降？」 · 「是什麼導致1月15日的收入激增？」 |
| 執行摘要和KPI摘要 | 製作適合利害關係人的效能摘要、規範性建議和投影片組大綱 | `cja-executive-summary`, `cja-bacom-anomaly-tracker-v2`, `cja-cno-weekly-pulse`, `cja-reporting`, `cja`, `dx-api` | Customer Journey Analytics (CJA) | 「給我上個月的執行摘要」 · 「從本季的資料建立投影片投影片組大綱」 |
| [AA ↔ CJA資料驗證](data-insights/data-validation-aa-cja.md) | 在Adobe Analytics和Customer Journey Analytics之間比較、稽核及調解資料，尤其是從Adobe Analytics升級為Customer Journey Analytics時 | `aa-cja-validation`, `cja`, `dx-api` | ADOBE ANALYTICS + CJA | 「將我的AA報告套裝與CJA資料檢視進行比較」 · 「驗證AA與CJA之間的頁面檢視」 |
| 作業時間序列與因果分析 | 查詢和分析具有因果歸因的對象、資料集和歷程的歷史時間序列資料 | `operational-stats-causal-analysis` | 所有符合資格的應用程式 | 「顯示過去90天的對象人數趨勢」 · 「為什麼我的資料集列會計入3月3日的尖峰？」 |
| 建立自訂CJA技能 | 將分析模式轉換為可重複使用、且跨工作階段儲存的技能 | `cja-skill-creator` | Customer Journey Analytics (CJA) | 「將此每週收入分析轉換為可重複使用的技能」·「將此儲存為每月funnel報告的技能」 |

## 客群

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| [從自然語言建立對象](audiences/create-audience-from-natural-language.md) | 透過每個階段的使用者核准，策劃逐步的受眾建立 | `audience-creation-flow` | Real-Time CDP (RTCDP) | 「建立過去30天內購買的使用者受眾」 · 「為加州的高價值忠誠會員建立區段」 |
| 建置PQL定義 | 從XDM屬性、行為事件或現有對象中組合對象定義；支援彙總和時間範圍 | `segment-definition-assembly` | Real-Time CDP (RTCDP) | 「為檢視3個以上產品但未購買的使用者建立PQL」 · 「為我的事件條件新增7天時段」 |
| 搜尋和尋找對象 | 依ID、名稱、語意搜尋尋找對象；偵測重複專案並分析重疊 | `audience-search` | Real-Time CDP (RTCDP) | 「尋找所有忠誠受眾」 · 「我的『節日購物者』區段是否有重複專案？」 |
| 預估對象規模 | 使用Adobe Experience Platform預覽API搭配輪詢來預估PQL運算式的設定檔觸及率 | `audience-size-estimate` | Real-Time CDP (RTCDP) | 「此對象有多大？」 · 「此PQL運算式的預估觸及率」 |
| 對象人數瀑布 | 將PQL分解為子述詞，並顯示每個條件對最終對象規模的貢獻 | `audience-size-waterfall` | Real-Time CDP (RTCDP) | 「顯示此PQL的瀑布圖」 · 「劃分每個條件如何減少受眾」 |
| 探索用於定位的XDM欄位 | 依名稱、說明或資料值搜尋欄位；檢視欄位的使用位置和使用位置 | `field-discovery` | Real-Time CDP (RTCDP) | 「我可以使用哪些欄位來鎖定忠誠客戶？」 · 「尋找與購買記錄相關的欄位」 |
| 發佈/儲存對象 | 透過命名慣例和合規性檢查將受眾定義儲存至Experience Platform細分服務 | `audience-publish` | Real-Time CDP (RTCDP) | 「將此專案儲存為草稿」 · 「以『春季促銷買家』名稱發佈對象」 |

## 歷程

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| [從自然語言建立歷程](journeys/create-journey-from-natural-language.md) | 透過文字提示或上傳的影像/流程圖，在AJO中協調歷程建立 | `journey-create` | Adobe Journey Optimizer (AJO) | 「建立歡迎歷程，在註冊後傳送電子郵件、等待3天，然後傳送後續追蹤」 · 「從這個上傳的流程圖影像建立歷程」 |
| 分析歷程衝突 | 偵測使用中歷程之間的對象重疊、排程衝突及重複資料刪除問題 | `journey-analyze-conflict` | Adobe Journey Optimizer (AJO) | 「我的購物車放棄歷程是否與其他歷程衝突？」 · 「檢查我作用中歷程之間的受眾重疊」 |
| 分析歷程流失 | 識別客戶在歷程中下降的位置和原因，並偵測導致脫離參與的行為模式 | `journey-analyze-fallout` | Adobe Journey Optimizer (AJO) | 「在我的重新參與歷程中，人們在哪裡停下來？」 · 「歷程X中的哪些節點流失率最高？」 |
| 分析自訂動作錯誤 | 識別歷程中自訂動作失敗或錯誤率飆升的時間，並在失敗升級為更廣泛的中斷之前診斷根本原因 | `journey-analyze-custom-action` | Adobe Journey Optimizer (AJO) | 「為什麼自訂動作會在我的忠誠度註冊歷程中失敗？」 · 「在我的歡迎歷程中，顯示自訂動作ExternalPush的錯誤率。」 |
| [建立、編輯和管理忠誠度挑戰](journeys/create-loyalty-challenge.md) | 簡化並加速熟客方案管理 | `loyalty` | Adobe Journey Optimizer (AJO) | 「建立挑戰，鼓勵會員嘗試新的季節性飲品」 · 「以最高的會員流失率向我展示忠誠度挑戰。」 |

## 基本元素

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| 產品知識與檔案 | 從官方Adobe檔案中回答操作說明、概念、疑難排解和最佳作法問題 | `product-knowledge` | 所有符合資格的應用程式 | 「如何設定串流目的地？」 · 「批次和串流細分之間有何差異？」 |
| 查詢Experience Platform / Journey Optimizer實體 | 作為平台實體相關問題的主要入口點；視需要路由至KG、欄位探索或API | `operational-insights` | 所有符合資格的應用程式 | 「我有多少資料集？」 · 「顯示所有使用中的歷程」 · 「列出我的目的地」 |
| 知識圖查詢 | 透過單一SQL查詢的彙總計數、跨實體聯結、關係查閱和中繼資料探索 | `knowledge-graph` | 所有符合資格的應用程式 | 「哪些對象使用此資料集？」 · 「顯示結構描述和資料集之間的關係」 |
| Experience Platform / Journey Optimizer / Customer Journey Analytics API作業 | 提供直接API閘道，用於變更、即時狀態檢查以及不在知識圖形中的實體型別 | `cxo-api` | 所有符合資格的應用程式 | &quot;刪除資料集X&quot; · &quot;檢查批次擷取工作的狀態&quot; |
| 實體解析度和連結 | 使用語意和辭彙搜尋來解析對實際Experience Platform實體的實體提及，並探索XDM欄位 | `entity-linking` | Adobe Experience Platform | 「將『節日購物者』解析為實際受眾」 · 「尋找與購買記錄相關的我欄位」 |
| 管理自訂技能 | 儲存、修改或刪除使用者擁有的可重複使用技能，這些技能會跨工作階段存留 | `manage-skill` | 所有符合資格的應用程式 | 「將工作流程另存為技能」 · 「刪除我的每週報告技能」 · 「將此轉換為可重複使用的技能」 |
| 監控串流容量和違規情形 | 檢查沙箱間目前和歷史串流使用情況、容量和違規狀態 | `observability-streaming-capacity`, `observability-streaming-usage`, `observability-capacity-breaches` | Adobe Experience Platform | 「我目前的沙箱中資料流容量是多少？」 · 「我目前的沙箱在上星期是否超過容量限制？」 |
| [檢視健康情況檢查評估結果](https://experienceleague.adobe.com/en/docs/experience-platform/run-and-operate/health-checks/overview) | 檢視沙箱的最新健康情況檢查評估、深入研究失敗檢查，並檢視受影響的實體 | `rao-view-latest-health-checks-assessment` | Adobe Experience Platform | 「我的沙箱有什麼問題？」 · 「告訴我最新的健康情況檢查評估的相關資訊」 · 「自訂名稱空間說明檢查有哪些問題？」 |
| 修正健康情況檢查問題 | 在進行任何變更之前，只要您核准，即可直接從聊天中修正標幟的身分名稱空間、合併原則和結構描述問題 | `rao-remediate-identity-namespace-description`, `rao-remediate-merge-policy-duplicate-name`, `rao-remediate-missing-audit-field-group`, `rao-remediate-default-merge-policy-naming` | Adobe Experience Platform | 「修正身分名稱空間說明」 · 「修正重複的合併原則名稱」 · 「修正缺少稽核欄位群組的結構描述」 · 「修正預設的合併原則命名」 |

## 沙箱工具

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| [跨沙箱移動物件](/help/agents/sandbox-tooling.md) | 透過自動解析的相依性，順暢地跨沙箱移轉結構描述、受眾和其他物件設定 | `sandbox-tooling-workflow` | Adobe Experience Platform | 「將方案Luma忠誠會員白金從目前的沙箱移至生產沙箱」· 「將美國金級忠誠會員對象提升至階段」 |

## 客戶警報

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| 管理警報訂閱 | 透過自然語言對話檢視及管理警示訂閱。 | `alerts-subscribe` | Adobe Experience Platform | 「我訂閱了哪些警示？」<br><br>「訂閱此警示給我。」<br><br>「移除此警示的訂閱。」 |
| 檢閱警示活動 | 檢閱指定期間內的目前警示狀態和歷史警示活動。 | `alerts-list` | Adobe Experience Platform | 「過去24小時內發生了什麼事？」<br><br>「過去24小時內觸發了哪些警示？」<br><br>「顯示過去七天的作用中警示。」 |
| 識別週期性警報模式 | 分析警示歷史記錄，以識別經常觸發的警示型別和運作趨勢。 | `alerts-list` | Adobe Experience Platform | 「顯示前3個觸發的警示型別。」<br><br>「哪些警示型別本月發生頻率最高？」<br><br>「您在過去七天看到哪些警示模式？」 |
| 著重於高優先順序的問題 | 依嚴重程度篩選警示活動，以排定調查工作的優先順序。 | `alerts-list` | Adobe Experience Platform | 「僅顯示高嚴重度警示。」<br><br>「本週觸發了哪些嚴重性警示？」<br><br>「顯示過去30天的嚴重性警示。」 |
| 瞭解警報的影響半徑 | 識別受警示影響最大的物件，並決定應從何處開始調查。 | `alerts-list` | Adobe Experience Platform | 「前5個受影響的物件為何？」<br><br>「哪些物件與最高嚴重性警示相關？」 |
| 將警示型別連線到受影響的物件 | 分析警示型別與受影響資源之間的關係。 | `alerts-list` | Adobe Experience Platform | 「哪些警報型別最常影響此資料集？」<br><br>「顯示警報型別與受影響物件之間的關係。」<br><br>「哪些警報型別最常影響最受影響的物件？」 |
| 將焦點放在我的警報上 | 分析您訂閱並負責監督的警示。 | `alerts-list` | Adobe Experience Platform | 「顯示我訂閱的高嚴重度警示。」<br><br>「本週觸發了哪些來自我的警示的警示？」<br><br>「我的任何訂閱警示需要注意嗎？」 |
