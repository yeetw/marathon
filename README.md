# 阿胖呆跑跑

網站：https://marathon.yeekuo.tw

與 read 專案相同，使用 GitHub Pages / Jekyll 的 `_data` YAML 資料。

## 新增或修改賽事

直接編輯 [`_data/races.yml`](_data/races.yml)，提交至 main 後會自動發布。
頁面無新增或編輯功能，也不讀取瀏覽器本機儲存的資料。

```yaml
- date: "2027-01-10"
  name: "渣打臺北公益馬拉松"
  distance: 21.0975
  limit: 210
  time: "05:20"
  start: "凱達格蘭大道"
  finish: "大佳河濱公園"
  fee: 1235
  website: ""
  route: ""
  tags: ["大佳河濱"]
```

- `date`：賽事日期，YYYY-MM-DD，保留引號。
- `distance`：公里數，單位 K。
- `limit`：限時分鐘，未提供可填 0；配速自動計算。
- `time`：起跑時間，HH:MM，保留引號。
- `start` / `finish`：起點與終點；終點可填「同起點」。
- `fee`：報名費，數字。
- `website` / `route`：官方網站與路線圖的 http/https 連結，未填用空字串。
- `tags`：自訂標籤；搜尋支援名稱、起終點與標籤。無標籤填 `[]`。

過往／即將起跑、倒數與最長距離，依臺灣當天日期自動計算。
瀏覽器以前自行新增或修改的資料不會自動寫入 YAML，需要補入此檔。

字型為 jf open Huninn，授權文件位於 fonts/OFL.txt。
