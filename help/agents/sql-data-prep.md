---
title: Co-worker中的SQL資料準備
description: 瞭解如何在Co-worker中使用SQL資料準備來產生、最佳化、疑難排解和排程SQL查詢。
source-git-commit: dff76b520c013554276e72a3e19b5d56c16af5fa
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 1%
---
# Co-worker中的SQL資料準備

在Co-worker中使用SQL資料準備，以自然語言提示執行一般[資料Distiller](https://experienceleague.adobe.com/en/docs/experience-platform/query/data-distiller/overview)工作。 您可以產生SQL、疑難排解或最佳化現有查詢、預覽結果，以及排程查詢以循環執行。

>[!AVAILABILITY]
>
>Co-worker中的SQL資料準備功能在「有限可用性」中提供。

## 先決條件 {#prerequisites}

在Co-worker中使用SQL資料準備之前，請確定您具有：

- 資料Distiller權益。
- 存取同事。

## 開始使用 {#get-started}

若要開始，請開啟[Co-worker]，然後輸入描述您要達成之SQL工作或結果的自然語言要求。

您可以識別要在請求中使用的資料集。 如果需要其他資訊才能完成工作，同事可以在繼續之前詢問後續問題。

Co-worker產生或更新SQL之後，您可以繼續交談以預覽結果、調整查詢、儲存查詢，或排程重複執行。

如需使用同事介面的指引，請參閱[同事使用者介面指南](../coworker/chat/ui-guide.md)。

## 支援的功能 {#supported-capabilities}

您可以使用SQL資料準備來執行下列工作：

| 功能 | 說明 |
| --- | --- |
| **SQL製作** | 從您要執行之資料作業的自然語言描述產生SQL。 |
| **SQL最佳化** | 分析現有的資料Distiller查詢，並將其效能最佳化，同時保留預期結果。 |
| **SQL錯誤診斷與更正** | 診斷現有SQL查詢中的錯誤，說明根本原因，並產生更正的SQL。 |
| **查詢排程與警示** | 儲存並排程定期執行的查詢，以及設定支援的查詢警示。 |

## 在交談中使用SQL資料準備 {#work-with-sql-data-preparation}

您可以將SQL資料準備功能合併到同一個同事交談中，而不是將它們視為單獨的工作流程。

例如，您可以：

1. 描述您要的結果並產生SQL。
2. 預覽最多5列的查詢結果。
3. 縮小查詢範圍或詢問有關所產生SQL的問題。
4. 儲存查詢。
5. 排程查詢以循環執行並設定警報。

當需要其他資訊時，同事可以詢問後續問題，例如識別適當的資料集或確認排程的時區。

查詢預覽最多可傳回5列。 若要直接在Experience Platform中執行和使用查詢，請參閱[查詢編輯器UI指南](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/user-guide)。

![顯示五列SQL查詢結果預覽的同事回應，以及可將查詢儲存為範本或排程重複執行的選項。](./assets/sql-data-prep/query-preview.png)

### 從自然語言產生SQL {#generate-sql}

當您知道想要達成的結果或轉換，但希望Co-worker產生對應的SQL時，請使用SQL編寫。

若要從正確的資料產生SQL，Co-worker可以識別並驗證相關的資料集。 如果您的請求未提供足夠的資訊來識別適當的資料集，同事可在繼續之前提出後續問題。

例如：

> 您好！ 使用test_luma_web_events_1000，依事件型別摘要客戶參與。 顯示事件型別、事件總數和不重複客戶。 針對每個事件型別傳回一列，並依獨特客戶從最高到最低排序結果。

Co-worker會傳回產生的SQL，並可執行查詢以提供結果的預覽。

![Co-worker回應顯示依據事件型別摘要客戶參與情況的已產生SQL，隨後是事件總數與不重複客戶的表格預覽，以及結果分析。](./assets/sql-data-prep/authoring-result.png)

如需有關直接在Experience Platform中建立和執行查詢的資訊，請參閱[查詢編輯器UI指南](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/user-guide)。

### 最佳化現有SQL {#optimize-sql}

當您已經有資料Distiller查詢，並且想要在不變更預期結果的情況下改善其效能時，請使用SQL最佳化。

您可以要求「同事」說明變更、比較原始與最佳化SQL，並提供驗證或查詢計畫資訊。

例如：

> 針對資料Distiller效能最佳化下列查詢，同時保留完全相同的結果。 說明您變更的內容，以及最佳化查詢在邏輯上等價的原因。
>
> ```sql
> SELECT
>         p.customer_id,
>         p.first_name,
>         p.last_name,
>         p.loyalty_status,
>         COUNT(o.order_id) AS total_orders,
>         SUM(CAST(o.order_total AS DOUBLE)) AS total_revenue
> FROM test_luma_profiles_1000 p
> INNER JOIN test_luma_orders_1000 o
>         ON p.customer_id = o.customer_id
> GROUP BY
>         p.customer_id,
>         p.first_name,
>         p.last_name,
>         p.loyalty_status
> ORDER BY total_revenue DESC;
> ```
>
> 傳送完整回應給我，尤其是原始的SQL、最佳化的SQL、對等性說明，以及任何EXPLAIN/驗證結果。

如果提供的查詢已經最佳化，Co-worker可以確定不需要修改，並解釋其評估。

![同事回應分析現有SQL查詢以進行最佳化，並說明不需要變更，以及查詢計畫發現專案與對等評估。](./assets/sql-data-prep/optimize-query.png)

已最佳化透過SQL編寫功能產生的SQL。 您不需要個別提交新產生的SQL以進行最佳化。

如需SQL語法和支援的命令，請參閱[查詢服務SQL參考](https://experienceleague.adobe.com/en/docs/experience-platform/query/sql/overview)。

### 診斷並修正SQL錯誤 {#diagnose-sql-errors}

當現有查詢失敗且您需要協助識別原因並修正SQL時，請使用SQL錯誤診斷。

Co-worker會分析查詢、識別錯誤原因、說明問題並提供更正的SQL。

例如：

> 嗨！ 下列查詢失敗。 診斷錯誤、說明根本原因，並提供更正的查詢：
>
> ```sql
> SELECT
>         o.order_id,
>         o.product_id,
>         p.product_name,
>         o.order_total
> FROM test_luma_orders_1000 o
> JOIN test_luma_product_catalog_1000 p
>         ON o.productid = p.productid;
> ```
>
> 更正後的查詢應使用兩個資料集中的適當產品ID欄位。

更正查詢之後，您可以要求Co-worker執行查詢並預覽結果。

![Co-worker回應正在診斷因產品ID欄位名稱不正確所導致的SQL查詢錯誤，並提供使用product_id欄位的更正SQL。](./assets/sql-data-prep/diagnose-error.png)

### 排程查詢並設定警報 {#schedule-queries}

產生、更正或預覽查詢後，您可以繼續交談以儲存並排程其重複執行。

例如：

> 將此查詢排程為每天早上6:00執行。 設定查詢失敗時的警示。

如果必要的資訊遺失或模稜兩可，同事會在建立排程之前詢問後續問題。 例如，它可以要求您確認與請求的執行時間關聯的時區。

在您確認必要的排程詳細資訊後，「同事」會傳回已儲存查詢範本、排程、時區、狀態及失敗警示的摘要。

![確認已排程SQL查詢的同事回應，包括儲存的範本、排程、時區、結束日期、排程狀態以及失敗警示。](./assets/sql-data-prep/schedule-query.png)

如需有關查詢排程、週期設定、輸出資料集和警示的詳細資訊，請參閱[查詢排程](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/query-schedules)。

## 後續步驟 {#next-steps}

如需SQL資料準備所使用的資料Distiller和查詢服務功能的詳細資訊，請參閱下列檔案：

- [資料Distiller概觀](https://experienceleague.adobe.com/en/docs/experience-platform/query/data-distiller/overview)
- [查詢編輯器UI指南](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/user-guide)
- [查詢排程](https://experienceleague.adobe.com/en/docs/experience-platform/query/ui/query-schedules)
- [查詢服務SQL參考](https://experienceleague.adobe.com/en/docs/experience-platform/query/sql/overview)
