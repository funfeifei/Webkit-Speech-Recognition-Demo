# Webkit Speech Recognition Demo

这是一个使用 Web Speech API 的简单语音识别和文字转语音演示。

## 功能

- 使用浏览器原生的语音识别 API（Speech to Text）
- 支持连续监听和中间结果显示
- 设置为中文识别
- 显示最终结果和中间结果
- 文字转语音功能（Text to Speech）
- 支持中文语音合成
- 语音选择：可选择不同的音色和语言

## 使用方法

1. 安装依赖：
   ```
   npm install
   ```

2. 启动服务器：
   ```
   npm start
   ```

3. 在浏览器中打开 http://localhost:8080

### 语音识别（Speech to Text）
4. 点击 "Start Listening" 按钮并对着麦克风说话
5. 点击 "Stop Listening" 停止监听
6. 识别结果会实时显示在页面上

### 文字转语音（Text to Speech）
7. 从语音下拉菜单中选择想要的音色
8. 在文本框中输入要朗读的文字
9. 点击 "Speak Text" 按钮开始朗读
10. 点击 "Stop Speaking" 停止朗读

## 注意事项

- 需要麦克风权限（语音识别）
- 在本地开发时使用 HTTP 即可，但在生产环境中需要 HTTPS
- 支持的浏览器：Chrome, Firefox, Safari 等现代浏览器
- 识别和合成语言设置为中文 (zh-CN)

## 兼容性

此演示使用 `window.SpeechRecognition` 或 `window.webkitSpeechRecognition` 以及 `speechSynthesis`，以确保在不同浏览器中的兼容性。