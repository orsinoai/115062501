# 學生作品 Prototype 展示牆

這是一個可直接部署到 GitHub Pages 的學生作品展示首頁。

## 檔案說明

```txt
student-prototypes-gallery/
├─ index.html          # 首頁與版面
├─ projects.js         # 學生作品資料，只要改這個就能新增作品
├─ .nojekyll           # 讓 GitHub Pages 不使用 Jekyll 處理
└─ assets/
   └─ screenshots/     # 未來可放作品截圖
```

## 如何新增作品

打開 `projects.js`，照下面格式新增一段：

```js
{
  name: "學生姓名",
  time: "10:30",
  title: "作品名稱",
  type: "遊戲 Prototype",
  url: "https://學生帳號.github.io/作品路徑/",
  status: "可展示",
  note: "作品備註"
}
```

注意：每一段物件之間要用逗號 `,` 分隔。

## 如何部署到 GitHub Pages

1. 到 GitHub 建立一個新的 Repository，例如：`student-prototypes-gallery`
2. 把這包檔案全部上傳到 Repository 根目錄
3. 到 Repository 的 `Settings`
4. 左側選 `Pages`
5. Source 選 `Deploy from a branch`
6. Branch 選 `main`，資料夾選 `/root`
7. 儲存後等待 GitHub Pages 產生網址

完成後網址通常會是：

```txt
https://你的帳號.github.io/student-prototypes-gallery/
```

## 顯示模式

首頁右上有「顯示即時預覽 / 只顯示卡片」。

如果作品很多，建議切成「只顯示卡片」，頁面會比較快。

如果某些作品不能在卡片裡預覽，通常是 iframe 限制，不代表作品壞掉，直接點「開啟作品」即可。
