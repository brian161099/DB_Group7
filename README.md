# DB_Group7
資料庫管理（112-1） 期末專案第7組：國道「事故熱點」回報平台
<br>
本專案在創建一個交通事故資訊整合平臺，融合事故、氣候與交通流量數據，涵蓋系統設計（包括ER圖、資料庫架構與正規化分析）與實作（包括資料庫建置、關鍵功能、SQL指令優化及模擬測試），展現從設計至實現整體流程。
<br>

一、檔案說明
<br>
1.dataset資料夾內容包含:
<br>
(1)Confirm.csv 檔案，使者確認資料。
<br>
(2)EtagObs.csv 檔案，ETag測量站資料。
<br>
(3)GeoLocatingStaticInfo.csv檔案，測量站地理位置等資料。
<br>
(4)Hotspot.csv檔案，經統計整理之事故熱點分析資料。
<br>
(5)Query.csv檔案，查詢紀錄資料。
<br>
(6)User.csv檔案，使用者資料。
<br>
(7)WeatherObs.檔案，氣候觀測站資料。
<br>
2.Highway Traffic Event Schema (Final).drawio 國道事故熱點回報平台Schema圖檔。
<br>
3.Highway Traffic Event ER diagram (Final).drawio 國道事故熱點回報平台ER-diagram圖檔。
<br>
4.README.md 操作手冊文檔。
<br>
5.accident.zip 前端相關程式碼與資源。
<br>
6.final_project.sql 國道事故熱點回報平台資料庫backup檔。
<br>


二、前後端系統說明
<br>
前端目錄結構:
- /figure - 可能用來存儲應用程式中使用的圖片和圖標。
  - admin.png - 管理員圖標。
  - highway.jpg - 用於背景或主題的公路圖片。
  - home_screen.jpg - 應用程式的主屏幕圖片。
  - 等等，包含多個針對特定功能或用戶界面的圖片。

- /src - 主要的源代碼目錄。
  - /vendor - 第三方庫和框架的目錄。

- /js - 存儲JavaScript文件，用於前端邏輯和互動。
  - geolocation.js - 處理地理定位的腳本。
<br>
PHP腳本

- admin_accident_manage.php - 管理員管理交通事故記錄的腳本。
- admin_operation.php - 管理員進行的操作相關的腳本。
- admin_traffic_weather_manage.php - 管理員管理交通和天氣資訊的腳本。
- admin_user_manage.php - 管理員管理用戶帳號的腳本。
- index.php - 應用程式的入口文件或主頁面。
- login_admin.php - 管理員登入界面的腳本。
- login_user.php - 用戶登入界面的腳本。
- login_viewer.php - 觀察者登入界面的腳本。
- signup.php - 用戶註冊界面的腳本。
- signup_success.php - 註冊成功的提示頁面。
- user_confirm_accident.php - 用戶確認事故發生的腳本。
- user_current_accidents.php - 顯示當前事故的腳本。
- user_operation.php - 處理用戶操作的腳本。
- user_query_accidents.php - 用戶查詢事故記錄的腳本。
- viewer_operation.php - 觀察者操作的腳本。
- viewer_query_history.php - 觀察者查詢歷史記錄的腳本。

<br>
其他文件

- composer.json / composer.lock - Composer相關文件，用於管理PHP的依賴項。
- styles.css - 應用程式的樣式表。
- test.php - 用於測試的腳本。


<br>
後端:以PostgreSQL建立之 final_project.sql，內容包含上述dataset中的各個table。
<br>


<br>
三、系統操作
<br>
系統操作參考影片連結:

