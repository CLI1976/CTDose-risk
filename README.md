# CT Dose to mSv Estimator

本專案提供一個簡單的網頁工具，用於計算 CT 檢查的 DLP（劑量長度乘積）轉換為等效劑量（mSv），並估算基於 BEIR VII 報告的終生癌症可歸因風險（LAR）。

## 🔹 功能
- 根據 DLP、CT 部位與年齡組別估算等效劑量 (mSv)
- 依線性無閾值假設 (LNT model) 估算終生癌症可歸因風險 (LAR)
- 計算約需多少患者接受該劑量輻射，統計上平均會產生 1 例輻射誘發癌症
- 提供簡單直觀的數值視覺呈現與風險說明

## 📊 技術細節
- 前端純 HTML + CSS + JavaScript
- 劑量轉換參數基於 AAPM TG204、TG96 報告
- LAR 基準值：BEIR VII 50 歲成年人全癌症 1.065% per 100 mSv

## 📝 使用說明
1. 輸入 Total DLP 數值 (mGy·cm)。
2. 選擇 CT 掃描部位。
3. 選擇年齡組別。
4. 點選 **Calculate** 按鈕，系統會顯示劑量與風險估算結果。

## ⚠ 注意事項

❗ **本工具估算結果僅供群體統計風險參考，不能作為個人癌症風險診斷或預測之用。**

🔬 本工具採線性無閾值假設（LNT model）進行風險推估，可能與實際風險落差甚大。

實際風險可能因個人年齡、性別、體質、生活型態等因素而有所不同。

## 📚 參考資料
- [AAPM Report 96 (TG 204)](https://www.aapm.org/pubs/reports/RPT_96.pdf)
- [BEIR VII Phase 2 Report](https://nap.nationalacademies.org/read/11340/chapter/14)

## 💡 
此工具為教育用途設計。  
若有建議或問題，歡迎開 issue 或提交 pull request。
