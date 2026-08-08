---
description: 瀏覽同事聊天使用案例和範例提示，依資料深入分析、受眾、歷程和平台操作的區域進行整理。
title: 使用案例
source-git-commit: 5a04f8fea57dcf6e50ca0040aaad904158c6edf7
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 4%

---

# 使用案例 {#use-cases}

以下為從業人員在Adobe CX Enterprise Co-worker Chat中使用的使用案例和範例提示，依工作區組織。 每個提示都是為複製而建置，會根據您自己的資料和內容進行調整，並透過對話進行細化。

## 資料深入分析

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| 提取CJA報告與量度 | 即時查詢CJA以提取量度、維度、區段和資料檢視 | `cja` | Customer Journey Analytics (CJA) | 「顯示過去30天的頁面檢視」 · 「在主資料檢視中列出排名最前的區段」 |
| 比較分析 | 並排比較不同管道、時段或區段的量度 | `cja` | Customer Journey Analytics (CJA) | 「按管道月份比較每月收入」 · 「本季行動與桌上型電腦轉換看起來如何？」 |
| funnel分析 | 逐步瞭解每個階段都有流失的多步驟轉換漏斗 | `cja` | Customer Journey Analytics (CJA) | 「帶我瀏覽funnel結帳」 · 「顯示從PDP到購買的轉換funnel」 |
| 預測 | 根據歷史CJA資料預測未來的量度值 | `cja` | Customer Journey Analytics (CJA) | 「未來30天的預測工作階段」 · 「我們是否可望達成收入目標？」 |
| 根本原因分析 | 調查量度變更的原因：診斷下降、尖峰和異常 | `cja-root-cause-analysis` | Customer Journey Analytics (CJA) | 「為什麼上週轉換率下降？」 · 「是什麼導致1月15日的收入激增？」 |
| 執行摘要和KPI摘要 | 製作適合利害關係人的效能摘要、規範性建議和投影片組大綱 | `cja-executive-summary` | Customer Journey Analytics (CJA) | 「給我上個月的執行摘要」 · 「從本季的資料建立投影片投影片組大綱」 |
| AA ↔ CJA資料驗證 | 在Adobe Analytics和Customer Journey Analytics之間比較、稽核及調解資料 | `aa-cja-validation` | ADOBE ANALYTICS + CJA | 「將我的AA報告套裝與CJA資料檢視進行比較」 · 「驗證AA與CJA之間的頁面檢視」 |
| 作業時間序列與因果分析 | 查詢和分析具有因果歸因的對象、資料集和歷程的歷史時間序列資料 | `operational-stats-causal-analysis` | 所有符合資格的應用程式 | 「顯示過去90天的對象人數趨勢」 · 「為什麼我的資料集列會計入3月3日的尖峰？」 |
| 建立自訂CJA技能 | 將分析模式轉換為可重複使用、且跨工作階段儲存的技能 | `cja-skill-creator` | Customer Journey Analytics (CJA) | 「將此每週收入分析轉換為可重複使用的技能」·「將此儲存為每月funnel報告的技能」 |

## 客群

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| 從自然語言建立對象 | 透過每個階段的使用者核准，策劃逐步的受眾建立 | `audience-creation-flow` | Real-Time CDP (RTCDP) | 「建立過去30天內購買的使用者受眾」 · 「為加州的高價值忠誠會員建立區段」 |
| 建置PQL定義 | 從XDM屬性、行為事件或現有對象中組合對象定義；支援彙總和時間範圍 | `segment-definition-assembly` | Real-Time CDP (RTCDP) | 「為檢視3個以上產品但未購買的使用者建立PQL」 · 「為我的事件條件新增7天時段」 |
| 搜尋和尋找對象 | 依ID、名稱、語意搜尋尋找對象；偵測重複專案並分析重疊 | `audience-search` | Real-Time CDP (RTCDP) | 「尋找所有忠誠受眾」 · 「我的『節日購物者』區段是否有重複專案？」 |
| 預估對象規模 | 使用Adobe Experience Platform預覽API搭配輪詢來預估PQL運算式的設定檔觸及率 | `audience-size-estimate` | Real-Time CDP (RTCDP) | 「此對象有多大？」 · 「此PQL運算式的預估觸及率」 |
| 對象人數瀑布 | 將PQL分解為子述詞，並顯示每個條件對最終對象規模的貢獻 | `audience-size-waterfall` | Real-Time CDP (RTCDP) | 「顯示此PQL的瀑布圖」 · 「劃分每個條件如何減少受眾」 |
| 探索用於定位的XDM欄位 | 依名稱、說明或資料值搜尋欄位；檢視欄位的使用位置和使用位置 | `field-discovery` | Real-Time CDP (RTCDP) | 「我可以使用哪些欄位來鎖定忠誠客戶？」 · 「尋找與購買記錄相關的欄位」 |
| 發佈/儲存對象 | 透過命名慣例和合規性檢查將受眾定義儲存至Experience Platform細分服務 | `audience-publish` | Real-Time CDP (RTCDP) | 「將此專案儲存為草稿」 · 「以『春季促銷買家』名稱發佈對象」 |

