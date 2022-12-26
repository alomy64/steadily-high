[TOC]

# 单键

### Ctrl + 打字区

1. `Ctrl` + `q`：弹出 主侧栏 选项
2. `Ctrl` + `w`：关闭当前Tab
3. `Ctrl` + `p` / `e`：转到文件
4. `Ctrl` + `r`：弹出 选择项目或文件 选项
5. `Ctrl` + `i`：弹出 相关建议
6. `Ctrl` + `o`：打开文件
7. `Ctrl` + `a`：全选
8. `Ctrl` + `s`：保存
9. `Ctrl` + `d`：搜索并选中光标所在的单词
10. `Ctrl` + `f`：在当前文件查找
11. `Ctrl` + `g`：跳转到第几行
12. `Ctrl` + `h`：查找并替换
13. `Ctrl` + `j` / `：打开 / 关闭 终端
14. `Ctrl` + `k`   `Ctrl` + `o`：打开文件夹
15. `Ctrl` + `k`   `Ctrl` + `t`：选择颜色主题
16. `Ctrl` + `k`  `w`：关闭所有打开的Tab
17. `Ctrl` + `l`：选中当前行
18. `Ctrl` + `z`：撤回
19. `Ctrl` + `x`：剪切
20. `Ctrl` + `c`：复制
21. `Ctrl` + `v`：粘贴
22. `Ctrl` + `b`：显示 / 隐藏 主侧栏
23. `Ctrl` + `n`：新建文本文件
24. `Ctrl` + `[` / `]`：将选中行向 左 / 右 移动
25. `Ctrl` + `/`：行注释 / 取消行注释
26. `Ctrl` + `\`：基于当前页面向右拆分编辑器

### Ctrl + 数字

1. `Ctrl` + `2`：向右拆分编辑器
2. `Ctrl` + `0`：打开 资源管理器

### Alt

1. `Alt` + `b`：用浏览器打开（需安装插件 `open in browser`）
2. `Alt` + `↑` / `↓`：移动整行（上 / 下）
3. `Alt` + `F4`：关闭窗口

### Shift

1. 长按 `Shift` + `↑` / `↓` / `←`/ `→`：可移动光标选中字符
2. `Shift` + `Home` / `End`：选中当前行光标之 前 / 后 的所有内容（不含首尾空格）
3. 鼠标点击选中起始位置，再按 `Shift` + 鼠标点击选中结束位置：可自定义选中内容

### F 区

1. `F2`：重命名（文件 / 单词）

### 功能区

1. `Home`：跳转到行头
2. `End`：跳转到行尾
3. `PgUp`：跳转到页头
4. `PgDn`：跳转到页尾
5. `Ctrl` +  `←` / `→`：以单词为间隔移动光标
6. `Ctrl` + `PgUp`：倒序（自右至左）切换打开的文件
7. `Ctrl` + `PgDn`：顺序（自左至右）切换打开的文件
8. `Ctrl` + `Backspace`：删除光标之前的 单词 / 字串
9. `Ctrl` + `Del`：删除光标之后的 单词 / 字串

### 鼠标

1. 选中文本后，`Ctrl` + 鼠标左键拖动：复制
2. 选中文本后，按住鼠标左键拖动：剪切



# 组合键

### Ctrl + Shift

1. `Ctrl` + `Shift` + `e`：打开 资源管理器
2. `Ctrl` + `Shift` + `p`：查看 命令面板
3. `Ctrl` + `Shift` + `s`：另存为...
4. `Ctrl` + `Shift` + `d`：打开 运行和调试
5. `Ctrl` + `Shift` + `f`：打开 全局搜索
6. `Ctrl` + `Shift` + `g`：打开 源代码管理
7. `Ctrl` + `Shift` + `z`：恢复撤销的内容
8. `Ctrl` + `Shift` + `x`：打开 扩展
9. `Ctrl` + `Shift` + `n`：新建窗口
10. `Ctrl` + `Shift` + `/`：块注释 / 取消块注释
11. `Ctrl` + `Shift` + `：新建终端
12. `Ctrl` + `Shift` + `c`：唤醒 Command Prompt
13. `Ctrl` + `Shift` + `←` / `→`：以 单词 / 字串 为间隔，光标依次选中（可与 `Ctrl` + `Alt` + `↑` / `↓` 结合使用）

### Ctrl + Alt

1. `Ctrl` + `Alt` + `↑` / `↓`：使光标统一在多行同一位置进行操作
2. `Ctrl` + `Alt` + `Enter`：将查找（`Ctrl `+ `f`）到的内容全部替换为指定内容

### Shift + Alt

1. `Shift` + `Alt` + `f`：格式化文档
2. `Shift` + `Alt` + `↑` / `↓`：复制光标所在行

### Ctrl + Tab

1. `Ctrl` + `Tab`：切换至最近打开的文件（可在弹出选择文件的列表后，再按 `Tab` / `↑` / `↓` 来选择文件进行切换）



# 其他

1. 键入 `/**` 后， 会出现 JSDoc 的相关提示，然后按 `Enter` 即可：可生成带有 params（参数）、returns（返回值）等更加详细的注释信息

   ```javascript
   /**
    * 返回 num1 和 num2 的和
    * @param {number} num1 
    * @param {number} num2
    * @returns {number} num1 和 num2 的和
    */
   ```