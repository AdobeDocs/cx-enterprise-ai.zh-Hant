---
title: CX Enterprise Applications中的AI
description: 瞭解CX Enterprise應用程式如何使用generative AI (GenAI)、AI Assistant、agentic AI、CX Enterprise Co-worker和MCP工具。
TQID: https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: d095671a-1355-40aa-8b5f-06c33c68080bid: e1e0219c-f879-479f-8427-888ed2a6e9c2id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 2d8059201070965b01e67d2c910adc3a7b66ab01
workflow-type: tm+mt
source-wordcount: 881
ht-degree: 3%

---

# CX Enterprise 中的 AI

本指南涵蓋Adobe CX Enterprise應用程式中可用的AI功能：適用於產品知識和營運見解的創作AI和AI助理、適用於自動化工作的Agent Orchestrator和Experience Platform代理程式、適用於完全對話且代理優先體驗的CX Enterprise Co-worker，以及用於將您自己的AI工具連線到CX Enterprise資料的MCP。

## 關於CX Enterprise中的AI

從這裡開始，瞭解在CX Enterprise中使用人工智慧的位置和方式：

- [Generative AI](./overview/generative-ai.md)說明哪些CX Enterprise應用程式支援generative AI和AI Assistant，以及它們的比較方式。
- [Agentic AI](./overview/agentic-ai.md)說明Experience Platform Agents如何在現有的CX Enterprise應用程式和AI優先應用程式中運作，並列出每個應用程式中可用的代理程式。
- [Agentic AI監控](./overview/monitoring.md)涵蓋追蹤代理程式採用、使用、回饋和AI信用消耗的控制面板。
- [代理程式工作和AI信用耗用量](./overview/ai-credit-consumption.md)說明代理程式工作如何使用AI信用耗用，以及代理程式和工作型別的預估耗用率。

## AI 助理

[AI小幫手](./ai-assistant/ai-assistant-ui.md)是對話式創作AI工具，可在Adobe Experience Platform應用程式中使用。 透過全熒幕或邊欄檢視介面中的自然語言提示，使用它來取得產品知識、疑難排解問題、尋找營運見解並存取Experience Platform代理程式。

閱讀[AI小幫手UI指南](./ai-assistant/ai-assistant-ui.md)，瞭解如何瀏覽介面，以及[提示程式庫](./ai-assistant/prompt-library.md)，以取得代理程式的範例提示。

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

如需代理程式、每個支援的應用程式以及資格要求的完整清單，請參閱[CX Enterprise中的Agentic AI](./overview/agentic-ai.md)。

## CX Enterprise同事

CX Enterprise Co-worker是AI Assistant的代理程式優先進化，可自動化客戶體驗和行銷工作流程，讓您的團隊可專注於業務目標而非例行執行。 您不必一次詢問一個問題，而是用自然語言描述一個目標，Co-worker會規劃工作、在您的Adobe和連線系統中執行、驗證結果，以及將完成的工作傳回給您核准。 同事包括：

- **[同事聊天](https://experienceleague.adobe.com/en/docs/cx-enterprise-coworker/content/chat/overview)**：探索資料、驗證對象和歷程以及完成CX Enterprise應用程式的多步驟工作的對話式介面。
- **[同事行銷活動](https://experienceleague.adobe.com/en/docs/cx-enterprise-coworker/content/campaigns/overview)**：AI原生應用程式，使用內建範本、最佳實務和提示指引，將行銷活動簡報、對象建立、內容產生、歷程設計和校訂整合為單一對話體驗，讓小型敏捷團隊能夠快速啟動行銷活動。
- **同事專案** （即將推出）：統一的工作區可自動化端對端客戶體驗協調工作流程，協助團隊協調工作、核准及執行，以推動策略到傳遞的結果。 專案的檔案即將推出。

符合資格的客戶正逐步從AI助理和Experience Platform代理程式轉換為同事聊天。 閱讀[CX Enterprise Co-worker試用版](./agents/trial.md)，了解試用資格、AI信用使用情況，以及如何取得存取權。

若要檢視同事聊天正在執行中，請逐步瀏覽[Playground中的同事聊天](./coworker/playground-coworker-chat.md)，或閱讀真實使用案例，例如[驗證AA到CJA的移轉資料](./coworker/data-validation-aa-cja.md)和[分析CJA資料](./coworker/analytics-chat.md)。

如需有關同事聊天、行銷活動和專案的完整產品檔案，請參閱[Adobe CX Enterprise Co-worker](https://experienceleague.adobe.com/zh-hant/docs/cx-enterprise-coworker/content/home)。

## MCP

[Adobe CX Co-worker閘道](./mcp/overview.md)是CX Enterprise的統一模型內容通訊協定(MCP)端點。 它提供與MCP相容的使用者端（例如[!DNL Claude]、[!DNL ChatGPT]和[!DNL Cursor]），與您組織有權使用的產品工具（包括Real-Time CDP、Experience Platform、Journey Optimizer、Customer Journey Analytics和Adobe Analytics）的單一控管連線。

## 開始使用

### 存取需求

您的Adobe管理員必須授與適當的許可權，您才能使用AI助理和Experience Platform代理程式。 需求因應用程式而異；如需詳細資訊，請參閱Agent Orchestrator指南中的[存取](./agents/agent-orchestrator.md#access)。

### 隱私權與安全性

AI Assistant和Experience Platform代理程式以隱私、安全性和控管作為最前沿，包括沙箱特定的資料隔離和遵循您現有的存取控制政策。 如需完整詳細資訊，請閱讀[AI助理的隱私、安全性和治理](./ai-assistant/privacy.md)。

## 最佳實務

若要從您的AI助理或同事體驗中獲得最大價值，請遵循以下最佳實務：

- **在提示中指定**，以取得目標和相關見解。
- **檢閱提供的來源引文和推理解釋，以驗證回應**。
- **使用內容設定**，確定您的問題使用了最相關的資料來源。
- **提供意見回饋**，協助改善一段時間內的效能和正確性。
- **結合來自多個代理程式的深入分析**，以獲得更全面的分析。

## 法律考量

AI Assistant目前僅支援英文回應，語言模型偶爾可能會出錯。 務必確認所提供的資訊，並使用每個回應中所包含的推理步驟來瞭解其產生方式。 如需完整詳細資訊，請閱讀[法律免責宣告](./ai-assistant/legal-disclaimer.md)。
