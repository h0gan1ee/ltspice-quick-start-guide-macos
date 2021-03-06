# LTspice Quick Start Guide (macOS)

> 本文首次发布 URL：[https://github.com/h0gan1ee/ltspice-quick-start-guide-macos/blob/main/README.md](https://github.com/h0gan1ee/ltspice-quick-start-guide-macos/blob/main/README.md)

## 下载与安装

官网下载地址：[https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html)

<img src="/assets/1.png" width="600">

下载完毕后得到一个 `.pkg` 格式的安装包，打开按指引安装即可。

## 文件操作

文件默认存储位置：`用户目录/Documents/LTspice/`

## 基本用法

### 概览

右键点击空白处即可调用出工具菜单。（这一点与 Windows 不同）

<img src="/assets/2.png" width="200">

点击 `View -> Grid Dots` 开启网格点视图。

点击 `🏃` 按钮开始仿真分析，点击 `🖐️` 按钮停止仿真模拟，点击 `🔨` 按钮进入配置界面。

推荐先画电线再嵌入元件，元件会自动覆盖电线。

LTspice 的右键功能非常强大，如果要修改某个东西，往往可以右键点击。（在图象界面中右键点击很有用）

### 元件基本操作

#### 添加电线

按 `F3`，绘制过程很直观，便不赘述。按 `esc` 可退出电线添加模式。

#### 添加元件

按 `F2`，输入元件符号名称（默认聚焦在搜索框），按 `return`，移动指针，可按 `⌘ R` 旋转元件，单击以添加。按 `esc` 可退出	元件添加模式。

基本元件符号名称：
|符号名称|描述|
|:---:|:---|
|`voltage` / `vo`|电压源|
|`current` / `cu`|电流源|
|`res` / `r`|电阻|
|`cap` / `c`|电容|
|`diode` / `d`|二极管|
|`ind` / `i`|电感|
|`led` / `l`|发光二极管|

#### 修改

移动鼠标指针到元件处，鼠标指针变为 `👈`，右键点击。

有些元件的某些参数需要点击 `Advanced` 才会显示。

除元件外，其他元素的修改同理，便不赘述。

#### 删除

按 `F5`，鼠标指针变为 `✂️`，点击以删除。按 `esc` 可退出	删除工具模式。

也可点击并拖拽鼠标，以删除框选的元素。

### SPICE 分析基本操作

#### 添加指令

按 `S`，输入指令（按 `⌘ return` 换行），按 `OK` 完成输入，移动指针，单击以添加。

在编辑框中右键单击，`Help me edit` 中的工具可以更直观地辅助添加指令。

#### 添加位点

按 `F4`，选择 `GND` 即为接地位点，否则为普通位点，普通位点需要输入名称，按 `OK`，移动指针，单击以添加。按 `esc` 可退出管脚名称添加模式。

#### 开始分析

按 `🏃`，在图中用鼠标指针放置测试位点，即可得到相应的图象。

右键单击图像中的相应元素即可编辑图像。

### 基本配置

在 `Drafting -> Configure Colors` 中可配置配色方案。

这是其中一种方便放在实验报告中的配色方案：

<img src="/assets/3.png" width="300">
<img src="/assets/4.png" width="300">

在 `Operation -> Model Update` 中可更新模型，在更新过程中**请不要操作软件**。

### 常用数值符号

|符号|数量级|
|:---:|:---:|
|`n`|−9|
|`u`|-6|
|`m`|-3|
|`k`|3|
|`MEG`|6|
|`G`|9|

### 常用快捷键

|快捷键|描述|
|:---:|:---|
|`空格键`|缩放到合适的大小|
|`esc`|退出当前模式|
|`F3`|电线添加模式|
|`F2`|元件添加模式|
|`F4`|管脚名称添加模式|
|`F7`|移动工具模式|
|`F8`|拖拽工具模式（原有连接的电线不断开）|
|`F5`|删除工具模式|
|`S`|SPICE 指令添加模式|
|`C`|评论添加模式|
|`B`|总线添加模式|
|`L`|画线模式|
|`W`|画三角形模式|
|`C`|画圆模式|
|`A`|画弧线模式|

在 `系统偏好设置` 中可以将 `F1`、`F2` 这些功能键设置为首选键（即反转 `fn` 作用这些按键的效果）。

<img src="/assets/5.png" width="600">
