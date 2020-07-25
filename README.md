# Laravel 7 Bugsnag 錯誤監控和紀錄

引入 bugsnag 的 bugsnag-laravel 套件來擴增使用 Bugsnag 監控應用程序的運行狀況，了解錯誤影響的發生次數和用戶數量有助於你確定錯誤的優先級；將所有診斷數據存儲在一個地方，使您能夠快速重現和修復錯誤；追蹤穩定性指標讓您評估應用程序版本的性能。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 在瀏覽器中輸入已定義的路由 URL 來訪問，例如：http://127.0.0.1:8000。

## 畫面截圖
![](https://i.imgur.com/NoHIhOf.png)
> 觸發錯誤例外以中斷程式流程

![](https://i.imgur.com/BFtZLqI.png)
> 使用 Bugsnag 確認程式錯誤的偵測
