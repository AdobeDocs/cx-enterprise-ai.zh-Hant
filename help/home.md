---
title: CX Enterprise 應用程式中的 AI
description: 瞭解CX Enterprise應用程式如何使用generative AI (GenAI)、CX Enterprise Coworker、AI Assistant、agentic AI和MCP工具。
TQID: 'https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds'
product_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
    internal-label: CX Enterprise Coworker
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
    internal-label: Governance
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
source-git-commit: 81c51c896a10559db58c6389a08f9c84b96ef73c
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 2%
---
# CX Enterprise應用程式中的AI

本指南涵蓋Adobe CX Enterprise中的AI功能：generative AI、CX Enterprise Coworker、AI Assistant、Agent Orchestrator和MCP。

## AI功能概觀

從這裡開始，逐步瞭解在CX Enterprise中使用人工智慧的位置和方式：

- [關於產生式AI](./overview/generative-ai.md)說明哪些CX Enterprise應用程式支援產生式AI和AI助理，以及它們之間的比較方式。
- [關於代理程式AI](./overview/agentic-ai.md)說明代理程式AI如何在現有的CX Enterprise應用程式和AI優先應用程式中運作，並列出每個應用程式中可用的代理程式。
- [AI監視](./overview/monitoring.md)涵蓋追蹤代理程式採用、使用、回饋和AI信用消耗的控制面板。
- [AI積分耗用量](./overview/ai-credit-consumption.md)說明代理程式工作如何耗用AI積分，以及依代理程式和工作型別的預估耗用率。
- [Generative AI內容透明度](./content-transparency.md)說明Adobe如何跨CX Enterprise應用程式將C2PA中繼資料自動附加至GenAI產生和GenAI編輯的內容。
- [CX Enterprise代理程式工具](https://experienceleague.adobe.com/zh-hant/docs/cx-enterprise-agentic-tools/using/overview)涵蓋擴充CX Enterprise代理程式的其他代理程式技能和工具（影片教學課程）。

## Coworker

Co-worker是AI Assistant的代理程式優先演化，可自動化客戶體驗和行銷工作流程，讓您的團隊可專注於業務目標而非例行執行。 您描述的目標不是一次詢問一個問題。 同事計畫、執行、驗證及傳回已完成的工作以供您核准。 深入瞭解[Adobe for Business](https://business.adobe.com/products/cx-enterprise-coworker.html)。

同事包括：

- **[同事聊天](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/overview)**：探索您的資料、驗證對象和歷程以及完成跨CX Enterprise應用程式的多步驟工作的對話式介面。
- **[同事行銷活動](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/overview)**：AI原生應用程式，將行銷活動簡報、對象建立、內容產生、歷程設計和校訂整合為單一對話體驗。 它使用內建範本、最佳實務和提示性指引，協助小型敏捷團隊快速啟動行銷活動。 深入瞭解[Adobe for Business](https://business.adobe.com/products/cx-enterprise-coworker/teams.html)。
- **同事專案** （即將推出）：統一的工作區可自動化端對端客戶體驗協調工作流程，協助團隊協調工作、核准及執行，以推動策略到傳遞的結果。 專案的檔案即將推出。

符合資格的客戶正逐步從AI助理和Experience Platform代理程式轉換為同事聊天。 閱讀[同事試用版](./agents/trial.md)，了解試用資格、AI信用使用情況，以及如何取得存取權。

若要檢視同事聊天正在執行中，請逐步瀏覽[Playground中的同事聊天](./coworker/playground-coworker-chat.md)，或閱讀真實使用案例，例如[驗證AA到CJA的移轉資料](./coworker/chat/use-cases/data-insights/data-validation-aa-cja.md)和[分析CJA資料](./coworker/chat/use-cases/data-insights/analytics-chat.md)。

如需有關同事聊天、團隊同事（同事行銷活動）和專案的完整產品檔案，請參閱[同事](./coworker/overview.md)。 如需沙箱到沙箱物件復寫，請參閱[沙箱工具代理程式技能](./agents/sandbox-tooling.md)。

## AI 助理

[AI小幫手](./ai-assistant/ai-assistant-ui.md)是對話式創作AI工具，可在Adobe Experience Platform應用程式中使用。 透過全熒幕或邊欄檢視介面中的自然語言提示，使用它來取得產品知識、疑難排解問題、尋找營運見解並存取Experience Platform代理程式。

若要瞭解如何導覽介面，請閱讀[AI助理使用者介面指南](./ai-assistant/ai-assistant-ui.md)。 若要檢視代理程式的範例提示，請參閱[提示程式庫](./ai-assistant/prompt-library.md)。

## Agent Orchestrator與Experience Platform代理程式

[Agent Orchestrator](./agents/agent-orchestrator.md)是支援Experience Platform代理程式的代理程式層。 當您向AI Assistant提問時，Agent Orchestrator會規劃工作、呼叫回答問題所需的專業代理程式，並傳回統一的回應，所有這些都是由人為監督。

本指南記錄下列Experience Platform代理程式：

- [Audience 代理](./agents/audience.md)
- [Data Insights Agent](./agents/cja-data-insights-agent.md)
- [Experimentation Agent](./agents/agent-experiment.md)
- [欄位探索代理程式](./agents/field-discovery-agent.md)
- [Journey Agent](./agents/ajo-agent.md)
- [通知代理](./agents/notifications.md)
- [產品支援代理](./agents/product-support.md)
- [Adobe Marketing Agent for Microsoft 365 Copilot](./agents/ama-ms.md)
- [驗證您的資料](./agents/data-validation.md)

如需代理程式、每個支援的應用程式以及資格要求的完整清單，請參閱CX Enterprise中的[代理程式AI](./overview/agentic-ai.md)。

## MCP

[Adobe CX Coworker閘道](./mcp/overview.md)是CX Enterprise的統一模型內容通訊協定(MCP)端點。 它提供與MCP相容的使用者端，例如[!DNL Claude]、[!DNL ChatGPT]和[!DNL Cursor]，與貴組織有權使用的產品工具進行單一控管連線：

- [Real-Time CDP工具](./mcp/rtcdp-mcp.md)
- [Experience Platform工具](./mcp/aep-mcp.md)
- [Journey Optimizer工具](./mcp/ajo-mcp.md)
- [Customer Journey Analytics工具](./mcp/cja-mcp.md)
- [Adobe Analytics工具](./mcp/analytics-mcp.md)
- [!DNL Workfront]工具，記錄在[Workfront MCP伺服器指南](https://experienceleague.adobe.com/en/docs/workfront/using/basics/workfront-mcp-server/workfront-mcp-server-overview)中
- [!DNL Target]工具，記錄在[目標MCP伺服器指南](https://experienceleague.adobe.com/en/docs/target/using/mcp/target-mcp)中

第一次使用CX Coworker Gateway？ 請參閱[存取CX Coworker閘道工具](./mcp/access.md)和[安裝CX Coworker閘道](./mcp/install.md)以連線。 連線之後，在呼叫產品工具之前，請使用[工作階段內容工具](./mcp/context-tools.md)來設定作用中的組織、沙箱和資料檢視。

在使用任何這些工具之前，請參閱[開始之前](./overview/overview-ai-cxe.md#before-you-begin)有關存取要求、隱私權及安全性考量事項。

## 最佳實務

若要從您的AI助理或同事體驗中獲得最大價值，請遵循以下最佳實務：

- **在提示中指定**，以取得目標和相關見解。
- **檢閱提供的來源引文和推理解釋，以驗證回應**。
- **使用內容設定**，確定您的問題使用了最相關的資料來源。
- **提供意見回饋**，協助改善一段時間內的效能和正確性。
- **結合來自多個代理程式的深入分析**，以獲得更全面的分析。

## 法律考量

AI Assistant目前僅支援英文回應，語言模型偶爾會犯錯。 務必確認所提供的資訊，並使用每個回應中所包含的推理步驟來瞭解其產生方式。 如需完整詳細資訊，請閱讀[法律免責宣告](./ai-assistant/legal-disclaimer.md)。

Adobe也會在CX Enterprise應用程式中，自動將C2PA中繼資料附加至GenAI產生和GenAI編輯的內容，以符合產生性的AI透明度法規。 如需詳細資訊，請閱讀[Generative AI內容透明度](./content-transparency.md)。

