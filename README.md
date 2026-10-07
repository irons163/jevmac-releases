# jevmac

原生 macOS Jev 操作助手，可觀察指定 App／視窗，依任務選擇輸入或按下控制項，再核對操作結果。提供逐步確認、有界自動模式與唯讀工作台。

## 下載與安裝

**[下載最新版本](https://github.com/irons163/jevmac-releases/releases/latest)**

**Apple Silicon 與 Intel 使用同一份 Universal ZIP。** 同一個 App 包含 arm64 與 x86_64 架構。

1. 下載最新 Release 中的 ZIP 安裝包並解壓。
2. 將 `jevmac.app` 移至「應用程式」後開啟。
3. 在 macOS「系統設定 → 隱私權與安全性 → 輔助使用」加入並啟用 jevmac。
4. 在 App 的「唯讀工作台／API Key」儲存自己的 TypeSafe AI API Key，再切回「操作助手」選擇目標 App 與任務。

需要 macOS 14 或更新版本。正式版本使用 Developer ID Application 簽章、通過 Apple 公證並附加票證，Gatekeeper 驗證通過。新版由 GitHub Actions 建置與發布；下載頁附有版本說明、`manifest.json` 與 `SHA256SUMS`，可核對建置來源及檔案完整性。此為直接下載版本。

## 操作與資料

- 操作前可檢查送給 TypeSafe AI 的 JSON；API Key 存於本機 macOS Keychain。
- 只輸入使用者指定的文字；替換會覆蓋整個欄位。
- 可逐步確認或設定有操作次數與時間上限的自動模式，並隨時停止。
- 自動化範圍取決於目標 App 的 Accessibility 能力；遇到新視窗、缺少能力或不確定結果會停止或請求協助。
- 不承諾任意 App 全自動完成。現有實機測試在 Apple Silicon 完成；獨立 Intel Mac 與全新使用者環境尚未完成實機測試。

請勿在 Issues 貼上 API Key、Apple 密碼或私人畫面內容。詳細功能、驗證與限制請參閱各版本的 Release 說明。ZIP 附有 `THIRD_PARTY_NOTICES.txt`。

此儲存庫只提供下載與版本說明。