## 歷程

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| 從自然語言建立歷程 | 透過文字提示或上傳的影像/流程圖，在AJO中協調歷程建立 | `journey-create` | Adobe Journey Optimizer (AJO) | 「建立歡迎歷程，在註冊後傳送電子郵件、等待3天，然後傳送後續追蹤」 · 「從這個上傳的流程圖影像建立歷程」 |
| 分析歷程衝突 | 偵測使用中歷程之間的對象重疊、排程衝突及重複資料刪除問題 | `journey-analyze-conflict` | Adobe Journey Optimizer (AJO) | 「我的購物車放棄歷程是否與其他歷程衝突？」 · 「檢查我作用中歷程之間的受眾重疊」 |
| 分析歷程流失 | 識別客戶在歷程中下降的位置和原因，並偵測導致脫離參與的行為模式 | `journey-analyze-fallout` | Adobe Journey Optimizer (AJO) | 「在我的重新參與歷程中，人們在哪裡停下來？」 · 「歷程X中的哪些節點流失率最高？」 |
| 分析自訂動作錯誤 | 識別歷程中自訂動作失敗或錯誤率飆升的時間，並在失敗升級為更廣泛的中斷之前診斷根本原因 | `journey-analyze-custom-action` | Adobe Journey Optimizer (AJO) | 「為什麼自訂動作會在我的忠誠度註冊歷程中失敗？」 · 「在我的歡迎歷程中，顯示自訂動作ExternalPush的錯誤率。」 |

## 基本元素

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| 產品知識與檔案 | 從官方Adobe檔案中回答操作說明、概念、疑難排解和最佳作法問題 | `product-knowledge` | 所有符合資格的應用程式 | 「如何設定串流目的地？」 · 「批次和串流細分之間有何差異？」 |
| 查詢Experience Platform / Journey Optimizer實體 | 作為平台實體相關問題的主要入口點；視需要路由至KG、欄位探索或API | `operational-insights` | 所有符合資格的應用程式 | 「我有多少資料集？」 · 「顯示所有使用中的歷程」 · 「列出我的目的地」 |
| 知識圖查詢 | 透過單一SQL查詢的彙總計數、跨實體聯結、關係查閱和中繼資料探索 | `knowledge-graph` | 所有符合資格的應用程式 | 「哪些對象使用此資料集？」 · 「顯示結構描述和資料集之間的關係」 |
| Experience Platform / Journey Optimizer / Customer Journey Analytics API作業 | 提供直接API閘道，用於變更、即時狀態檢查以及不在知識圖形中的實體型別 | `cxo-api` | 所有符合資格的應用程式 | &quot;刪除資料集X&quot; · &quot;檢查批次擷取工作的狀態&quot; |
| 實體解析度和連結 | 使用語意和辭彙搜尋來解析對實際Experience Platform實體的實體提及，並探索XDM欄位 | `entity-linking` | Adobe Experience Platform | 「將『節日購物者』解析為實際受眾」 · 「尋找與購買記錄相關的我欄位」 |
| 管理自訂技能 | 儲存、修改或刪除使用者擁有的可重複使用技能，這些技能會跨工作階段存留 | `manage-skill` | 所有符合資格的應用程式 | 「將工作流程另存為技能」 · 「刪除我的每週報告技能」 · 「將此轉換為可重複使用的技能」 |

## 沙箱工具

| 使用案例 | 說明 | 技能 | 應用程式 | 範例提示 |
| --- | --- | --- | --- | --- |
| 在沙箱間移動物件中繼資料 | 透過自動解析的相依性，順暢地跨沙箱移轉結構描述、受眾和其他物件設定 | `sandbox-tooling-workflow` | Adobe Experience Platform | 「將方案Luma忠誠會員白金從目前的沙箱移至生產沙箱」· 「將美國金級忠誠會員對象提升至階段」 |
