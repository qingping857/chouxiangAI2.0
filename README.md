# 抽象AI 对话网站

这是一个基于 [Next.js](https://nextjs.org) 14 开发的现代化 AI 对话网站，使用 DeepSeek API 实现智能对话功能。我们的 AI 助手充满中国互联网文化特色，极度"抽象"且搞笑。

## 功能特点

- 简约现代的用户界面，采用 Twitter 风格的设计
- 使用 DeepSeek API 实现实时 AI 对话功能
- AI 助手精通中文互联网梗和表情包，回答极度"抽象"
- 响应式设计，完美适配各种设备
- 优雅的动画效果
- AI 回复附带经典的"滑稽"表情头像，增添趣味性

## 开始使用

首先，确保你的 Node.js 和 npm 是最新版本。然后，按照以下步骤安装依赖：

```bash
npm install
npm install openai
```

如果遇到模块导入问题，请尝试以下步骤：

1. 删除 `node_modules` 文件夹和 `package-lock.json` 文件（如果存在）。
2. 重新运行 `npm install`。

然后，运行开发服务器：

```bash
npm run dev
```

在浏览器中打开 [http://localhost:3000](http://localhost:3000) 体验抽象AI。

## AI 个性

我们的 AI 助手是一个充满"抽象"元素的搞笑角色：

- 精通中国互联网文化和流行梗
- 喜欢使用各种表情包描述（如狗头🐶、滑稽😏等）
- 经常使用网络流行语和"抽象话"
- 会玩文字游戏和谐音梗
- 有时会模仿网络红人或虚拟角色的说话方式

与抽象AI聊天，你会感受到一种独特的、充满中国互联网特色的幽默体验！

## 项目结构

- `app/page.tsx`: 主页面组件，采用动态导入加载聊天界面
- `components/ChatInterface.tsx`: 聊天界面组件，使用客户端渲染，集成 DeepSeek API
- `app/api/chat/route.ts`: API 路由，处理与 DeepSeek API 的通信
- `styles/`: CSS 样式文件目录
- `lib/`: 工具函数和 API 调用目录
- `public/`: 存放静态资源，如图片等
  - `huaji.png`: AI 回复使用的滑稽表情头像
- `next.config.js`: Next.js 配置文件，包含 webpack 配置

## 技术栈

- Next.js 14
- React
- TypeScript
- Tailwind CSS（用于现代化的样式和动画）
- OpenAI（用于与 DeepSeek API 交互）

## 设计理念

抽象AI 采用简约而现代的设计风格，灵感来源于 Twitter 的界面设计。使用黑色背景配合白色线条边框，营造出简洁而高端的视觉效果。蓝色作为强调色，为界面增添活力。整体设计旨在突出AI的"抽象"个性，为用户带来轻松愉快的对话体验。

## 注意事项

本项目使用 DeepSeek API 进行 AI 对话。请确保您有有效的 API 密钥，并在使用前正确配置。

## 环境设置

在项目根目录创建一个 `.env.local` 文件，并添加以下内容：

```
DEEPSEEK_API_KEY=你的DeepSeek_API密钥
```

确保将 `.env.local` 添加到 `.gitignore` 文件中，以防止 API 密钥被意外提交。

## 贡献

我们欢迎各种形式的贡献！无论是添加新的中国互联网梗，优化AI的"抽象"表现，还是改进用户界面，都请随时提出建议或提交 pull request。

## 许可证

本项目采用 [MIT](https://opensource.org/licenses/MIT) 许可证。
