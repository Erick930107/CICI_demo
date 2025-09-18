# 簡易CICD demo
## 操作說明
1. 已於actions介面設定workflow(.github/workflows/test_main.yml)，可再自行客製化。
2. 任何push, pull操作都會觸發workflow，運行檢出程式碼、設定python版本、安裝依賴、運行單元測試等...。
3. 若以上運行皆正常更動沒有造成測試失敗，更動將成功被佈署。

## 操作案例
* 主要包含`main.py`和`test_main.py`，用於模擬真實大型專案中每個程式碼都有專屬的測試。
* 這裡透過新增和更動`test.txt`的內容，確保每次的push都會觸發workflow。
* 另外模擬更動造成測試失敗的案例，以驗證CI/CD能讓錯誤能被及時捕捉和修正。
<img width="1444" height="557" alt="image" src="https://github.com/user-attachments/assets/1d321e8e-eeff-491b-8e3e-df6354ccb265" />

