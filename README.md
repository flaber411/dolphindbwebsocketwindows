# DolphinDB WebSocket Windows DLL CI/CD

## 使用步驟
1. Fork 本倉庫
2. 點擊 **Actions** → **Build DolphinDB WebSocket Windows DLL**
3. 等待 8-10 分鐘完成
4. **Artifacts** → 下載 `websocket-windows-dll-v2.0.0.zip`
5. 解壓 → 複製 `websocket.dll` 到 `C:\dolphindb\plugins\websocket\`

## 驗證

## 如何刪除 WebSocket 插件

如果您需要移除 DolphinDB WebSocket 插件，請按照以下步驟操作：

1. 停止 DolphinDB 服務器（如果正在運行）
   - 如果作為 Windows 服務運行，請使用服務管理器停止服務
   - 如果從命令行運行，請關閉運行 DolphinDB 的命令提示符窗口
2. 刪除插件文件：
   - 導航到 `C:\dolphindb\plugins\websocket\`
   - 刪除 `websocket.dll` 文件
3. （可選）刪除整個插件目錄：
   - 刪除 `C:\dolphindb\plugins\websocket\` 資料夾
4. 重新啟動 DolphinDB 服務器（如果需要）

**注意：** 刪除插件後，任何依賴 WebSocket 功能的腳本或應用程式將無法正常工作。
