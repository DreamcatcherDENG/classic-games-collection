# 经典游戏合集

一个包含10个经典游戏的合集，可部署到 GitHub Pages。

## 🎮 游戏列表

1. **贪吃蛇 (Snake)** - 控制蛇吃食物，避免撞墙或自身
2. **俄罗斯方块 (Tetris)** - 旋转下落方块，消除完整行
3. **乒乓球 (Pong)** - 双人对战乒乓球游戏
4. **太空侵略者 (Space Invaders)** - 射击外星人，避免被击中
5. **吃豆人 (Pacman)** - 在迷宫中吃豆子，躲避幽灵
6. **扫雷 (Minesweeper)** - 点击安全格，避免地雷
7. **数独 (Sudoku)** - 填写数字，避免重复
8. **纸牌 (Solitaire)** - 移动纸牌到基础堆
9. **Flappy Bird** - 点击使鸟飞过管道
10. **打砖块 (Breakout)** - 用球击碎所有砖块

## 🚀 部署到 GitHub Pages

### 自动部署（推荐）

1. **创建 GitHub 仓库**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/your-username/games.git
   git push -u origin main
   ```

2. **启用 GitHub Actions 自动部署**
   - 自动部署工作流已配置在 `.github/workflows/deploy.yml`
   - 推送到主分支后自动触发部署
   - 部署完成后访问 `https://your-username.github.io/games`

### 手动部署

1. **创建 gh-pages 分支**
   ```bash
   git checkout -b gh-pages
   git push origin gh-pages
   ```

2. **在 GitHub 仓库设置中启用 Pages**
   - 进入仓库 Settings → Pages
   - Source 选择 gh-pages 分支
   - Branch 选择 / (root)

## 📁 项目结构

```
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions 部署配置
├── games.json                   # 游戏列表配置文件
├── index.html                   # 主页（游戏选择界面）
├── snake.html                   # 贪吃蛇游戏
├── tetris.html                  # 俄罗斯方块游戏
├── pong.html                    # 乒乓球游戏
├── space_invaders.html          # 太空侵略者游戏
├── pacman.html                  # 吃豆人游戏
├── minesweeper.html             # 扫雷游戏
├── sudoku.html                  # 数独游戏
├── solitaire.html               # 纸牌游戏
├── flappy_bird.html             # Flappy Bird游戏
├── breakout.html                # 打砖块游戏
├── .gitignore                   # Git忽略文件
└── README.md                    # 说明文档
```

## ⚙️ 技术栈

- **前端**: 纯 HTML5 + CSS3 + JavaScript
- **UI框架**: 无框架依赖
- **字体**: Press Start 2P (Google Fonts)
- **部署**: GitHub Pages

## 🎨 界面特点

- 复古街机风格
- 深色主题 + 霓虹色彩
- 像素字体
- 悬浮动画效果
- 响应式设计

## 🔧 添加新游戏

要添加新游戏到合集：

1. 创建新的 HTML 文件
2. 按照现有游戏的风格和结构实现
3. 在 `games.json` 中添加游戏配置
4. GitHub Actions 会自动检测并更新主页

### 新游戏配置示例

```json
{
  "id": "new_game",
  "name": "新游戏",
  "description": "游戏描述",
  "path": "new_game.html",
  "thumbnail": "data:image/svg+xml;base64,...",
  "rules": "游戏规则说明"
}
```

## 🎯 自动化

项目支持自动化扩展：

- **游戏检测**: GitHub Actions 自动扫描 HTML 文件
- **更新配置**: 自动更新 games.json
- **自动部署**: 推送代码自动部署到 GitHub Pages

## 📱 兼容性

- 所有现代浏览器
- 移动设备（触摸控制）
- GitHub Pages 自动优化

## 🎮 操作指南

### 游戏控制

- **方向键**: 游戏移动/选择
- **空格键**: 暂停/继续
- **Enter**: 开始/重玩游戏
- **鼠标点击**: 点击交互（部分游戏）

### 导航

- 点击主页游戏卡片进入游戏
- 游戏内返回主页按钮

## 🏆 特色功能

1. **统一的设计风格**
2. **流畅的游戏体验**
3. **本地最高分记录**
4. **一键部署到 GitHub Pages**
5. **自动化游戏管理**

## 📄 许可证

MIT License - 自由使用和修改