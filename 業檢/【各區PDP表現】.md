### 操作步驟
- Step1: 清空 **DataSource** 表格中的數據
- Step2: 到 Access 中找到 **業檢 - 區域中心分組PDP**，需要檢查或設定如下查詢
    - 業檢 - 區域中心分組PDP
    - 業檢 - 區域中心分組PDP(新戶)
    - 業檢 - 區域中心分組PDP(總收益及存放款)
- Step3: 設定 **業檢 - 區域中心分組PDP(總收益及存放款)** 中 **年月** 為 **Between 去年第一個月 And 去年當前月**
    - "Betwween 202501 And 202503"
- Step4: 匯出 **業檢 - 區域中心分組PDP** 查詢為 excel 檔案，並複製數據到 **DataSource** 表格中