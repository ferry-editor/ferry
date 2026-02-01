<div align="center">
  <img width="128" height="128" src="https://github.com/user-attachments/assets/535f8411-3e83-4531-9c02-5fdf66561da4" />

  # 轻渡

  **静态博客写作工具**
  <br>
  支持 Hexo / Hugo / Jekyll

  [功能特性](#功能特性) • [界面预览](#界面预览) • [语法支持](#语法支持) • [安装](#安装) • [使用指南](#使用指南)
</div>

---

## 功能特性

**轻渡** 旨在解决静态博客写作中的痛点，提供“开箱即用”的闭环体验：

### 核心写作
* **多引擎支持**：完美兼容 Hexo、Hugo、Jekyll 的文件结构与 Front Matter 规范。
* **全能编辑器**：基于 CodeMirror，支持 **LaTeX 公式**、代码高亮及 Emoji 快捷输入。
* **Git 友好**：直接挂载本地 Git 仓库，文件变动实时同步。

### 资源管道
* **图床零配置**：支持图床拖拽上传，**独家内置 403 防盗链修复方案**及历史图片迁移工具。
* **AI 适配**：自动擦除 Gemini 生成图片的 SynthID 水印。
* **自动优化**：上传前自动执行有损/无损压缩并统一格式，减轻带宽压力。

### 效率与体验
* **模板引擎**：自定义 Front Matter 模板，一键生成标准博文。
* **视觉舒适**：精心调教的深色/浅色模式，专注写作本身。

## 界面预览

<div align="center">
  <img width="100%" alt="主界面预览" src="https://github.com/user-attachments/assets/0c4c90c6-feed-46ec-81ee-f3bcdeb0cb8b" style="border-radius: 8px; border: 1px solid #30363d;" />
<blockquote>主界面编辑预览</blockquote>
  <img width="100%" alt="主界面预览" src="https://github.com/user-attachments/assets/19583ef0-64b6-4ddd-85cf-a848cfb17c4f" style="border-radius: 8px; border: 1px solid #30363d;" />
<blockquote>主界面全预览</blockquote>
</div>

<br>

> 🎨 **个性化定制**
> 轻渡提供多种内置配色方案。此外，支持用户修改配置文件来自定义 UI 颜色，详见 Wiki：[配色自定义数据结构](https://github.com/ferry-editor/ferry/wiki/%E9%85%8D%E8%89%B2%E8%87%AA%E5%AE%9A%E4%B9%89%E7%BB%93%E6%9E%84)

<details>
<summary><b>🎭 点击预览更多主题 (珊瑚紫 / VS Code / 海洋蓝)</b></summary>
<br>

<table width="100%">
  <tr>
    <th width="50%">☀️ 浅色模式 (Light)</th>
    <th width="50%">🌙 深色模式 (Dark)</th>
  </tr>
  <tr>
    <td align="center"><b>珊瑚紫</b></td>
    <td align="center"><b>珊瑚紫</b></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/0363f75d-b14c-47eb-aa2c-9c02b5b80c0b" style="border-radius: 6px; border: 1px solid #d0d7de;"/></td>
    <td><img src="https://github.com/user-attachments/assets/9bea9bde-3ab7-4599-bc7d-4438280f33f4" style="border-radius: 6px; border: 1px solid #30363d;"/></td>
  </tr>
  <tr>
    <td align="center"><b>VS Code 经典</b></td>
    <td align="center"><b>VS Code 经典</b></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/51287c12-e208-46fa-84a2-588b63efa7ae" style="border-radius: 6px; border: 1px solid #d0d7de;"/></td>
    <td><img src="https://github.com/user-attachments/assets/a9990a17-b7bd-4ac5-8014-7b348f75c774" style="border-radius: 6px; border: 1px solid #30363d;"/></td>
  </tr>
  <tr>
    <td align="center"><b>海洋蓝</b></td>
    <td align="center"><b>海洋蓝</b></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/3abb8117-12fd-49a9-8c89-1a334f355044" style="border-radius: 6px; border: 1px solid #d0d7de;"/></td>
    <td><img src="https://github.com/user-attachments/assets/cd896d1d-175d-4277-b7d1-2f7b3ccc4933" style="border-radius: 6px; border: 1px solid #30363d;"/></td>
  </tr>
</table>

</details>

### 语法支持

<table width="100%">
  <tr>
    <th width="50%">LaTeX 数学表达式</th>
    <th width="50%">Emoji 简码</th>
  </tr>
  <tr>
    <td valign="top">
      <img width="100%" alt="LaTeX 预览" src="https://github.com/user-attachments/assets/dec9b7c4-d489-481e-8931-d2b2d79936a1" style="border-radius: 6px; border: 1px solid #d0d7de;" />
      <br><br>
      <details>
        <summary><b>常用 LaTeX 公式示例</b></summary>
        <br>
        
**行内公式**
质能方程 $E = mc^2$

**块级公式**
二次方程求根：
$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

求和公式：
$$\sum_{i=1}^{n} i = \frac{n(n+1)}{2}$$

积分公式：
$$\int_{0}^{\infty} e^{-x^2} dx = \frac{\sqrt{\pi}}{2}$$

矩阵：
$$\begin{pmatrix} a & b \\ c & d \end{pmatrix}$$

分段函数：
$$f(x) = \begin{cases} x^2 & x \geq 0 \\ -x & x < 0 \end{cases}$$
      </details>
    </td>
    <td valign="top">
      <img width="100%" alt="Emoji 预览" src="https://github.com/user-attachments/assets/1fb91b6d-afa2-488b-83ee-891683db08e0" style="border-radius: 6px; border: 1px solid #d0d7de;" />
      <br><br>
      <details>
        <summary><b>支持的 Emoji 列表</b></summary>
        <br>

**😄 笑脸**
:smile: :grinning: :laughing: :blush: :smiley: :relaxed: :smirk: :heart_eyes: :kissing_heart: :wink: :grin: :tongue: :joy: :rofl: :innocent: :sunglasses: :nerd_face: :star_struck:

**😞 情绪**
:disappointed: :worried: :angry: :rage: :cry: :sob: :fearful: :scream: :sleeping: :thinking: :rolling_eyes: :nauseated_face: :exploding_head:

**👍 手势**
:thumbsup: :+1: :thumbsdown: :-1: :ok_hand: :punch: :fist: :v: :wave: :point_up: :point_down: :clap: :muscle: :pray:

**❤️ 心形**
:heart: :yellow_heart: :green_heart: :blue_heart: :purple_heart: :black_heart: :broken_heart: :two_hearts:

**🐶 动物**
:dog: :cat: :mouse: :rabbit: :fox: :bear: :panda: :tiger: :lion: :pig: :frog: :monkey: :unicorn: :butterfly: :dolphin: :shark:

**🍎 其他**
:apple: :banana: :coffee: :beer: :rocket: :tada: :warning: :question:
      </details>
    </td>
  </tr>
</table>

## 安装

支持跨平台安装，目前支持一下平台
1. Mac（Apple Silicon/Intel）
2. Windows
3. Ubuntu（x86/arm64）

从 [Releases](../../releases) 下载最新版本的安装文件进行安装。

> [!TIP]
> **首次打开提示 "无法验证开发者"?**
> 
> 请前往「系统设置 > 隐私与安全性」，在安全性部分点击“仍要打开”。
> 
> 高版本则需要执行命令 `sudo xattr -r -d com.apple.quarantine /Applications/轻渡.app`


## 使用指南

### 1. 启动工作区
点击左上角 **「文件」** 菜单，你可以灵活选择工作模式：
* **打开目录**：直接挂载本地的 Hexo / Hugo / Jekyll 博客目录。
* **打开 Git 仓库**：克隆并接管远程仓库，实现云端同步。

<p align="center">
<img width="400" alt="工作区选择" src="https://github.com/user-attachments/assets/efba543d-b3cb-4524-8a54-acfe20712057" style="border-radius: 6px; border: 1px solid #d0d7de;" />
</p>


### 2. 标准化写作
**轻渡** 内置了智能的 **Front Matter 脚手架**。
在新建文章或页面时，编辑器会通过可视化引导，协助你快速生成符合规范的头部元数据（如标题、日期、标签等），无需手动编写繁琐的 YAML 格式。

<p align="center">
<img width="400" alt="Front Matter 引导" src="https://github.com/user-attachments/assets/1a5dd6f7-08ea-4061-bb04-6117dc820860" style="border-radius: 6px; border: 1px solid #d0d7de;" />
</p>


### 3. 智能图像流水线
体验极致的“拖拽即发布”流程。你只需将图片拖入或粘贴至编辑器，**轻渡** 将自动在后台并发处理以下任务：
* **⚡️ 自动压缩**：平衡画质与体积，提升加载速度。
* **✨ AI 清洗**：自动识别并擦除 Google Gemini 生成图片的 SynthID 水印。
* **☁️ 极速上传**：直接上传至图床并回填 Markdown 链接。

用户原本繁琐的“修图-压缩-上传-复制链接”四步操作，现在缩减为一个动作。

### 4. 实时保存与同步
* **自动保存**：编辑器监听内容变更并自动写入本地文件。顶部状态栏会实时显示保存进度，请在显示“已保存”状态后再关闭文件。
* **一键同步**：若挂载了远程 Git 仓库，编辑器右上角将激活 **「保存到远程仓库」** 按钮，点击即可通过可视化引导完成 `Commit` 与 `Push`，轻松发布文章。

### 5. 进阶工具箱
点击顶部 **「工具」** 菜单，你可以快捷解锁更多效率功能：
* **🧩 动态模板引擎**：支持自定义 Front Matter 字段。无论是博客文章还是复杂的页面配置，只需定义一次，即可将繁琐的 YAML 转化为可视化表单。
* **⚙️ 上传策略配置**：集中管理图床参数。在此处开启“自动压缩”或“去水印”开关，定制专属的图像处理流，“拖拽即发布”从未如此简单。
* **🔄 图床一键迁移**：不仅是上传，更是管理。支持将历史文章中的图片批量迁移至国内 CDN 加速源，解决旧图床失效或加载缓慢的问题。
* **🌐 网络连接增强**：考虑到部分Git仓库连接不稳定的场景，特支持内置网络代理设置，消除同步失败的焦虑，保障沉浸式写作的最后一道防线。
