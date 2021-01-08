- [安裝(Window)](#安裝window)
  - [設置環境變數](#設置環境變數)
  - [檢測環境](#檢測環境)
  - [Android Studio](#android-studio)
    - [安裝 Plugin (Flutter & Dart)](#安裝-plugin-flutter--dart)
- [Create Project(vscode)](#create-projectvscode)

## 安裝(Window)

參考: [官方](https://flutter.dev/docs/get-started/install/windows)

### 設置環境變數

解壓縮至想要的路徑 (EX: D:\flutter)
於 Path 新增 D:\flutter\bin

### 檢測環境

執行 `flutter doctor`

### Android Studio

安裝流程照推薦的配置裝好即可，會幫你裝好最新的 Android SDK

#### 安裝 Plugin (Flutter & Dart)

Android Studio > config > plugin

搜尋 flutter 並安裝即可(會幫你連 Dart 都裝)

到這再執行 `flutter doctor` 還是會出錯的話

解法參考: [這裡](https://stackoverflow.com/a/65129643/5134658)

就是把 channel 轉到 dev 就好 (可以 `flutter channel` 查看有哪些)

```bash
flutter channel dev
flutter upgrade
```

## Create Project(vscode)

參考: [官方](https://flutter.dev/docs/get-started/test-drive?tab=vscode)

創建好後，於右下角選擇要連接的模擬器 (若沒有，要去 Android Studio > AVD Manager 新增)

這階段可能會連不上，可以嘗試關閉模擬器、vscode => 開啟 vscode 再次選取看看 (不先開啟模擬器)

連接好後，可以執行 flutter run 來開始撰寫專案了
