# monso3.github.io
某个人的个人网页

## 项目架构

### 文件结构
```
.
├── README.md
├── index.html
└── pictures/
    ├── Gariton1.png
    ├── Gariton2.png
    ├── Gariton3.png
    ├── JHQ.jpg
    ├── Mask1.png
    └── Mask2.png
```

### 技术栈
- **前端技术**: 纯 HTML5 + CSS3 + JavaScript (ES6)
- **字体**: Google Fonts (Playfair Display, Special Elite, IM Fell English)
- **样式特性**:
  - CSS 自定义属性 (变量)
  - Flexbox 与 CSS Grid 布局
  - CSS 动画 (@keyframes)
  - 响应式设计 (viewport, media queries)
- **交互特性**:
  - 原生 JavaScript DOM 操作
  - 拖拽交互 (窗帘和票证)
  - 点击事件与状态切换
- **图形**:
  - SVG 背景纹理
  - 内联 SVG 效果
  - CSS 渐变与阴影

### 架构特点
- 单页应用 (SPA) 风格，所有内容在一个 HTML 文件中
- 无外部框架依赖 (如 React, Vue, Angular)
- 无构建工具 (如 Webpack, Vite) 迹象
- 静态资源 (图片) 本地托管

### 性能优化
- **硬件加速**: 为关键动画元素添加 `will-change`、`backface-visibility` 和 `translateZ(0)` 属性
- **动画优化**: 使用 `translate3d()` 替代 `translate()` 以启用 GPU 加速
- **关键帧简化**: 减少 `@keyframes` 中的关键帧数量，优化动画性能
- **性能监控**: 内置 FPS 监控和动画性能检查脚本
- **开发体验**: 开发环境下自动启动性能监控，提供实时性能反馈

### 文件信息
- `index.html`: 2880 行，约 101KB (包含所有样式、脚本及性能优化代码)
