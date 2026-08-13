# 微软式中文翻译器 (Microsoft-Style Chinese Translator)

一个基于 DeepSeek API 的趣味翻译工具，可将中文、英文和“微软式中文”进行相互转换，体验微软软件本地化中独特的拗口、正式且略带幽默的语言风格。

## ✨ 功能特色

- 🌐 支持 **中文**、**英文**、**微软式中文** 三种语言的互译
- 🤖 基于 DeepSeek 大语言模型，翻译自然且符合风格
- 🔄 **智能同语言处理**：当输入与输出语言相同时，直接返回原文，不消耗 API 配额
- 📋 一键复制翻译结果
- 🎲 随机示例快速体验
- ⌨️ 键盘快捷键 `Ctrl+Enter` 快速翻译
- 🎨 毛玻璃 UI 风格，响应式设计，适配移动端
- 📝 完全开源，可自由修改和部署

## 🚀 在线体验

您可以直接访问 GitHub Pages 或 Vercel 等平台部署后的版本。  
（*如果未配置 API 密钥，页面将提示您填入密钥*）

## 📦 本地运行

1. 克隆仓库到本地

2. 在浏览器中打开 `index.html` 即可使用（无需额外服务器）。

> **注意**：为了使用翻译功能，您需要配置自己的 DeepSeek API 密钥（见下文）。

## 🔑 配置 API 密钥

1. 前往 [DeepSeek 平台](https://platform.deepseek.com/api_keys) 注册并获取您的 API 密钥。
2. 打开 `index.html`，找到文件顶部的 JavaScript 配置区域：
   ```javascript
   // ============================================================
   //  配置区域 - 请在此填入您的 DeepSeek API 密钥
   // ============================================================
   const API_KEY = 'YOUR_DEEPSEEK_API_KEY_HERE'; // 替换为您的实际密钥
   const API_URL = 'https://api.deepseek.com/v1/chat/completions';
   const MODEL = 'deepseek-chat';
   // ============================================================
   ```
3. 将 `YOUR_DEEPSEEK_API_KEY_HERE` 替换为您的真实密钥。

> **安全提示**：请不要将包含密钥的代码提交到公开仓库。建议使用环境变量或后端代理。本示例仅为演示，生产环境请务必隐藏密钥。

## 🛠️ 技术栈

- **前端**：纯 HTML5 + CSS3 + JavaScript (ES6)
- **UI 框架**：无依赖，自定义样式，Font Awesome 图标库
- **API**：DeepSeek Chat Completions API
- **部署**：静态文件，可直接托管于任何 Web 服务器

## 📖 使用指南

1. **选择输入语言**：从“输入”下拉菜单中选择源语言（中文、英文、微软式中文）。
2. **选择输出语言**：从“输出”下拉菜单中选择目标语言。
3. **输入文本**：在文本框中输入待翻译或润色的内容。
4. **执行翻译**：点击“翻译”按钮或按 `Ctrl+Enter`。
   - 如果输入输出语言相同，将直接显示原文（无 API 调用）。
   - 如果不同，将调用 DeepSeek API 进行翻译。
5. **查看结果**：翻译结果会显示在下方“结果”区域。
6. **复制结果**：点击“复制”按钮或直接点击结果框即可复制译文。
7. **清空内容**：点击“清空”按钮重置输入和结果。
8. **随机示例**：点击“随机示例”快速填入一个示例句子，并自动匹配输入语言。

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！如果您有改进建议或发现了 bug，请随时参与。

1. Fork 本仓库
2. 创建您的特性分支 (`git checkout -b feature/amazing-feature`)
3. 提交您的修改 (`git commit -m 'Add some amazing feature'`)
4. 推送到分支 (`git push origin feature/amazing-feature`)
5. 打开一个 Pull Request

## 📄 许可证

本项目采用 [MIT 许可证](LICENSE)，您可以自由使用、修改和分发，但请保留原始版权声明。

---

**Enjoy the “Microsoft-style” translation! 😄**  
*该页面可能正在执行“错误”操作，但您的翻译请求已成功被处理。*

