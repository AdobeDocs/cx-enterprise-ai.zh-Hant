---
title: Generative AI內容透明度
description: 瞭解Adobe如何在Adobe CX Enterprise應用程式中，自動將C2PA中繼資料附加至GenAI產生和GenAI編輯的內容。
feature_v2:
  - id: f84b2906-3ce9-4ef0-86f6-cda249273937
  - id: ec4263d9-bf7c-44c7-b3f1-3e664861c8f2
source-git-commit: 4a9ab38cc3aa650dbb90639558d25f6acf707da5
workflow-type: tm+mt
source-wordcount: 1714
ht-degree: 1%

---


# Generative AI內容透明度

在整個2026年8月，Adobe已逐步在Adobe Creative Cloud、Adobe Document Cloud、Adobe Firefly和Adobe CX企業應用程式中推出C2PA中繼資料支援。

>[!NOTE]
>
>推出後，涉及使用AI建立或編輯內容的未來工作流程將自動獲得C2PA中繼資料支援。

本頁包含有關Adobe如何跨Adobe CX Enterprise應用程式處理C2PA中繼資料自動附加的詳細資訊。

新法規要求創作AI技術的提供者支援與GenAI產生和GenAI編輯的內容工作流程相關的永續性、機器可讀披露，以擴大透明度。

