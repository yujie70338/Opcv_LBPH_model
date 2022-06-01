# Opcv_LBPH_model
OpenCV 製作影像辨識登入系統
* 需要套件:CV2、numpy
* 需要設備:攝影機
---
目前專案分成兩隻程式碼  
  1. 註冊帳號 register.py
  2. 登入系統 Login.py  
---
register.py 會自動開啟您的攝影機，並拍100張照片，存於images資料夾內，並且利用cv2內建的Local Binary Pattern Histogram 演算法建立模型，並且存檔faces_LBPH.yml於當前目錄。

---
Login.py 會自動開啟您的攝影機，並拍1張照片，存於media資料夾內，按下Z鍵拍照或是等待五秒後自動拍照，並且讀取模型檔faces_LBPH.yml判斷信心值。
