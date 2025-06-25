# university-life-quality-guide-search-enhancement
【大学生活质量指北网站搜索增强 】是一款为“大学生活质量指北”网站量身打造的 Tampermonkey 油猴脚本，旨在大幅提升大学信息检索效率。通过内存预加载和优化UI，实现毫秒级搜索响应、多结果智能展示、以及流畅的用户交互体验。告别繁琐查找，快速定位所需信息。

-----

# 📚 大学生活质量指北网站搜索增强

**告别手动查找，即刻拥有闪电般的大学信息检索体验！🚀**

这是一个为 [大学生活质量指北](https://colleges.chat/) 网站精心设计的 Tampermonkey 油猴脚本。旨在彻底解决您在查找特定大学信息时遇到的耗时和不便，尤其是在网站左侧导航栏数据量庞大时。本脚本通过创新的**内存预加载**和**原生 DOM 驱动**的交互，为您带来前所未有的搜索效率与流畅体验。

## ✨ 核心功能亮点

1.  **🔍 全站极速搜索：** 告别传统低效的 DOM 遍历，脚本在页面加载时（仅一次！）便自动将所有大学数据预加载到内存。这意味着您的每一次搜索都是**毫秒级响应**，快到飞起！

2.  **📊 多结果智能呈现：** 当您的搜索关键词匹配到多所大学时，脚本会优雅地弹出一个**美观且可滚动**的模态窗口。所有匹配结果（包含大学名称和所属类别）一目了然，您可以从中精确选择想要跳转的目标。

3.  **⚡️ 流畅的用户反馈：**
    * 搜索启动时，底部会显示一个**非阻塞**的加载提示（Toast），配有精致的加载动画，让您清晰掌握搜索进度。
    * 点击结果中的“前往”按钮时，该 Toast 会智能切换为“即将跳转...”提示，平滑过渡到新页面，避免跳转时的突兀感。

4.  **✅ 智能类别筛选：** 除了模糊匹配大学名称，您还可以根据需要在“问卷数据”、“已归档数据”或新增的“所有类别”中进行精确筛选，让搜索结果更聚焦。

5.  **🛡️ 纯原生稳定：** 彻底移除了对外部第三方库（如 SweetAlert2）的依赖。所有 UI 元素和交互逻辑均采用**纯 JavaScript 和原生 DOM** 构建，确保在各种浏览器和 Tampermonkey 环境下的**最佳兼容性与稳定性**。

## 兼容性

本脚本适用于安装了 Tampermonkey、Greasemonkey 等用户脚本管理扩展的**所有主流浏览器**，包括 Chrome、Firefox、Edge 等。

## 📦 安装步骤

1.  **安装 Tampermonkey 扩展：**
    * **Chrome:** [点击安装](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)
    * **Firefox:** [点击安装](https://addons.mozilla.org/zh-CN/firefox/addon/tampermonkey/)
    * **Edge:** [点击安装](https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmkjmpbldldcalohfklkllfgjnnlse)
---
2.  **配置 Tampermonkey 扩展权限（重要）：**
    * 安装 Tampermonkey 扩展后，进入浏览器的“管理扩展程序”界面。
    ![PixPin_2025-06-26_02-33-48](https://github.com/user-attachments/assets/9e74ff64-6a0f-4929-87b1-c78e13b696f7)
    * 找到“篡改猴”或“Tampermonkey”扩展，点击“详细信息”。
      ![PixPin_2025-06-26_02-35-39](https://github.com/user-attachments/assets/3c5c54e9-3cd7-4371-9f7f-a10c3d78dcee)
    * **确保“允许访问文件网址”处于开启状态。**
    * **确保“有权访问的网站”选择“在所有网站上”或者选择“在特定网站上”（并添加 `colleges.chat`）。**
    ![PixPin_2025-06-26_02-37-05](https://github.com/user-attachments/assets/931349a6-b858-4e17-9168-c14818614589)

---

3.  **获取并安装脚本代码/插件（推荐两种方式）：**

    * **方式一 (推荐：通过 Greasy Fork 网站直接安装插件 - 易于更新):**
        1.  右键点击此链接并选择"在新标签页打开链接"后进入 Greasy Fork 上的脚本页面：
            **[大学生活质量指北网站搜索增强 (Greasy Fork)](https://greasyfork.org/en/scripts/540757-%E5%A4%A7%E5%AD%A6%E7%94%9F%E6%B4%BB%E8%B4%A8%E9%87%8F%E6%8C%87%E5%8C%97%E7%BD%91%E7%AB%99%E6%90%9C%E7%B4%A2%E5%A2%9E%E5%BC%BA-%E6%9C%80%E7%BB%88%E4%BF%AE%E5%A4%8D%E7%89%88)**
        2.  在 Greasy Fork 页面上，找到并点击“**安装此脚本**”（或 `Install this script`）按钮。
      
        ![PixPin_2025-06-26_02-10-45](https://github.com/user-attachments/assets/b46f32b0-3981-4c99-8f17-717b26e9dd8f)
      
        3.  Tampermonkey 会自动捕获安装请求，弹出一个确认安装的界面。点击“**安装**”或“**确认安装**”按钮。
      ![PixPin_2025-06-26_02-16-44](https://github.com/user-attachments/assets/8299735e-b3c0-4ded-ab00-917eee5bc573)

        ![PixPin_2025-06-26_02-13-41](https://github.com/user-attachments/assets/0bd5ba82-adfa-4973-8219-da5135a93228)
      
        4.  安装完成后，点击 Tampermonkey 的浏览器插件图标后会打开仪表盘，
      
        ![PixPin_2025-06-26_02-14-55](https://github.com/user-attachments/assets/52ff69f8-b5f8-400c-9651-3773cb7f0fa0)
      
        5.  找到并点击“控制面板”选项
      
        ![PixPin_2025-06-26_02-16-09](https://github.com/user-attachments/assets/d2f5241c-5921-44e5-a021-bed1597ae255)
           
        6.  点击后进入插件管理界面，确认“大学生活质量指北网站搜索增强”脚本已下载完毕并处于“**已启用**”状态（开关为绿色）。

        ![PixPin_2025-06-26_02-16-44](https://github.com/user-attachments/assets/8cbecbe8-92be-4edf-8cfa-0e8fae197f45)
            
        * **如果安装未能成功，请多尝试几次，或者尝试清除浏览器缓存后再试。**

    * **方式二 (备用：通过 GitHub 源代码安装 - 适合开发者或手动更新):**
        1.  点击此处访问**[脚本源代码文件在 GitHub](https://github.com/Endotch/university-life-quality-guide-search-enhancement/blob/main/university-life-quality-guide-search-enhancement.user.js)** （请确保链接中的用户名和仓库名是您自己的）。
        2.  在打开的 GitHub 页面中，点击文件内容上方的 `Raw` 按钮右边的"Copy raw file"按钮即可直接复制源代码。
           （ 也可以点击raw按钮进入纯文本显示模式并将页面中的所有代码复制或者下载完源文件之后用IDE工具打开文件再复制 ）
        4.  在 Tampermonkey 仪表盘中，点击“**创建新脚本/添加新脚本...**”，然后将默认生成的所有代码**全部删除**，再将复制的代码**粘贴**进去。
        5.  点击“文件” (File) -> “保存” (Save) 按钮。（或者使用"ctrl+s"快捷键保存）

        6.  在 Tampermonkey 控制面板中，确认脚本已启用。

5.  **刷新网站：**
    * 访问 <https://colleges.chat/>。
    * **强制刷新页面**（Windows/Linux: `Ctrl + Shift + R`，macOS: `Cmd + Shift + R`），以确保新脚本加载生效。

## 🚀 使用方法

1.  **访问目标网站：** 打开 [大学生活质量指北](https://colleges.chat/)。

2.  **定位搜索框：** 在页面加载完成后，您会在**右上方**看到一个简洁的搜索模块（包含输入框、类别选择和“搜索”按钮）。

![PixPin_2025-06-26_00-07-57](https://github.com/user-attachments/assets/ac65668d-43b8-47b1-a601-1f49d2814786)

3.  **输入大学名称：** 在输入框中键入您想查找的大学名称（支持模糊匹配，例如输入“浙大”也可能找到“浙江大学”）。

![PixPin_2025-06-26_00-08-21](https://github.com/user-attachments/assets/9feb23cf-51f0-4d96-83ae-6b33d00e87ac)

4.  **选择信息类别：** 在下拉菜单中选择您想搜索的类别：“问卷数据”、“已归档数据”或“所有类别”。

5.  **启动搜索：** 点击“**搜索**”按钮。

6.  **查看搜索结果：**
    * 页面底部会出现一个短暂的“**正在搜索...**”加载提示。
    * 搜索完成后，页面中央会弹出一个“**搜索结果**”模态窗口，列出所有符合条件的大学及其所属类别。

![PixPin_2025-06-26_00-08-58](https://github.com/user-attachments/assets/6ae688da-e523-42fa-862f-8f3576952560)

7.  **跳转到大学页面：**
    * 在结果列表中，点击您希望前往的大学旁的“**前往**”按钮。
    * 模态窗口会关闭，底部会显示“**即将跳转...**”提示，随后页面会自动跳转到该大学的详情页。

![PixPin_2025-06-26_00-09-17](https://github.com/user-attachments/assets/7df9f675-1d27-487a-8235-fcc32db43d66)

8.  **关闭结果窗口：** 您可以点击结果窗口右上角的“**×**”按钮，或点击窗口外部的半透明区域来关闭它。

## 💡 常见问题与故障排除

* **搜索框没有显示 / 脚本没有运行：**
    * 请确保您已正确安装 Tampermonkey 扩展，并且其图标为彩色（表示已启用）。
    * 在 Tampermonkey 仪表盘中，确认“大学生活质量指北网站搜索增强”脚本旁边的开关为**绿色**（已启用）。
    * 尝试强制刷新网站页面 (`Ctrl + Shift + R` / `Cmd + Shift + R`)。
    * 打开浏览器控制台 (F12 -> Console)，检查是否有任何“`油猴脚本:`”开头的错误信息。

* **点击“搜索”或“前往”按钮后没有反应：**
    * 请再次检查浏览器控制台 (F12 -> Console)，查看是否有任何新的错误日志，特别是点击后没有日志输出的情况。这通常意味着事件监听器未被正确触发或脚本执行中断。
    * 尝试清除浏览器缓存，然后强制刷新页面。

## 💖 贡献与反馈

如果您在使用过程中遇到任何问题（Bug）、有功能上的建议，或者希望为脚本的改进贡献代码，都非常欢迎！
* 请通过 Greasy Fork 的评价/评论功能或 GitHub 仓库（如果有）提供反馈。
* 您的每一次反馈都是脚本变得更好的动力！

## 📜 许可证

本脚本依据 **MIT 许可证** 发布。这意味着您可以自由地使用、复制、修改、合并、发布、分发、再许可和/或销售本软件的副本。唯一的条件是，在使用时需包含原始的版权和许可证声明。

-----



