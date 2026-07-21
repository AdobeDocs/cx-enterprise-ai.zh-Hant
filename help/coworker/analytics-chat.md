---
title: 透過同事聊天分析Customer Journey Analytics資料
description: 瞭解如何使用Adobe CX Enterprise Co-worker Chat分析Customer Journey Analytics資料、建立漏斗，以及找出客戶在歷程中的流失點。
source-git-commit: 6e3ab12f1d9ec706e745749b7ca47b91a09ff8b3
workflow-type: tm+mt
source-wordcount: '2104'
ht-degree: 4%

---

# 透過同事聊天分析Customer Journey Analytics資料

>[!AVAILABILITY]
>
>本文所述的功能處於發行的有限測試階段，可能尚未在您的環境中提供。 當功能正式可用時，將移除此附註。 如需Customer Journey Analytics發行程式的相關資訊，請參閱[Customer Journey Analytics功能發行](https://experienceleague.adobe.com/zh-hant/docs/analytics-platform/using/releases/latest)。

Adobe CX Enterprise Co-worker Chat可以執行進階資料分析，而以前只能在Analysis Workspace中執行這種分析。 Co-worker Chat會存取您Customer Journey Analytics資料檢視中的資料，讓您探索該資料並獲得自然語言提示的答案。

開始分析之前，請先瞭解同事聊天介面和設定選項，然後確定同事已連線至Customer Journey Analytics以及包含您要使用之資料的資料檢視。

## 開始使用同事聊天

### 介面和設定選項

在使用「同事聊天」處理Customer Journey Analytics資料之前，請先瞭解如何登入及管理下列功能的設定選項：

* 聊天輸入

* 交談

* Marketplace

* MCP伺服器

* 記憶體

* 外掛程式

* 技能

* 及更多內容

如需詳細資訊，請參閱[同事聊天使用者介面指南](https://experienceleague.adobe.com/en/docs/cx-enterprise-coworker/content/chat/ui-guide)。

### Customer Journey Analytics的使用案例

您可以檢視Customer Journey Analytics使用案例和從業人員在Adobe CX Enterprise Co-worker Chat中使用的範例提示。 每個提示都是為複製而建置，會根據您自己的資料和內容進行調整，並透過對話進行細化。

如需詳細資訊，請參閱[使用案例](https://experienceleague.adobe.com/en/docs/cx-enterprise-coworker/content/chat/use-cases)。

## 確認同事聊天已連線至Customer Journey Analytics

1. 在同事聊天中，確認同事已連線至Customer Journey Analytics：

1. 在左側邊欄中選取MCP圖示，然後確定連線的MCP伺服器清單中有&#x200B;[!UICONTROL **cja-mcp**]。

   ![Co-worker左側邊欄中反白的MCP圖示](assets/data-validation-aa-cja/coworker-mcp-cja.png)

1. （條件式）如果尚未連線&#x200B;[!UICONTROL **cja-mcp**]，請選取&#x200B;[!UICONTROL **新增MCP伺服器**]，在&#x200B;[!UICONTROL **伺服器名稱**]&#x200B;欄位中指定cja，並在它出現時加以選取，然後選取&#x200B;[!UICONTROL **新增伺服器**]。

## 連線到正確的資料檢視

資料檢視是Customer Journey Analytics中的容器，可決定如何解譯資料。

您可能會存取Customer Journey Analytics中的各種資料檢視，每個檢視都包含Co-worker在分析資料時可使用的不同維度和量度。

### 決定您要使用哪些資料檢視

告訴同事您要回答的問題型別，並詢問您有權存取哪些資料檢視最適合提供該資訊。 您也可以[將資料檢視設定為記憶體](#add-a-data-view-preference-in-memory)中的偏好設定。

**您：**

>[!BEGINSHADEBOX]

我感興趣的是瞭解客戶在客戶歷程中何時流失。 我在Customer Journey Analytics中可以存取哪些資料檢視，以便回答這個問題？

>[!ENDSHADEBOX]

**同事聊天回應：**

>[!BEGINSHADEBOX]

您可以存取三個資料檢視。 `Customer lifecycle`資料檢視包含以下維度和量度，最適合回答您的問題。

>[!ENDSHADEBOX]

**您：**

>[!BEGINSHADEBOX]

很好，讓我們使用該資料檢視。

>[!ENDSHADEBOX]

**同事聊天回應：**

>[!BEGINSHADEBOX]

好的，我將使用`Customer lifecycle`資料檢視來回答此聊天工作階段中未來的問題。

>[!ENDSHADEBOX]

### 在記憶體中新增資料檢視偏好設定

Co-worker Chat包含記憶體功能，可讓您存取跨越所有聊天內容的資訊。 將您偏好的資料檢視新增為同事記憶體的偏好設定，會是個好做法。

1. 在「同事聊天」的左側導覽中，選取「記憶體」圖示。

1. 在「記憶體」頁面的「預存的偏好設定」段落中，指定您希望「同事聊天」在聊天中使用的一或多個資料檢視。

   左側邊欄中的![記憶體區段](assets/data-validation-aa-cja/coworker-memory.png)

## 在Customer Journey Analytics中分析

Co-worker建立視覺效果後，您可以在Customer Journey Analytics中開啟Analysis Workspace的視覺效果，以更精細的控制功能進行更深入的分析。 視覺效果會在Customer Journey Analytics的新Analysis Workspace專案中開啟。

若要在新的Analysis Workspace專案中開啟視覺效果：

1. 選取「在CJA中分析&#x200B;**]」（位於在Co-worker中建立的任何視覺效果旁）。[!UICONTROL **

1. 在Customer Journey Analytics中開啟視覺效果後，您可以使用Analysis Workspace拖放瀏覽器介面進行修改、進一步製作分析、建立對象等。 您甚至可以和您選擇的任何人共用您的Workspace專案。

   如需Analysis Workspace的詳細資訊，請參閱[Analysis Workspace概觀](https://experienceleague.adobe.com/zh-hant/docs/analytics-platform/using/cja-workspace/home)。

## 範例：尋找客戶流失的位置

您可以要求「同事聊天」使用您的資料來分析任何業務問題。

例如，身為行銷經理、銷售人員或成長負責人，您可能想要瞭解客戶在哪裡捨棄購買路徑、他們為什麼捨棄，以及可以採取哪些措施來推動更高轉換率。

>[!NOTE]
>
>下圖是虛構的retailer [!DNL TechPulse Electronics]的說明性範例資料，用來顯示交談的形狀。

### 您可以問的問題型別

您不需要知道「流失視覺效果」是什麼，或哪個量度屬於哪個位置。 請改用簡單的語言描述您關心的結果：

* 「在購買的過程中，我們在哪裡失去客戶？」
* 「從產品檢視到結帳，我的完整轉換funnel是什麼？」
* 「哪些行銷管道在購物車和購買之間洩漏最多？」
* 「在行動裝置或桌上型電腦上放棄購物車的情況更糟糕嗎？」
* 「付費社交網站的訪客與電子郵件的訪客的轉換有不同嗎？」

### 交談

#### &#x200B;1. 從業務問題開始

**您：**

>[!BEGINSHADEBOX]

在購買途中，我們會在哪裡失去人員？

>[!ENDSHADEBOX]

**同事聊天回應：**

請注意，「同事聊天」會選擇正確的視覺效果、排序接觸點，甚至新增建議的後續步驟。

>[!BEGINSHADEBOX]

![同事funnel回應](assets/data-validation-aa-cja/coworker-funnel-response.png)

這是funnel的問題 — 讓我執行轉換funnel，以檢視購買路徑上下降發生在何處。

以下是您失去人的地方：

| funnel步驟 | Count | 轉換至下一個 | 流失 |
| --- | --- | --- | --- |
| 工作階段 | 137,476 | 45.0%檢視產品 | 55%離開而不瀏覽產品 |
| 產品檢視 | 61,845 | 購物車新增55.0% | 45%瀏覽但未新增 |
| 購物車新增次數 | 34,045 | 購買16.4% | 83.6%放棄購物車 |
| 購買 | 5,582 | — | — |

**重大發現：要購買的購物車是您最大的流失**

28,463個人將商品加入購物車，但從未完成購買。 這相當於83.6%的購物車對購買量下降率，是目前最大的單一故障點。

若以美元計算，這些購物車加貨者中只要轉換10%，就能增加約2,846筆購買。 在目前的資料規模下，這是表格上可能尚存的重大收入。

**這告訴您優先順序的內容：**

| 優先順序 | 問題 | 機會規模 |
| --- | --- | --- |
| #1 | 放棄購買（下跌83.6%） | 28,463位失去的買家 |
| #2 | 產品檢視的工作階段（55%永不瀏覽） | 75,631場不含產品參與的工作階段 |
| #3 | 產品檢視到購物車（45%未新增） | 27,800個有興趣但未認可 |

**建議的後續步驟：**

1. 依行銷管道劃分購物車放棄率 — 某些管道是否帶來低意圖流量，這些流量新增至購物車但從未購買？
1. 依裝置型別檢視購物車放棄率 — 行動結帳摩擦是否會造成轉換次數？
1. 識別哪些產品最遭捨棄 — 價格問題？ 送貨驚喜？

**您想讓我深入瞭解其中的哪些專案？** 管道劃分會直接告訴您哪些行銷動作會帶來「幾乎買家」或實際買家。

>[!ENDSHADEBOX]

#### &#x200B;2. 深入探查洩漏

**您：**

>[!BEGINSHADEBOX]

好，讓我們依行銷管道來劃分

>[!ENDSHADEBOX]

**同事聊天回應：**

>[!BEGINSHADEBOX]

![同事funnel回應](assets/data-validation-aa-cja/coworker-funnel-response2.png)

有一個自訂&#x200B;**行銷管道**&#x200B;維度。 讓我提取funnel，然後計算每個管道的轉換率，並識別每個管道的洩漏點。

**裁決：洩漏不是通道特定的**

這是個很有啟發性的發現。 以下是每個管道的funnel劃分：

| 頻道 | 工作階段 | 至產品檢視 | 至購物車新增 | 要購買 | 整體轉換 | 收入/工作階段 |
| --- | --- | --- | --- | --- | --- | --- |
| 付費搜尋 | 43,958 | 45.1% | 54.6% | 16.6% | 4.09% | $499.58 |
| 有機搜尋 | 31,492 | 44.9% | 54.9% | 16.9% | 4.17% | $494.76 |
| 直接 | 25,661 | 43.6% | 55.4% | 15.8% | 3.82% | $497.29 |
| 電子郵件 | 17,586 | 45.3% | 55.4% | 16.2% | 4.07% | $501.13 |
| 付費社交 | 12,684 | 45.4% | 55.7% | 16.0% | 4.03% | $512.17 |
| 顯示 | 6,511 | 45.3% | 55.7% | 16.2% | 4.09% | $501.45 |

**主要外賣點：**

1. 所有管道的購物車對購買量下降都一樣是不良的(83-84%)。 這表示問題不在於流量品質 — 每個管道都會提供類似的參與訪客。 洩露的是您的結帳體驗本身，而不是您的行銷。
1. 沒有管道在轉換方面要好或壞很多。 整體轉換率在3.8%和4.2%之間緊密叢集，每個工作階段的收入幾乎相同（495美元至512美元）。
1. 數量影響最重要的地方：付費搜尋的絕對損失人數最多（9,015個購物車放棄），接著是有機搜尋（6,449個損失）。 這些是價值最高的商機，因為它們帶來的流量最多。

**這會在策略上告訴您什麼**

行銷管道正在完成他們的工作 — 它們讓人們對它們感興趣並以類似的速率加入購物車。 問題是行銷的下游：您的結帳和付款流程是資金流失的地方。

**建議的下一個調查：**

1. 依裝置型別劃分購物車放棄率 — 行動結帳是損壞還是令人沮喪？
1. 看看哪些產品最容易被捨棄 — 結帳時有價格或運送驚喜嗎？
1. 檢查「holiday_flash_sale」行銷活動是否有更好的結帳轉換 — 急迫性導向的行銷活動可能會克服結帳摩擦

**您接下來要探索哪個角度？**

>[!ENDSHADEBOX]

#### &#x200B;3. 繼續調查

**您：**

>[!BEGINSHADEBOX]

有意思。 讓我們嘗試依裝置型別劃分。

>[!ENDSHADEBOX]

**同事聊天回應：**

>[!BEGINSHADEBOX]

![同事funnel回應](assets/data-validation-aa-cja/coworker-funnel-response3.png)

**已找到：行動簽出已中斷**

在結帳之前，所有裝置中的funnel都相同，然後行動裝置就會掉落懸崖：

| 裝置 | 工作階段 | 至產品檢視 | 至購物車新增 | 要購買 | 整體轉換 |
| --- | --- | --- | --- | --- | --- |
| 桌面 | 70,172 | 44.9% | 54.8% | 23.2% | 5.70% |
| 平板電腦 | 14,149 | 44.7% | 55.6% | 14.3% | 3.56% |
| Mobile | 53,449 | 44.9% | 55.3% | 8.1% | 2.02% |

**確鑿證據**

| 量度 | 桌面 | Mobile | 間隙 |
| --- | --- | --- | --- |
| 購物車到購買率 | 23.2% | 8.1% | 15個百分點 |
| 行動裝置是 | — | 差2.8倍 | — |
| 放棄的購物車 | 13,274 | 12,178 | 絕對體積幾乎相同 |

行動裝置上的瀏覽和加入購物車的體驗相當不錯（相同的瀏覽率約為45%，加入購物車的率約為55%）。 人們也同樣感興趣和參與。 但行動結帳流程中的某些專案會扼殺轉換次數。

**收入機會**

如果行動結帳的轉換率與桌上型電腦的轉換率相同，您將會額外購買約1,991件，修正一次體驗後，購買量會增加35%。

**可能發生的情況**

資料模式（平等參與、災難性的結帳下降）是下列專案的典型訊號：

* 小熒幕上的付款表單摩擦（自動填寫問題、表單版面配置）
* 結帳時發現意外成本（運費、稅金），造成貼紙震動
* 訪客簽出不可用或行動裝置上的登入留言板
* 在行動裝置上進行付款處理期間，出現頁面載入或逾時問題

**建議的後續步驟：**

1. 依產品類別劃分行動購物車放棄率 — 高價商品會更糟糕嗎（建議行動支付信任問題）？
1. 看看哪些行銷管道帶來的行動流量最多 — 您花在付費媒體上的錢將人們送到中斷的行動裝置funnel中嗎？
1. 檢查是否有頁面或網站區域訊號 — 我們是否能看到行動使用者在放棄前最後點選的結帳頁面？

**您想要探索哪些，或此證據是否足以帶給您的UX和結帳團隊？**

>[!ENDSHADEBOX]

#### &#x200B;4. 將其轉換為決定

**您：**

>[!BEGINSHADEBOX]

那我該怎麼辦？

>[!ENDSHADEBOX]

**同事聊天回應：**

>[!BEGINSHADEBOX]

根據資料顯示內容，我會聚焦於以下位置：

* **修正行動簽出 — 這不是頻道問題。** 每個管道都會以類似且健康的比率將人們轉換為購物車，因此廣告支出是全面運作的。 該收入會遺失，尤其是修正所屬的行動結帳流程。
* **開始付款和表單摩擦。** 這些是高意願行動購物者放棄購物車的最常見原因。 提供行動電子錢包選項和縮短表格通常是最快的贏家。
* **修正後重新檢查。** 結帳變更送貨後，請注意行動裝置的購物車對購買率是否朝桌上型電腦的23.2%移動。

希望我將此專案儲存為專案，以便您進行追蹤，或是在行動購物車到購買次數降到臨界值以下時設定警報？

>[!ENDSHADEBOX]

### 剛發生的事

在四個直白的問題中，同事幫助我們：

* 建立多步驟轉換funnel，並將購物車對購買標示為最大流失
* 排除行銷管道是造成問題的原因 — 每個管道洩漏的速度幾乎相同
* 將真正的問題隔離到行動結帳中，並以35%的購買量來量化修正
* 離開時可設定優先順序：行動支付與表單摩擦。 以桌上型電腦的23.2%轉換率為基準

<!--

## Example #2: Find which marketing efforts drive revenue

You can ask Coworker Chat to use your data to analyze any business question.

For example, as a marketing manager, demand generation lead, or CMO, you might want to know which marketing efforts actually deserve credit for revenue so you can confidently decide where to put your marketing spend, rather than rewarding whichever channel happened to get the last click.

>[!NOTE]
>
>The figures below are illustrative sample data for a fictional retailer, [!DNL TechPulse Electronics], used to show the shape of the conversation.

### The types of questions you can ask

You don't need to know what an "attribution model" is, or how to configure an Attribution panel. Instead, describe the outcome you care about in plain language:

* "Which channels actually drive our revenue, not just the last click?"
* "If I change how I give credit for a sale, does my best channel change?"
* "Which campaigns start customer journeys versus close them?"
* "Am I over-investing in paid search because it always gets the last click?"
* "What role does email play in conversions it never gets credit for?"

### The conversation

#### 1. Start with the business question

**You:**

>[!BEGINSHADEBOX]

Which marketing channels actually drive our revenue?

>[!ENDSHADEBOX]

**Coworker Chat response:**

Notice that Coworker Chat picks the right analysis, starts with the model most reports default to, and immediately flags what that model can't tell you.

>[!BEGINSHADEBOX]

![Coworker Chat showing attributed revenue by marketing channel under a last-touch model](assets/data-validation-aa-cja/coworker-attribution-response.png)

This is an attribution question — let me attribute revenue to your marketing channels so you can see who's earning it.

I'll start with **last-touch attribution**, since that's what most out-of-the-box reports show. It gives all the credit for a sale to the last channel a person used before purchasing.

| Marketing channel | Attributed revenue (last touch) | Share |
| --- | --- | --- |
| Paid search | $948,000 | 34% |
| Organic search | $614,000 | 22% |
| Direct | $474,000 | 17% |
| Email | $307,000 | 11% |
| Paid social | $251,000 | 9% |
| Display | $195,000 | 7% |

**The headline: paid search looks like your hero**

Under last touch, paid search earns a third of all revenue — more than any other channel. If this were the only view you had, you'd likely pour more budget into paid search.

**One important caveat before you do that**

Last touch only tells you who *closed* the sale. It says nothing about who *started* the journey or *assisted* along the way. A channel that introduces people to your brand weeks before they buy gets zero credit here, even if the purchase never would've happened without it.

To know whether paid search is really driving revenue — or just harvesting demand other channels created — you need to compare attribution models.

**Recommended next step:**

Compare the same channels across first-touch, last-touch, and linear models. If paid search stays on top across all of them, it's a genuine driver. If it shrinks under first touch, it's a closer, not a creator.

**Want me to run that comparison?**

>[!ENDSHADEBOX]

#### 2. Compare attribution models

**You:**

>[!BEGINSHADEBOX]

Yes, compare it across models.

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

![Coworker Chat comparing channel revenue share across first-touch, last-touch, and linear attribution models](assets/data-validation-aa-cja/coworker-attribution-response2.png)

Here's each channel's share of revenue under three models. First touch credits the channel that started the journey, last touch credits the one that closed it, and linear splits credit evenly across every touch.

| Marketing channel | First touch | Last touch | Linear |
| --- | --- | --- | --- |
| Paid search | 19% | 34% | 26% |
| Organic search | 20% | 22% | 21% |
| Direct | 9% | 17% | 13% |
| Email | 18% | 11% | 15% |
| Paid social | 21% | 9% | 15% |
| Display | 13% | 7% | 10% |

**The verdict: your "best" channel depends entirely on how you count**

This is the finding that changes budget decisions.

1. **Paid search closes far more than it starts.** It jumps from 19% of first touches to 34% of last touches. That's the signature of a *harvester* — it captures people who are already ready to buy, often after another channel introduced them. Valuable, but it's finishing journeys, not creating them.
1. **Paid social and email are badly undercredited by last touch.** Paid social starts 21% of journeys but gets credit for only 9% of sales. Email starts 18% but closes 11%. These channels are doing the expensive work at the top of the funnel and handing warm prospects to paid search.
1. **Organic search is your steady workhorse.** It sits around 20% across every model — it both starts and closes journeys reliably.

**Why this matters for budget**

If you cut paid social or email based on their weak last-touch numbers, you'd starve the top of your funnel — and paid search would have far fewer ready-to-buy people to close. You'd likely see paid search revenue fall too, even though you didn't touch its budget.

**Recommended next step:**

Look at the campaign level to see exactly which efforts start journeys versus close them. That's where you can act — trimming or protecting specific campaigns rather than whole channels.

**Want me to break this down by campaign?**

>[!ENDSHADEBOX]

#### 3. Keep investigating

**You:**

>[!BEGINSHADEBOX]

Let's break it down by campaign.

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

![Coworker Chat showing top campaigns ranked by their role as initiators or closers of customer journeys](assets/data-validation-aa-cja/coworker-attribution-response3.png)

There's a **Campaign Name** dimension. Here are your highest-involvement campaigns, comparing the revenue they start (first touch) against the revenue they close (last touch).

| Campaign | Starts (first touch) | Closes (last touch) | Role |
| --- | --- | --- | --- |
| brand_awareness_q3 | $412,000 | $103,000 | Initiator |
| email_winback | $214,000 | $88,000 | Initiator |
| holiday_flash_sale | $268,000 | $249,000 | All-rounder |
| retargeting_dynamic | $71,000 | $339,000 | Closer |
| branded_search_always_on | $84,000 | $498,000 | Closer / harvester |

**The pattern: some of your "worst" campaigns are actually your best starters**

* **brand_awareness_q3** and **email_winback** start far more revenue than they close. On a last-touch ROI report, these look like underperformers you might cut. In reality, they're filling the top of your funnel — the journeys other campaigns finish.
* **retargeting_dynamic** and **branded_search_always_on** are the opposite. They close a lot but start almost nothing. They're efficient closers, but they can only close demand that already exists. Branded search, in particular, is largely capturing people who were going to search for you by name anyway.
* **holiday_flash_sale** does both — it introduces new shoppers and closes them, which is why urgency-driven promotions often look strong under any model.

**What this tells you strategically**

The campaigns you'd cut first on a last-touch report — the awareness and win-back efforts — are the ones creating the demand your closers depend on. Judge initiators on the journeys they start, and closers on the journeys they finish.

**Recommended next steps:**

1. Protect the initiator campaigns even though their last-touch ROI looks weak — they're feeding the funnel.
1. Right-size the branded search spend — test whether trimming it changes total revenue, since much of that demand may convert anyway.
1. Adopt a balanced model — like linear or a position-based model — as your default reporting view, so no channel gets systematically over- or under-rewarded.

**Want me to save this as a project, or is this enough to take into your budget planning?**

>[!ENDSHADEBOX]

#### 4. Turn it into a decision

**You:**

>[!BEGINSHADEBOX]

So how should I allocate budget?

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

Based on what the data shows, here's where I'd focus:

* **Stop judging upper-funnel channels on last touch alone.** Paid social and email start about 20% of your revenue each, but last touch credits them for less than half of that. Protect their budgets — they're creating the demand paid search closes.
* **Treat branded search as a harvester, not a driver.** It closes a lot but starts almost nothing. Test trimming it, since much of that demand may convert through other paths anyway.
* **Make a balanced model your default.** Reporting on linear or a position-based model instead of last touch will stop you from over-rewarding closers and under-funding the channels that start journeys.
* **Re-check after you rebalance.** Watch whether total revenue holds steady as you shift spend toward initiators — that's the signal your funnel is healthier, not just your last-touch report.

Want me to save this as a project so you can track it, or build a calculated metric that reports revenue on a balanced attribution model going forward?

>[!ENDSHADEBOX]

### What just happened

In four plain-language questions, Coworker helped us:

* Attribute revenue to marketing channels and flag that the default last-touch view tells only part of the story
* Compare attribution models and reveal that the "best" channel changes completely depending on how credit is counted
* Discover that paid social and email start far more revenue than they ever get credit for closing
* Identify which campaigns initiate journeys versus close them, and walk away with a budget direction: protect the initiators, right-size the harvesters, and report on a balanced model

-->
