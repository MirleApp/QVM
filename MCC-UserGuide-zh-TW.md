# MCC 使用者指南

在網址列輸入MCC系統網址並開啟MCC網站，進入主畫面。
![MCC網站主畫面](mcc_user_guide_images/2-02_home.png)

---

## 資料收集

選擇時間區間範圍之生產履歷條件進行建模，並點擊Get Piece獲取資料建模筆數。

![MCC建模資料條件篩選頁面](mcc_user_guide_images/2-03_modeling_data_filtering.png)
 
點選Piece Count可以會出現Piece ID列表，可以在此選擇或排除Piece ID，最後點擊Next進入資料參數篩選步驟。

![點擊Piece Count](mcc_user_guide_images/2-04_click_piece_count.png)

![Piece ID 列表](mcc_user_guide_images/2-05_piece_id_list.png)

---

## 資料參數篩選

選擇生產重要參數與量測種類並納入建模模型中，挑選完畢後點擊Next進入資料前處理步驟。

![MCC資料參數篩選頁面](mcc_user_guide_images/2-06_data_parameter_filtering.png)

---

## 資料前處理

設定每個重要參數規格，並透過演算法(Algorithms)設定上下限(USL、LSL、UCL、LCL)規格。

![MCC設定重要參數規格頁面](mcc_user_guide_images/2-07_setting_important_parameter_specifications.png)

顯示單一重要參數之數據。

![MCC顯示單一參數數據頁面](mcc_user_guide_images/2-08_display_single_parameter_data.png)

顯示單一重要參數之趨勢圖。

![MCC顯示單一參數趨勢頁面](mcc_user_guide_images/2-09_displays_a_single_parameter_trend.png)

---

## 演算法參數設定

演算法參數設定名詞說明

| 系統 | 名詞 | 說明 |
|------|------|------|
| **Metrology Setting** | Target | 規格目標 |
| | USL | 規格上限 |
| | LSL | 規格下限 |
| | UCL | 管制上限 |
| | LCL | 管制下限 |
| **DOI<sub>k</sub> Model** | PhaseI Error Threshold | 實際量測值與預測值可容許之誤差上限值 |
| **Neuro Network(NN) Model** | Mom Term Range | 慣性項（momentum term）<br>瞬時誤差的最陡坡降方向加上前一次迭代調整值的某一比例。<br>慣性因子的學習速率，值愈大學習速率較慢。 |
| | Alpha Range | 學習速率<br>值愈小：則收斂過程因此趨緩，但迭代次數就相對地提高；值愈大：可加速搜尋效率，但容易造成搜尋過程中，目標函數產生不穩定的振盪情形。 |
| | Epochs Range | 迭代次數限制<br>值愈大迭代(迴圈)次數愈多 |
| | Nodes Range | 神經元個數 |
| **Reliable Index(RI) Model** | Tolerable Maximum Error | NN 與 PLS 預測值可容許之誤差上限值 |

設定完畢點擊Build建立模型

![MCC演算法設定頁面](mcc_user_guide_images/2-10_algorithm_settings.png)