作為工具提供者，Adobe使用Adobe技術（包括Adobe工作流程中受支援的協力廠商產生式人工智慧模型），將機器可讀的C2PA中繼資料自動附加到GenAI產生的和GenAI編輯的內容。 [進一步瞭解C2PA](https://c2pa.org/)。

## 變更內容

Adobe將於2026年8月推出，在Adobe Creative Cloud、Adobe Document Cloud、Adobe Firefly和Adobe CX企業應用程式中推出C2PA中繼資料支援。

此版本包括：

* 將C2PA中繼資料自動附加至支援的GenAI產生和GenAI編輯的內容。
* 支援內容型別，包括影像、視訊、音訊和文字。
* 在整個支援的Adobe工作流程中保留C2PA中繼資料。

將C2PA中繼資料附加到合格的產生AI內容不需要額外的動作。

>[!NOTE]
>
>C2PA中繼資料不會影響內容的外觀。 C2PA中繼資料和可見浮水印有不同的用途。 C2PA中繼資料提供機器可讀取的來源資訊，而可見浮水印提供視覺化公開。 您可以根據業務需求與每個適用管轄區的法律規定，選擇將可見浮水印新增至您的內容。

## C2PA中繼資料會新增哪些詳細資訊

自動附加的C2PA中繼資料可能包含下列資訊：

* 所使用AI系統的名稱和版本資訊（例如，Adobe GenStudio、Adobe Firefly）
* 使用的AI模型（例如Adobe Firefly）
* 使用方式：是否使用GenAI產生或編輯
* 使用創作AI工具建立和/或修改內容的時間和日期
* 唯一識別碼（可用來區分Generative AI的每種用法）

## 整個內容supply chain的C2PA中繼資料

C2PA中繼資料的設計目的，是在其在Adobe應用程式和相容的協力廠商平台之間移動時，維持與支援內容的關聯。

當內容發佈、發佈或共用時，支援C2PA中繼資料或相關來源技術的平台可以讀取附加的中繼資料並向使用者顯示透明度資訊。

Adobe無法控制內容離開Adobe應用程式後，外部服務如何解譯、顯示或使用C2PA中繼資料。 客戶應參閱個別發佈平台的檔案，瞭解如何處理C2PA中繼資料。

## 可見浮水印

在某些情況下，在特定地理區域中，組織可能會選擇或要求以可視方式識別GenAI產生的或GenAI編輯的內容。

Adobe提供使用Adobe應用程式支援的現有浮水印功能的[指南](https://helpx.adobe.com/tw/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html)。 是否需要可見的浮水印取決於組織的業務需求以及發佈內容所在司法管轄區的適用法律和法規。

>[!NOTE]
>
>C2PA中繼資料和可見浮水印有不同的用途。 C2PA中繼資料提供機器可讀取的來源資訊，而可見浮水印則提供組織可選擇套用的視覺公開。

## 可用性與版本

這些功能將於整個&#x200B;**2026年8月**&#x200B;日在支援的Adobe CX Enterprise工作流程中推出。

>[!NOTE]
>
>推出後，涉及使用AI建立或編輯內容的未來工作流程將自動獲得C2PA中繼資料支援。

此版本包含：

### 自動C2PA中繼資料

C2PA中繼資料會自動附加至受支援的GenAI產生和GenAI編輯的內容。 此功能預設為啟用，無法停用。

### 浮水印指引

Adobe提供[檔案](https://helpx.adobe.com/tw/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html)，說明如何為選擇或需要套用可見標籤的組織使用受支援Adobe應用程式中可用的現有浮水印功能。

## Adobe CX Enterprise支援的應用程式 {#supported-applications}

下列Adobe應用程式和服務會針對C2PA中繼資料如何及何時附加至特定CX Enterprise應用程式中的合格內容提供詳細資訊。

不過，如果適用，所有Adobe CX Enterprise應用程式會在支援的資產透過Adobe工作流程移動時，繼續保留現有的C2PA中繼資料。 這有助於在supply chain內容中維持來源資訊的完整性。

>[!NOTE]
>
>下列各應用程式的發行說明或指南，將可於Experience League上其各自的應用程式產品頁面區段中取得。 表格會在連結可用時隨連結更新。 請參閱Experience League的最新產品區段。

| 應用程式/解決方案 | 發行說明/指南 |
|---|---|
| Adobe Advertising Cloud | [文件](https://experienceleague.adobe.com/zh-hant/docs/advertising/creative/creative-studio/creative-studio-content-credentials) |
| Adobe Experience Manager (AEM) | [文件](https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/c2pa-metadata-dynamic-media-openapi) |
| 用於內容產生的AI助理（Adobe Journey Optimizer / Adobe Campaign中的功能） | [文件](https://experienceleague.adobe.com/zh-hant/docs/journey-optimizer/using/content-management/generate-content/generative-c2pa-metadata) |
| Adobe Journey Optimizer B2B Ultimate | [文件](https://experienceleague.adobe.com/zh-hant/docs/journey-optimizer-b2b/user/content-management/assets/c2pa-metadata) |
| Adobe Journey Optimizer B2B Prime （亦稱為Adobe Marketo Optimizer） | [文件](https://experienceleague.adobe.com/zh-hant/docs/marketo-optimizer/user/content/assets/c2pa-metadata) |
| Adobe Journey Optimizer B2C | |
| Adobe Campaign | |
| Adobe Commerce | [文件](https://experienceleague.adobe.com/zh-hant/docs/commerce/optimizer/manage-results/success-metrics#c2pa-metadata-on-exported-reports) |
| GenStudio for Performance Marketing | [文件](https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/content/content-credentials) |
| Adobe Marketo Engage | [文件](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/demand-generation/images-and-files/c2pa-metadata) |
| Adobe Workfront | [文件](https://experienceleague.adobe.com/zh-hant/docs/workfront/using/documents/c2pa-metadata-overview) |
| CX Enterprise Co-worker Campaigns （前身為HALO） | [文件](https://experienceleague.adobe.com/zh-hant/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/c2pa-metadata) |

## 相關連結

* [可見浮水印指南](https://helpx.adobe.com/tw/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html)
* [Adobe Inspect](https://contentauthenticity.adobe.com/inspect)
* [Adobe GenAI標籤合規性計畫概覽](https://helpx.adobe.com/tw/creative-cloud/apps/generative-ai/ai-content-labeling-faq.html)

## 常見問題

**哪些Adobe應用程式將C2PA中繼資料套用至已編輯或建立的產生AI內容？**

支援的Adobe CX Enterprise應用程式會自動將C2PA中繼資料附加至合格的GenAI產生和GenAI編輯的內容。 如需Adobe CX Enterprise應用程式的詳細資訊，請參閱[支援的應用程式](#supported-applications)區段。

**Adobe將C2PA中繼資料新增到哪些內容型別？**

大致來說，影像、音訊、視訊、檔案和文字都在範圍之內。 不過，請參考[支援的應用程式](#supported-applications)區段中的檔案，瞭解每個應用程式如何支援不同產品和內容型別的C2PA中繼資料。

**Adobe CX中的哪些應用程式會在編輯和發佈期間保留C2PA中繼資料？**

所有Adobe CX Enterprise應用程式的設計目的，都是為了在內容流經相容的Adobe工作流程時保留C2PA中繼資料。 Adobe應用程式外部的儲存取決於外部平台是否支援C2PA中繼資料。

**將多個GenAI產生的影像合併成單一影像時會發生什麼事？**

產生的C2PA中繼資料取決於使用的應用程式和工作流程。 如果支援此功能，Adobe會在整個編輯過程中保留來源資訊。 如需每個應用程式中工作流程特定行為的檔案，請參閱[支援的應用程式](#supported-applications-across-adobe-cx-enterprise)區段。

**當GenAI從Adobe和非Adobe應用程式產生的影像合併時，會發生什麼事？**

Adobe會保留工作流程中可用且支援的C2PA中繼資料。 只要適用，只要在Adobe工作流程中使用GenAI編輯或建立適用內容（影像、音訊、視訊、文字），Adobe就會使用最新資訊更新基礎中繼資料。 將多個來源合併為一個新資產時，不會取代或遺失其基礎中繼資料。 相反地，新資產會取得自己的C2PA中繼資料，而來自每個來源的詳細資訊會保留在其中。 如果來源已有其自己的C2PA中繼資料（無論來自Adobe或非Adobe工具），則歷史記錄會附加至該來源。 這表示最終資產會呈現完整影象：其使用GenAI建立或編輯的專屬記錄，加上每個片段的個別歷史記錄。

**在Adobe CX應用程式中，GenAI編輯和GenAI建立的工作流程會自動附加C2PA中繼資料嗎？**

有。 對於支援的創作AI工作流程，Adobe會自動附加C2PA中繼資料，以識別內容是GenAI產生還是GenAI編輯，以及其他來源資訊，例如時間戳記、AI系統資訊和唯一識別碼。

**在整個內容supply chain中如何維護C2PA中繼資料？**

C2PA中繼資料是耐用的中繼資料，可在相容的Adobe應用程式與支援的協力廠商平台之間移動時，與支援的內容維持關聯。 外部服務決定附加的來源資訊在發佈後如何顯示。

**組織如何在不中斷來源鏈的情況下新增自己的已驗證資訊？**

有些Adobe應用程式可讓建立者和組織將其他驗證資訊新增至現有的C2PA中繼資料，同時保留原始資料。 可用性因應用程式而異。

**是否可以關閉C2PA中繼資料的自動附件？**

沒有。 新的創作AI透明度法律要求提供創作AI工具（包括Adobe）的公司將持久中繼資料附加到使用創作AI產生或編輯的合格內容。 無法關閉C2PA中繼資料的自動附加。

**使用generative AI在8月發行之前建立/編輯的內容有什麼改變？**

在2026年8月版本之前使用創作AI工具建立或編輯的內容沒有附加自動C2PA中繼資料。 不過，在Firefly網站和先前套用C2PA中繼資料的其他應用程式中建立的內容，仍會繼續附加這些內容。

**客戶如何檢查內容是否附加C2PA中繼資料？**

客戶可透過將C2PA中繼資料上傳至[Adobe Inspect](https://contentauthenticity.adobe.com/inspect)頁面來檢查內容是否附加了C2PA中繼資料。

**發佈或共用內容後，外部平台如何顯示C2PA中繼資料？**

隨著內容在發佈平台、社群媒體頻道、電子郵件服務和其他數位生態系統中移動，支援C2PA中繼資料或相關來源技術的下游服務可能能夠讀取附加的中繼資料，並根據該資訊選擇顯示披露或指標。 Adobe無法控制外部平台如何顯示、詮釋或套用與附加的C2PA中繼資料相關聯的披露。 如需特定平台如何處理來源資訊的最新資訊，客戶應直接檢視該平台的指引。

**這些變更是否會增加Adobe產品或訂閱的成本？**

沒有。 C2PA中繼資料不會影響Adobe產品的成本。
