---
description: 瞭解Co-worker Campaigns如何在AI產生和編輯的影像上自動附加和保留C2PA中繼資料(Content Credentials)，不需要採取任何動作。
title: 同事行銷活動中的C2PA中繼資料
hide: true
source-git-commit: 785b5d106cb029d68506c90385786cbdae164991
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 2%

---

# 同事行銷活動中的C2PA中繼資料 {#overview}

圍繞創作AI透明度的新法律不斷湧現，Adobe正在努力滿足各個司法轄區的適用要求。 [C2PA中繼資料](https://c2pa.org/) （也稱為Content Credentials）是Adobe用來符合這些法律要求的來源工具。

C2PA中繼資料是持久且隱藏的中繼資料，會記錄內容的建立或編輯方式。 當您使用Co-worker Campaigns中的產生AI工具產生或編輯影像時，C2PA中繼資料會自動附加至該影像。 您不需要採取任何動作。

## 附加C2PA中繼資料的動作 {#cc-workflows}

下表根據在Co-worker Campaigns中產生影像時執行的影像動作，摘要附加C2PA中繼資料的時間。

| 動作 | 說明 | 要附加C2PA中繼資料嗎？ | 使用案例範例 |
| --- | --- | --- | --- |
| **產生影像** | 從文字提示或參考影像建立新影像，或從現有影像產生類似影像。 | 一律。 影像是由產生式AI產生，因此一律會攜帶最新的C2PA中繼資料。 | 電子郵件促銷活動的橫幅影像是從描述所需視覺效果的文字提示中產生。 |
| **裁切影像** （中央或智慧型裁切） | 將影像調整至要求的尺寸 | 僅當來源影像已具有C2PA中繼資料時。 裁切會重新建立影像的畫素，這通常會清除該C2PA中繼資料，因此Co-worker Campaigns中的影像產生會在裁切前從來源影像中讀取該影像，然後重新建置該影像，並將其重新附加至裁切的結果。 裁切本身不會新增創作AI動作，而是保留現有動作。 | 產生的橫幅影像會裁切成適合網頁：透過裁切會保留C2PA中繼資料。<br> 用作推播通知背景的上傳庫存像片會被裁切以適合熒幕：由於庫存像片不執行產生式AI動作，因此不會建立任何C2PA中繼資料。 |
| **新增文字覆蓋** | 在背景影像上演算產生的文字 | 僅當背景影像已具有C2PA中繼資料時。 轉譯覆蓋圖時，會從背景加上文字產生新影像，通常會清除該C2PA中繼資料，因此Co-worker Campaigns中的影像產生會預先從背景影像讀取，然後重新建置並重新附加至結果。 覆蓋步驟不會新增新產生的AI動作。 | 促銷標題會在登陸頁面產生的背景影像上呈現為文字重疊：背景影像的C2PA中繼資料會保留。 |
| **覆蓋影像** | 將兩個或多個影像複合在一起 | 如果任何來源影像有C2PA中繼資料，則合併的影像會攜帶所有內容，並合併到單一C2PA中繼資料集中。 合成作業會從來源產生新影像，這通常會清除該C2PA中繼資料，因此在Co-worker Campaigns中產生的影像會在合成作業前讀取每筆資料，然後建立一筆合併的C2PA中繼資料記錄，其中列出有助於產生式AI動作的每個來源。 | 產生的產品影像與為電子郵件標題產生的背景複合在一起：結果包含反映兩個產生AI來源的C2PA中繼資料。<br> 將兩張上傳的品牌像片合成一個拼貼：由於來源皆未執行創作AI動作，因此不會建立任何C2PA中繼資料。 |

## 內容型別及其範圍 {#cc-content-types}

* **影像**：已涵蓋。 使用產生AI產生影像時，會附加C2PA中繼資料，並透過在Co-worker Campaigns中由影像產生執行的裁切、文字覆蓋和影像覆蓋作業來保留。
* **文字**：不適用。 在合作行銷活動中產生影像的純文字輸出，例如產生復本、翻譯和品牌對齊建議，不需要C2PA中繼資料。

## 內容移動時發生什麼事 {#cc-content-moves}

「同事行銷活動」會保留與支援的影像資產相關聯的Content Credentials。 如果影像在匯入至「同事行銷活動」時包含Content Credentials，則當資產用於產生的行銷活動內容和傳出電子郵件體驗時，會保留這些憑證。 [進一步瞭解C2PA中繼資料](https://helpx.adobe.com/firefly/using/content-credentials.html){target="_blank"}。

<!-- Some ways of bringing images into your content, such as extracting an image from a PDF or from an embedded (base64) source, may not preserve the original C2PA metadata. In these cases, no C2PA metadata can be read from the source, and none is created for the result. -->

>[!MORELIKETHIS]
>
>[Adobe Experience Cloud Generative AI使用者指南](https://www.adobe.com/tw/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}
