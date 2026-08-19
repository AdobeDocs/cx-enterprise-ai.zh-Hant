---
description: 瞭解同事行銷活動如何自動在影像上附加及保留C2PA中繼資料(Content Credentials)，從產生到電子郵件傳遞。
title: 同事行銷活動中的C2PA中繼資料
hide: true
source-git-commit: 17acfbd783e1e70b965636b806c465be8cf73522
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 4%

---

# 同事行銷活動中的C2PA中繼資料 {#overview}

圍繞創作AI透明度的新法律不斷湧現，Adobe正在努力滿足各個司法轄區的適用要求。 [C2PA中繼資料](https://c2pa.org/) （也稱為Content Credentials）是Adobe用來符合這些法律要求的來源工具。

C2PA中繼資料是持久且隱藏的中繼資料，會記錄內容的建立或編輯方式。 當您使用Co-worker Campaigns中的產生AI工具產生或編輯影像時，C2PA中繼資料會自動附加至該影像。 您不需要採取任何動作。

## 電子郵件行銷活動中的Content Credentials {#content-credentials-email}

電子郵件行銷活動中傳送的影像會儲存其Content Credentials，讓收件者可以直接從傳送的電子郵件驗證任何影像的來源和真實性。

## 附加C2PA中繼資料的動作 {#cc-workflows}

下表根據在Co-worker Campaigns中產生影像時執行的影像動作，摘要附加C2PA中繼資料的時間。

| 動作 | 說明 | 要附加C2PA中繼資料嗎？ | 使用案例範例 |
| --- | --- | --- | --- |
| **產生影像** | 從文字提示或參考影像建立新影像，或從現有影像產生類似影像。 | 一律。 影像是由產生式AI產生，因此一律會攜帶最新的C2PA中繼資料。 | 電子郵件促銷活動的橫幅影像是從描述所需視覺效果的文字提示中產生。 |

## 內容型別及其範圍 {#cc-content-types}

* **影像**：已涵蓋。 使用產生AI產生影像時，會附加C2PA中繼資料，並透過在Co-worker Campaigns中由影像產生執行的裁切、文字覆蓋和影像覆蓋作業來保留。
* **文字**：不適用。 在合作行銷活動中產生影像的純文字輸出，例如產生復本、翻譯和品牌對齊建議，不需要C2PA中繼資料。

## 內容移動時發生什麼事 {#cc-content-moves}

「同事行銷活動」會保留與支援的影像資產相關聯的Content Credentials。 如果影像在匯入至「同事行銷活動」時包含Content Credentials，則當資產用於產生的行銷活動內容和傳出電子郵件體驗時，會保留這些憑證。

<!-- Some ways of bringing images into your content, such as extracting an image from a PDF or from an embedded (base64) source, may not preserve the original C2PA metadata. In these cases, no C2PA metadata can be read from the source, and none is created for the result. -->

## 其他資源

* [Adobe Experience Cloud Generative AI使用者指南](https://www.adobe.com/tw/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}

* [護欄與限制](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/generate-content/gs-generative#generative-guardrails){target="_blank"}
