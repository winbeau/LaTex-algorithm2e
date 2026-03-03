# algorithm2e Overleaf Workspace

这个仓库是一个只关注“论文算法框”的工作台模板，适合在 Overleaf 直接写算法，不包含章节模板和参考文献模板。

## 目录

- `main.tex`: 编译入口，顺序加载算法示例。
- `tex/algorithm2e.sty`: 固定版本的 `algorithm2e` 包（仓库内置，保证可复现）。
- `tex/algorithm-setup.tex`: 统一算法样式配置（行号、关键字、注释风格等）。
- `algorithms/*.tex`: 算法示例文件（当前 6 个）。

## Overleaf 使用

1. 上传整个仓库到 Overleaf 项目。
2. 将主文件设置为 `main.tex`。
3. 直接编译（pdfLaTeX 即可）。

## 新增算法示例

1. 新建文件：`algorithms/07_your_algo.tex`。
2. 按 `algorithm2e` 语法写 `algorithm` 环境。
3. 在 `main.tex` 末尾增加 `\input{algorithms/07_your_algo}`。

## 常见注意事项

- `algorithm2e` 里每行通常用 `\;` 结束。
- 窄栏（双栏）写法建议“一行一操作”，避免公式或语句过长。
- 全局样式尽量只改 `tex/algorithm-setup.tex`，不要在每个算法里重复定义。

## 官方文档

- CTAN: <https://ctan.org/pkg/algorithm2e>
