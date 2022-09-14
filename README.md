# CCU MVL Website
- [CCU MVL Website](#ccu-mvl-website)
  - [基本說明](#基本說明)
  - [GitHub 更新維護規定](#github-更新維護規定)
  - [專案資料夾架構](#專案資料夾架構)
  - [Site Map](#site-map)
  - [開發團隊](#開發團隊)
  - [TODO List](#todo-list)

## 基本說明
這份文件為中正大學機器視覺與學習實驗室的網站相關規定說明。
- 網站預設網址為 [https://ccumvllab.github.io/](https://ccumvllab.github.io/)
- 本網站為利用 GitHub Pages 來建立靜態網站，並以 [Themefisher Meghna Template v1.0](https://themefisher.com/products/meghna) 建立基本架構及美術編排。

## GitHub 更新維護規定
- 此網站建立在 GitHub Pages 之上，而 GitHub Pages 會抓取 [ccumvllab.github.io](https://github.com/ccumvllab/ccumvllab.github.io) 專案中的 `index.html` 當作預設開啟網頁，而在此網頁中自動導向到真正的網站連結，此網站的內容如下，[https://ccumvllab.github.io/new-site](https://ccumvllab.github.io/new-site) 就是真正的網站連結。
    ```html
    <!DOCTYPE html>
    <html>
    <head>
        <meta http-equiv="Refresh" content="0;url=https://ccumvllab.github.io/new-site">
    </head>
    </html>
    ```
- 更新規定:
  - ***不能直接更新 `ccumvllab/ccumvllab.github.io` 或 `ccumvllab/new-site` 兩個專案的內容，`ccumvllab/ccumvllab.github.io` 的內容非必要不得更動！！！***
  - 更新步驟
    1. 請先 `fork` 到個人的帳號底下
    2. 用個人帳號的專案進行更新
    3. 更新完成後使用 `pull request` 將變更合併回 `ccumvllab/new-site`

## 專案資料夾架構
```
ccumvllab/new-site
|
|------ blogs/  # 佈告欄的所有相關照片、網頁皆放於此
|       |
|       |------ 20220824/               # 活動資料夾，以日期為命名
|       |       |------ 20220824-1.jpg  # 活動照片，以資料夾名及編號為命名
|       |       |------ 20220824.html   # 活動網頁，以日期為命名
|       |       |______ ...
|       |------ blog.html   # 過往活動紀錄
|       |______ ...
|
|------ css/
|       |
|       |------ style.css       # 網頁中的風格皆於此編輯
|       |______ style.css.map   # 不重要
|
|------ images/ # 網站中其餘圖片皆存放於此
|       |
|       |------ banner/     # 網站封面頁背景圖片
|       |------ research/   # 研究說明相關圖片
|       |------ team/       # 實驗室成員個人照
|       |       |
|       |       |------ Graduated/      # 畢業成員個人照
|       |       |------ Master Student/ # 碩士班成員個人照
|       |       |------ Phd Student/    # 博士班成員個人照
|       |       |------ chen.kuo.chiang-225x225.jpg # 江振國個人照
|       |       |______ default.png     # 預設個人照，只限於尚未提供照片的成員使用
|       |______ logo.png    # 網站 Logo
|
|------ js/
|       |
|       |______ script.js   # javascript 相關程式，含動畫程式
|
|------ plugins/    # 模板相關檔案，建議勿動
|------ .gitignore  # 不要被 git 的清單
|------ graduated-students.html # 畢業成員清單介面
|------ index.html  # 網站主要網頁
|------ LICENSE/    # MIT 授權規定
|------ README.md   # 本說明文件
|______ research.html   # 實驗室研究說明網頁
```
## Site Map
```
index.html
|
|------ Research
|       |______ research.html
|
|------ News
|       |------ 20220824.html
|       |------ ...
|       |______ blog.html
|
|------ Members
|       |______ graduated-students.html
|
|------ Contact
|
|______ Old Website (https://ccumvllab.github.io/site/)
```

## 開發團隊
- 林岳 `lyjeff` : 建立及維護新網站
- 李皓庭 `aquastripe` : 維護網站
- 李昀倫 `apie0419` : 更新維護舊網站
- `egoistclaris` : 建立及維護舊網站

## TODO List
- 新成員個人照
- 更新研究說明
- 加入課程頁面
- 完全英文化