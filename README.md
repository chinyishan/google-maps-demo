# Google Map Demo

## 專案簡介

本專案主要練習如何在前端專案中整合 Google Maps JavaScript API，實作地圖渲染、標記 (Marker) 放置、資訊視窗 (InfoWindow) 展示，以及基本的地圖互動控制。
同時測試不同參數設定，了解地圖自訂化與最佳化技巧，作為後續地圖應用開發的基礎練習。

## Demo 連結

<a href="https://chinyishan.github.io/google-maps-demo/" target="_blank">網站連結</a>

## 使用技術

1. Google Maps Javascript API
2. Vue.js
3. D3.js
4. Echart

## 建立地圖 google.maps.Map 參數

### center

- 中心點座標

### zoom

- 1-20，數字愈大，地圖愈細：1 是世界地圖，20 就會到街道

### mapTypeId

- roadmap 顯示默認道路地圖視圖。
- satellite 顯示 Google 地球衛星圖像。
- hybrid 顯示正常和衛星視圖的混合。
- terrain 顯示基於地形信息的物理地圖。

### Code

```
this.map = new google.maps.Map(document.getElementById("map"), {
  center: new google.maps.LatLng(2.8, -187.3), // 中心點座標
  zoom: 16, // 1-20，數字愈大，地圖愈細：1是世界地圖，20就會到街道
  mapTypeId: "terrain",
});
```

## 設置多個標記 Marks

### map.geojson

- geojson 檔案是用於紀錄地理資訊 JSON

### Code

```
new google.maps.marker.AdvancedMarkerElement()
```

### 改地圖樣式

https://mapstyle.withgoogle.com/

# D3.js SVG 台灣

## 繪製 SVG 圖形

```jsx
// 將圖形儲存以利後續使用
const svg = d3
  // 選擇一個畫面上元素作為容器
  .select("#chart")
  // 設定要新增的標籤名稱
  .append("svg")
  // 設定svg的width屬性
  .attr("width", 600)
  // 設定svg的height屬性
  .attr("height", 400);
```
