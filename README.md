# PRSM — Predictive Retail Survival Model

> AI 選址存活診斷引擎｜輸入地址，即時評估開店風險

## 🌐 Live Demo

**[→ 立即體驗 PRSM 診斷工具](https://bw5168.github.io/prsm-demo/interactive.html)**

---

## 什麼是 PRSM？

PRSM 是一套專為零售選址設計的風險預測模型，核心指標為**營租比 OLR（Operating Leverage Ratio）**。

透過輸入候選地點的地址、租金與預估營收，PRSM 能在 3 秒內輸出：

- ✅ 當前存活分數（OLR）
- ⚡ 壓力測試（人流下降 20% 情境）
- 💊 生存處方箋（建議安全租金、科學議價空間）
- 📄 PDF 報告一鍵下載

---

## 判斷邏輯

| OLR 分數 | 狀態 | 說明 |
|----------|------|------|
| ≥ 1.3 | ✅ 安全 | 營收足以支撐租金，具擴張潛力 |
| 1.0 ~ 1.3 | ⚠️ 警示 | 邊際存活，需控制成本或議租 |
| < 1.0 | ❌ 危險 | 租金壓力過大，建議重新評估 |

---

## 技術架構
```
前端 (GitHub Pages)     後端 (Google Cloud Run)
interactive.html   →   PRSM API (Python)
                        ├── OLR 計算引擎
                        ├── 壓力測試模組
                        └── CORS 支援
```

- **前端：** 純 HTML/CSS/JavaScript，無框架依賴
- **後端：** Python + Functions Framework，部署於 Google Cloud Run
- **API 端點：** `https://retail-survival-api-859868518848.asia-east1.run.app`
- **引擎版本：** PRSM-V2-Pro

---

## 應用場景

- 🏪 **連鎖品牌展店評估**（路易莎、cama café、85度C）
- 🏢 **商業不動產租賃決策**
- 🤝 **房仲科學議價工具**
- 📊 **加盟主選址風險評估**

---

## 商業合作

本工具後端 API 可授權串接，歡迎洽談：

- 連鎖品牌展店系統整合
- 房仲平台 API 授權
- 企業客製化版本

> Powered by PRSM-V2-Pro｜Shield Voice Technology
