# 操作步驟
- Step1: 找到 **YYYY RM預算及收益(公式).excel** 並打開
- Step2: 找到 **底稿** 工作表中標記的 **DataSource**
- Step3: 到 Access 中找到 **業檢 - RM業務動能-預算、收益、存放** 查詢
    - 基本上無需設定參數
    - 如果不放心，可以打開某一支 **子查詢** 來查看
- Step5: 將 **底稿工作表中 DataSource 表格** 中的數據做清除
- Step6: 匯出該查詢為 excel 檔案，並複製
- Step7: 將剛複製的數據，**貼上值** 到 **底稿工作表中 DataSource 表格** 
- Step8: 回到 **底稿** 中 **【KPI人力招募】工作表** 中的 **業檢 - 人員名單(RM)** 表格，檢查是否有人員 **離職或派任**
- Step9: 如果有 **人事異動** 就需要回到 **YYYY RM預算及收益(公式).excel** 中的 **YYYY RM預算及YTM收益** 工作表修正數據
    - 新增行的時候，不要在 **表頭、表尾** 做新增，因為會發生公式錯誤的問題
    - **派任情況**
        - 找到該 **RM人員** 所屬的 **區域中心** 表格後 **新增一行**
            - 注意！！！ **新增空白列時**，不能在 **表頭、表尾** 做新增，不然會發生公式跑掉的問題
        - 複製 **正確的人員類別** 的數據到 **空白列** 中，並將該 **RM 人員** 的 **區域代碼、RM員編、區域中心、RM姓名** 為正確的 **人事異動的RM人員** 資料(去底稿找該名人員的數據)。
            - 如果該 **RM 人員** 是 **區主管** 就複製 **區主管** 的數據。
            - 如果該 **RM 人員** 是 **區副主管** 就複製 **區副主管** 的數據。
            - 如果該 **RM 人員** 是 **一般 RM人員** 就複製 **一般 RM人員** 的數據。
            - 因為 **區主管、副主管、RM人員** 的公式不一樣
                - 廣義RM：包含副主管、RM人員
    - **離職情況：**
        - 如果該離職人員有績效不需要隱藏，添加上 **灰色字體** 顏色。 
        - 如果該離職人員沒有績效(數值都是0)，會選取離職人員 **整列數據**，並點擊 **Delete** 清除資料後並隱藏該行。

# 檢查數字是否正確
- **總收益**：找到 **底稿** 中 **【各區PDP表現】** 中 **總收益(mln)** 欄位值，去檢查每個區域中心的 **區域中心合計** 值是否正確
    - **法金總處合計的總收益**：找到 **底稿** 中 **【各區PDP表現】** 中 **總收益欄位的合計（區域中心合計）** 欄位值，去檢查值是否正確
- **放款**(BQ欄位)：到 **底稿** 中 **資產結構by信評** 中 **YYYYMM放款均額含催(mln)** (當前月)欄位值，去檢查每個區域中心的 **區域中心合計** 值是否正確
    - **法金總處合計的存款**：對應 **資產結構by信評** 中 **YYYYMM放款均額含催(mln)** (當前月)欄位的合計
- **存款**(CG欄位)：到 **底稿** 中 **資產結構by信評** 中 **YYYYMM存款均額(mln)** (當前月)欄位值，去檢查每個區域中心的 **區域中心合計** 值是否正確
    - **法金總處合計的存款**：對應 **資產結構by信評** 中 **YYYYMM存款均額** (當前月)欄位的合計

# 備註
- 注意！！！ **新增人員** 的時候，要放在該 **所屬主管的下方**，
- 整個弄完之後，告訴 **京哥** 要維護 **DM、新戶、新貸**
