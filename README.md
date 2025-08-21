# 调查问卷模板 (Survey Template)

一个基于Netlify Forms的可复用调查问卷模板，专为医院科室宣传微视频项目设计，但可根据不同主题需求进行定制。

## 🌟 特性

- **Netlify Forms集成** - 无需后端代码，自动处理表单提交
- **响应式设计** - 适配桌面和移动设备
- **现代化UI** - 使用Tailwind CSS构建的简洁美观界面
- **本地存储** - 支持本地数据保存和查看
- **可定制性** - 易于根据不同主题需求修改

## 🚀 快速开始

### 1. 克隆仓库
```bash
git clone https://github.com/Wendealai/Videosurvey.git
cd Videosurvey
```

### 2. 部署到Netlify

#### 方法一：通过Netlify UI
1. 访问 [Netlify](https://netlify.com)
2. 点击 "New site from Git"
3. 选择 GitHub 并授权
4. 选择 `Wendealai/Videosurvey` 仓库
5. 点击 "Deploy site"

#### 方法二：拖拽部署
1. 将项目文件夹拖拽到 Netlify 的部署区域
2. 自动部署完成

### 3. 配置表单检测
- Netlify 会自动检测 `netlify` 属性的表单
- 在 Netlify 仪表板中查看表单提交

## 📋 表单结构

### 当前包含的字段
- **科室背景信息** (4个问题)
- **宣传目标与诉求** (5个问题)
- **内容构思与表现形式** (4个问题)
- **项目执行信息** (4个必填字段)
- **补充说明** (1个开放性问题)

### Netlify Forms 配置
```html
<form id="survey-form" netlify>
    <input type="hidden" name="form-name" value="survey-form" />
    <!-- 表单字段 -->
</form>
```

## 🎨 自定义指南

### 1. 修改主题和标题
编辑 `index.html` 中的标题部分：
```html
<h1 class="text-3xl md:text-4xl font-bold main-title mb-2">客户需求调查问卷</h1>
<p class="text-gray-500">医院科室宣传微视频项目</p>
```

### 2. 更换Logo
- 将新的logo文件命名为 `logo.png`
- 放置在项目根目录
- 或修改HTML中的logo路径

### 3. 调整表单字段
- 在 `index.html` 中找到对应的表单部分
- 修改 `name` 属性以匹配新的字段名
- 更新标签文本和占位符

### 4. 自定义样式
主要颜色变量（橙色主题）：
```css
.main-title { color: #FF8C00; }
.accent-color { color: #FF8C00; }
.accent-bg { background-color: #FF8C00; }
```

## 📱 响应式设计

- **桌面端** - 最大宽度1200px，双栏布局
- **平板端** - 自适应单栏布局
- **移动端** - 优化触摸交互，字体大小调整

## 🔧 技术栈

- **HTML5** - 语义化标记
- **CSS3** - Tailwind CSS 框架
- **JavaScript** - 原生JS，无依赖
- **Netlify Forms** - 表单处理
- **LocalStorage** - 本地数据存储

## 📊 数据管理

### Netlify 仪表板
- 自动收集所有表单提交
- 支持导出CSV格式
- 实时通知功能

### 本地存储
- 浏览器本地保存提交记录
- 支持查看历史提交
- 数据导出功能

## 🎯 使用场景

### 当前模板
- 医院科室宣传微视频需求调研
- 医疗品牌建设调查
- 专业服务需求收集

### 可扩展场景
- 产品需求调研
- 客户满意度调查
- 活动报名表单
- 意见反馈收集
- 任何需要表单收集的场景

## 🔄 复用流程

1. **Fork 仓库** - 创建自己的副本
2. **修改内容** - 根据新主题调整
3. **更新配置** - 修改表单字段和样式
4. **重新部署** - 部署到新的Netlify站点

## 📝 最佳实践

### 表单设计
- 保持问题简洁明了
- 使用适当的输入类型
- 必填字段明确标识
- 提供清晰的说明文字

### 用户体验
- 响应式设计确保移动端友好
- 加载速度快，无外部依赖
- 清晰的视觉层次
- 直观的交互反馈

### 数据收集
- 合理的问题数量（建议15-20个）
- 逻辑清晰的问题分组
- 适当的开放性问题
- 必要的联系信息收集

## 🤝 贡献

欢迎提交 Issue 和 Pull Request 来改进这个模板！

## 📄 许可证

MIT License - 可自由使用和修改

## 🔗 相关链接

- [Netlify Forms 文档](https://docs.netlify.com/forms/setup/)
- [Tailwind CSS 文档](https://tailwindcss.com/docs)
- [项目演示](https://your-demo-site.netlify.app)

---

**注意**: 这是一个模板项目，部署后请根据实际需求进行定制化修改。
