# 效果量的計算方法 {#effectsize}

本書取用及建議的再現實驗實驗，設計都是比較兩組參與者表現的參與者間設計(Between Participant Design)，以及比較同一位參與者在兩種情況表現的參與者內設計(Withing Participant Design)。兩種設計的效果量都是計算Cohen's d，只是計算公式並不相同。

雖然本書推薦的統計軟體都有計算Cohen's d的功能，為了未來學習設計更複雜的實驗，讀者還是有必要了解如何計算。 @lakens_calculating_2013 整理兩種Cohen's d的計算方法，節錄如下：

- 參與者間設計 Cohen's $d_s$

需要數值：兩組平均值($\bar{X}_1$, $\bar{X}_2$)，兩組樣本變異數($SD^2_1$, $SD^2_2$)，兩組樣本人數($n_1$, $n_2$)。

$$d_s = \frac{\bar{X}_1 - \bar{X}_2}{\sqrt{ \frac{(n_1 - 1)SD^2_1 + (n_2 - 1)SD^2_2}{n_1 + n_2 - 2}}}$$


- 參與者內設計 Cohen's $d_Z$

需要數值：差異分數平均值($M_{diff}$)，每位參與者的差異分數($X_{diff}$)，參與者人數(N)。

$$d_z = \frac{M_{diff}}{\sqrt\frac{\sum(X_{diff} - M_{diff})^2}{N - 1}}$$

# 預估隨機化實驗的樣本人數 {#sampling}

規劃一項實驗之前，必須根據可測得的效果量以及預期達到的考驗力，規劃能得到如此結果的樣本人數。在許多實驗研究法教材培養的研究執行能力，包括軟硬體安排實現設計的完整度，以及執行與解釋資料分析符合學術規範。為了增加研究的可重製性，新手研究者應當在學習如何規劃的時期，了解執行實驗應收集的樣本人數。這個單元以**形態模擬效應**為範例，說明如何考慮估計樣本人數的重要資訊，以及示範操作程序。

@zwaanParticipantNonnaiveteReproducibility2017 招募80位參與者，再現 @ZwaanLanguageComprehendersMentally2002 的研究結果。80位是不是合理的樣本人數，可運用過去研究文獻的效果量資料，評估再現實驗若能發現相同的結果，所達到的考驗力。 @ZwaanRevisitingMentalSimulation2012 曾進行兩次招募176人的實驗，雖然也得到顯著的結果，測得的效果量(.15, .18)只有 @ZwaanLanguageComprehendersMentally2002 的一半(.31)。要評估 @zwaanParticipantNonnaiveteReproducibility2017 招 募的人數，最適當的方式是假設以此實驗方法測得的**形態模擬效應**，效果量範圍在.15到.31之間，評估達到考驗力.80或.90時的人數。


# jPower操作示範 {#power-estimation}

只有兩組比較的參與者間設計或參與者內設計，可運用jPower評估參與者人數。讀者可參考以下影片，了解如何合理評估**形態模擬效應**再現研究的樣本人數：

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/CJwvc9C3Cw4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

將估計樣本人數的思維換個方向，當我們不清楚可能測得的效果量，只有計畫收集的樣本人數，例如第一次進行中文版**形態模擬效應**實驗。只要更換計算項目，就可估計收集的資料如果通過顯著性檢定，應測得至少多小的效果量，才能達到預期的考驗力。這種方法稱為**敏感度分析**，讀者可參考以下影片：

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/NsOO5w_1peo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

請留意影片最後的提醒，以上示範的**敏感度分析**，如果是事後進行，必須確定不再收集資料，分析結果才有意義。詳細說明可參考Daniel Lakens的線上課程"[Improving your statistical inferences](https://zh-tw.coursera.org/learn/statistical-inferences)"之單元5.2~"Sample Size Justification"。


# 心理學實驗操作學習資源 {#learning-resource}

[psytoolkit學習筆記](https://hackmd.io/s/S1WIz64IE)
