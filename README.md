# 分析病人生命跡象數據
我常在新聞中看到來不及急救而死去的人們，引發我想要分析病人生命跡象數據來預測急救，早一步讓醫護做準備以挽救生命。近期大數據和機器學習已廣泛被應用且成效良好。此研究的目的是希望發展一個模組避免加護病房的病人急救。實驗數據使用MIMIC IV 的數據來做分析，經由我的分析數據，最後我達到百分之88.2的準確度。

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
│   └── ...
├── config/                  # 存放設定檔案
└── reports/                 # 存放報告、文檔或投影片等相關資料
```
## 目錄說明：
- `Data/raw`裡面有幾個重要的檔案要載入
    - `chartevents.csv`
    - `procedureevents.csv`
    

```
Johnson, A., Bulgarelli, L., Pollard, T., Horng, S., Celi, L. A., & Mark, R. (2023). MIMIC-IV (version 2.2). PhysioNet. https://doi.org/10.13026/6mm1-ek67.


Johnson, A.E.W., Bulgarelli, L., Shen, L. et al. MIMIC-IV, a freely accessible electronic health record dataset. Sci Data 10, 1 (2023). https://doi.org/10.1038/s41597-022-01899-x


Goldberger, A., Amaral, L., Glass, L., Hausdorff, J., Ivanov, P. C., Mark, R., ... & Stanley, H. E. (2000). PhysioBank, PhysioToolkit, and PhysioNet: Components of a new research resource for complex physiologic signals. Circulation [Online]. 101 (23), pp. e215–e220.
```