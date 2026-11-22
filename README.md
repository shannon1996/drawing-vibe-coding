# Drawing Vibe Coding

用于绘画结构练习的交互工具。当前版本是手臂骨骼与动作观察页，单个 HTML 文件即可离线使用。

## 使用

下载项目后，用浏览器打开 `index.html`，无需安装依赖或运行构建命令。

1. 在「手臂动作」中选择左臂或右臂，分别调整各自姿势。
2. 调整抬臂角度、抬臂方向、肘部屈伸、大臂内外转和前臂翻转；也可以选择「参考① · 斜臂」或「参考② · 折回」。
3. 两只手臂始终显示在同一场景中，通过正面、背面、左侧、右侧切换共同观察方向。

## 当前功能

- 左右臂独立设置，双臂同图观察。
- 自然透视和正交投影。
- 尺骨为蓝色、桡骨为橙色，鹰嘴突以粉色突出标注。
- 肱桡肌以绿色显示，仅在对应手臂伸直时出现。
- 人体小图同步显示两侧手臂姿态。
- 标签优先放在手臂外侧，并避让模型和其他标签。

## 文件

- `index.html`：完整应用，包含所需脚本与模型数据。
- `README.md`：项目说明。

## 模型数据与来源

骨骼及肌肉数据来自 [BodyParts3D 4.0](https://dbarchive.biosciencedbc.jp/en/bodyparts3d/download.html)。

**BodyParts3D, © The Database Center for Life Science**，模型数据采用 [Creative Commons Attribution 4.0 International（CC BY 4.0）](https://creativecommons.org/licenses/by/4.0/)，依照[数据提供方的许可说明](https://dbarchive.biosciencedbc.jp/en/bodyparts3d/lic.html)使用。

当前应用选取 32 块右侧骨骼和 1 块肱桡肌网格，转换坐标与单位、生成平滑法线，并加入左侧镜像、关节运动、肌肉近似变形和绘画观察界面。完整的数据来源和结构参考说明保留在应用的「使用与来源」中。
