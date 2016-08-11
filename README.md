<img src="https://s3-us-west-1.amazonaws.com/udacity-content/degrees/catalog-images/nd003.png" alt="iOS Developer Nanodegree logo" height="70" >

# iOS应用开发入门 纳米学位
## 滴滴实习生项目：开发你自己的天气应用
### 前言
来到这里说明你已经顺利完成了 iOS应用开发入门 纳米学位的前8个项目。在这个过程中，你通过学到的知识帮助我们添加了水雷，提升了 **海盗舰队** 的可玩性；编写更加智能的判断逻辑，帮助机器人顺利走出 **机器人迷宫** ；基于你对 Swift 的熟练掌握，帮助机器人一次又一次地化解 **外星人** 的难题；并在之后第一次展现你从0到1的应用开发技能，将课程所有的知识整合在一起，创造出了简单但很有趣的 **古怪之歌** 游戏。走到这里，你应该为自己感到骄傲，你踏上了这条缤纷多彩的编程之路，你希望开发出更加好玩好用的应用，让世界变得更加有趣和美好！

我们为你喝彩，为你所取得的成绩倍感骄傲！我们深知你所取得的这些成绩来之不易，也相信你并不会停止于此，而是会继续向前，克服一个又一个难题，使自己变得更为出色。而在这个过程中，我们——[优达学城](https://cn.udacity.com/course/ios-developer-nanodegree--nd003/)——依然是你最好的伙伴，帮助，引导，鼓励，见证你的成功，是我们最大的成功！

我们坚信，项目是知识学习和证明自己最好的方式，也是我们构建纳米学位的核心基础。在此，作为 **iOS应用开发入门** 的毕业生，我们再次向你发出邀请，开启新的征程，完成天气预报应用，向滴滴证明你的能力！

## 项目概述
你可以根据自己的实际情况选择不同难度的项目版本开发。对于绝大部分学生，我们建议你从 **基础版** 开始制作。若你对后面两个版本同样有兴趣，建议你在 **基础版** 的基础上不断迭代更新。

### 基础版：

* 通过自建 UI Button 列出中国主要热门城市，用于选定某个城市查看当天天气；
* 根据选择的城市，拉取天气数据。数据可从 free weather api 获取；
* 基于天气数据显示，至少包括：当天天气状况（晴、多云……）和温度；
* 提供UI Button 手动刷新按钮

### 中级版：

* 通过 **Table View** 列出中国主要热门城市，用于选定某个城市查看天气；
* 根据选择的城市，拉取天气数据。数据可从 free weather api 获取；
* 基于天气数据显示，至少包括：当天及 **未来3天** 的天气状况（晴、多云……）和温度；
* 提供UI Button 手动刷新按钮

### 高级版：

* 通过 **Table View** 列出中国主要热门城市，用于选定某个城市查看天气；**同时提供搜索框（汉字或拼音）输入城市信息**；
* 根据选择的城市，拉取天气数据。数据可从 free weather api 获取；
* 图形显示天气数据显示，至少包括：当天及 **未来3天** 的天气状况（晴、多云……）和温度；
* **下拉拖动手势自动刷新**

### 可选：
* 自动获取地理位置
* 背景随天气而变化

# 开始

## 准备：在这个过程中你可能会遇到不少需要自己解决的问题, 这也意味着你正在成长

### [搜索](http://so.chongbuluo.com)

**例**：我想要知道哪些控件可以用来显示天气数据的文本内容

* iOS 可显示文本的控件 [结果](https://letsgg.tk/search?newwindow=1&hl=zh-CN&q=iOS+显示文本的空间&oq=iOS+显示文本的空间&gs_l=serp.3...369740.373601.0.373850.13.12.0.0.0.0.280.702.0j3j1.4.0....0...1c.1j4.64.serp..9.0.0.6Uccz-blOxQ)

* iOS how to display text [结果](https://letsgg.tk/search?newwindow=1&hl=zh-CN&q=ios+how+to+display+text&oq=ios+how+to+display+text&gs_l=serp.3.0.0i30j0i8i30l7.62087.63205.0.74130.7.7.0.0.0.0.218.497.0j2j1.3.0....0...1c.1.64.serp..5.2.347...0i7i30j0i8i7i30.xQdIzqGJoko)

#### 建议：
* 使用良好的搜索引擎
* 使用英文关键字搜索

### [文档](https://developer.apple.com/library/mac/documentation/Swift/Conceptual/Swift_Programming_Language/TheBasics.html#//apple_ref/doc/uid/TP40014097-CH5-ID309)

* Xcode内置文档搜索: Shift + Command + 0 
* **查阅**： 在左边的 **Task** 里寻找与你目标吻合的内容

### [GitHub](https://discussions.youdaxue.com/t/github/6596)：放心地迭代代码

### [Debug](https://cn.udacity.com/course/xcode-debugging--ud774/)： 快速定位bug

### [UIKit](https://cn.udacity.com/course/uikit-fundamentals--ud788/)： 深入界面与数据

## 界面：

### 控件：
* **要求**：显示天气数据，热门城市按钮
* **建议**：使用英文文本

### 约束：
* **要求**：垂直或平放时，控件显示正常
* **参考**：Silly Song 的课程(我现在进不去)
* **测试**：command ＋ －>

### 可选：
* 设置背景图片
* 按钮添加边框

## API：

### 申请：
* [openweathermap](https://home.openweathermap.org/users/sign_up)
* 正常登录后点击 [API keys](https://home.openweathermap.org/api_keys)

### 解析：
* **要求**：从API中获取JSON，JSON转化为字典
* **提示**：NSURL、NSURLSession、NSJSONSerialization waixingren2

## 交互：
* **要求**：正确使用 IBOutlet 和 IBAction 与解析的数据进行关联
* **建议**：Silly Song 的课程