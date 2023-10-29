# mod-ChenRabbitMqSeting-1_MDD
---

# 壹、模組說明
提供建置RabbitMQ container指引

# 貳、DevOps說明
## 一、Code階段
* 編輯docker-compose.yml（含修改帳密）
* 編輯README.md

## 二、Release階段
* 將上述檔案打包發佈至Release載點

## 三、Deployment階段
* 安裝[Docker Desktop](https://www.docker.com/products/docker-desktop/)，包含docker及docker compose主程式。
* 將發佈檔案複製至執行環境後，執行下列指令
```sh
docker-compose up -d

參數說明
-d：背景模式，視需要使用
```
* 開啟Docker Desktop Dashboard確認Container執行狀況。
* 開啟瀏覽器連接(http://localhost:15672)管理頁面，確認執行正常（帳密參見docker-compose）。

## 四、Operation階段
* 另自製軟體連接RabbitMQ存取訊息佇列。

## 五、Monitor階段
* 開啟瀏覽器連接(http://localhost:15672)管理頁面，掌握執行狀況。
