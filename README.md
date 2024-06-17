# Google Map Demo

## 使用技術

1. Google Maps Javascript API
2. Vue.js
3. Bootstrap4

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
new google.maps.marker.AdvancedMarkerElement({})
```
