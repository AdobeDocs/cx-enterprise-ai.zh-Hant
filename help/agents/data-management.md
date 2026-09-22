---
title: Adobe Experience Platform的資料管理代理程式
description: 瞭解如何使用CX Coworker中的資料管理代理程式來尋找和分析Adobe Experience Platform資料集，以及管理Data Lake保留政策。
source-git-commit: 40f144c7a06592c78dccc6c17f19554b62f667c9
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 3%
---
# 資料管理代理程式

>[!AVAILABILITY]
>
>所有可存取Adobe CX Enterprise Coworker的客戶皆可使用資料管理代理程式。

若要瞭解並管理體驗事件資料集的資料湖保留，請使用CX Coworker中的資料管理代理程式。 隨著Adobe Experience Platform資料湖中的體驗事件資料整合長，查詢和下遊程式可能需要更長的時間才能完成，而保留要求則變得更難管理。 以自然語言描述您想要達成的目的。 資料管理代理程式會尋找相關的體驗事件資料集、分析這些資料集的使用主動性，並模擬提議的保留期會對多少資料產生影響。 當您準備好採取行動時，它可幫助您設定、變更或移除保留原則，並在任何變更前要求您確認。

## Data Management Agent的功能 {#what-the-data-management-agent-can-do}

資料管理代理程式提供四種技能。

>[!NOTE]
>
>列出資料集、分析資料集使用情形和分析資料集保留技能均為唯讀。 只有「管理資料集保留」技能可以變更資料湖保留政策，而且需要在套用任何變更前進行明確確認。

| 技能 | 說明 |
|---|---|
| **列出資料集** | 在決定從何處開始保留檢閱時使用。 列出具有儲存大小、列數、現有保留設定和設定檔啟用的體驗事件資料集，以便您快速識別可能成為資料湖保留原則的候選資料集 |
| **分析資料集使用量** | 在決定資料集是否適合用於資料湖保留原則之前，請先使用。 根據訊號（例如最近的擷取、查詢活動和下游應用程式使用情況）分類特定資料集的使用主動性。 |
| **分析資料集保留** | 在確認保留期間之前使用。 顯示資料集的儲存量度和資料的年齡，然後使用該年齡分佈來估計潛在保留期將保留或移除的資料量。 |
| **管理資料集保留** | 在您準備好採取行動時使用。 設定、變更或移除資料集上的資料湖保留原則，並在任何變更前進行影響預覽和確認。 |

## 範圍：資料湖保留與其他資料管理工具的比較 {#scope}

當您需要尋找和分析體驗事件資料集，以及設定、變更或移除資料湖保留原則時，請使用資料管理代理程式。

如果您不確定資料湖保留原則是否為目標的正確選項，請參閱[選擇正確的資料生命週期管理功能](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/data-lifecycle/choose-a-capability)，以比較可用的保留和刪除選項。

這些技能不會管理下列相關功能：

- **設定檔存放區保留原則。** 若要管理體驗事件在設定檔存放區中保留的時長，請針對已啟用設定檔的體驗事件資料集設定體驗事件到期原則。 請參閱[體驗事件有效期](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/profile/event-expirations)。
- **沙箱範圍的假名設定檔資料到期日。** 如果要在符合設定的條件時，自動刪除沙箱中的假名設定檔資料，請參閱[假名設定檔](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/profile/pseudonymous-profiles)。
- **資料集到期日。** 若要將整個資料集排程在未來日期刪除，請參閱[資料集到期日](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/data-lifecycle/ui/dataset-expiration)。
- **刪除記錄。** 若要基於隱私權或衛生理由移除個別設定檔記錄，請參閱[刪除記錄](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/data-lifecycle/ui/record-delete)。

## 先決條件 {#prerequisites}

在開始之前，請確定您已：

- 存取Adobe Experience Platform和包含您要檢閱之資料集的沙箱。
- 您要使用的資料集和保留動作所需的Adobe Experience Platform許可權。 Data Management Agent會使用您現有的Experience Platform許可權，不會授與額外存取權。 請參閱[存取控制總覽](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/access-control/home)，瞭解Adobe Experience Platform許可權和角色的運作方式。
- CX Coworker中安裝的Adobe CXO外掛程式。

如需有關安裝外掛程式的說明，請參閱[Co-worker UI指南](https://experienceleague.adobe.com/zh-hant/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide)。

## 使用資料管理代理程式 {#use-the-data-management-agent}

使用自然語言透過CX Coworker與資料管理代理程式互動。 說明您的目標，然後使用後續問題調整結果。

>[!NOTE]
>
>開始之前，請確定您使用的沙箱包含您要檢閱的資料集。

若要使用「資料管理代理程式」：

1. 導覽至&#x200B;**[!UICONTROL CX Coworker]**。 如需存取詳細資訊，請參閱[同事使用者介面指南](https://experienceleague.adobe.com/zh-hant/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide)。
1. 輸入說明所要完成之工作的要求。
1. 檢閱結果並使用後續問題繼續您的調查。

如果請求變更資料湖保留原則，資料管理代理程式會顯示建議的影響，並需要您確認後再套用變更。

如需識別資料集、分析使用情況和保留影響，以及管理資料湖保留原則的端對端工作流程，請參閱[管理資料湖保留](../coworker/chat/use-cases/data-management/manage-data-lake-retention.md)。

## 資料管理代理程式的運作方式 {#how-the-data-management-agent-works}

資料管理代理程式會使用確定性計算來分析資料集使用情況，讓相同的輸入產生相同的使用情況層級。 它也能以程式設計方式計算保留率影響，而非依賴AI產生的估計值。 保留影響仍維持近似值，因為它是根據資料的年齡分佈。 代理程式會直接從Adobe Experience Platform服務擷取資料，以提供資料集的最新資訊。

## 限制 {#limitations}

資料管理代理程式可以識別可能是資料湖保留原則良好候選的資料集，但不會決定資料集是否需要候選資料集。 若未經您明確確認，則不會套用、變更或移除保留原則。

## 後續步驟 {#next-steps}

如需使用各項技能來尋找、分析和管理體驗事件資料集上的資料湖保留率的相關指引，請參閱[管理資料湖保留率](../coworker/chat/use-cases/data-management/manage-data-lake-retention.md)。

如需有關Adobe Experience Platform中資料湖保留原則如何運作的詳細資訊，包括保留行為和設定，請參閱[體驗事件資料集保留(TTL)指南](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/catalog/datasets/experience-event-dataset-retention-ttl-guide)。
