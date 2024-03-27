# 分析病人生命跡象數據


## 專案根目錄結構：
```
project/
├── Data/
│   ├── raw/                 # 存放原始資料檔案
│   ├── preprocessed/        # 存放處理後的資料檔案
│   └── resampled            # 存放平衡正偽的資料
├── src/                     # 存放程式碼
│   ├── data/                # 存放資料讀取或轉換的程式碼
│   ├── models/              # 存放機器學習模型的程式碼
│   ├── utils/               # 存放共用的工具程式碼
│   └── ...                  # 其他程式碼相關的子目錄
├── config/                  # 存放設定檔案
├── results/                 # 存放實驗結果、日誌等輸出檔案
├── reports/                 # 存放報告、文檔或投影片等相關資料
└── ...                      # 其他專案相關的子目錄
```
## 目錄說明：
- `Data/raw`裡面有幾個重要的檔案要載入
    - `chartevents.csv`
    - `chartenevt_part1.csv` 為上一個檔案的小型檔案
    - `procedureevents.csv`
