# 设计参考（Dribbble + Apple）

> 版本 v0.1 · 2026-10-30 · 配套文档：[PRD.md](./PRD.md)
>
> **方法说明（请先读）**
> - Dribbble 的搜索页对普通抓取返回 403 / 人机验证，所以我用无头 Chrome 打开了公开的搜索页和单个 shot 页面（没有登录，没有绕过任何付费或权限）。
> - 搜索词：`music box`、`skeuomorphic`、`foldable`、`music player animation`、`alarm clock app`、`tactile ui`、`vintage music`、`lid opening`、`skeuomorphism ios`、`wooden music box 3d`、`mechanical animation interaction`、`music box ios app`。`foldable phone ui` 触发了人机验证，没有结果。
> - 下面每一条的 URL 都是我在搜索结果里看到、并且逐个打开过的 shot 页，**标题和作者来自页面标题**。"我看到了什么"来自我实际看到的预览图。
> - **GIF / 视频类 shot 我只看到了静帧**（下面标了"仅静帧"）。动效节奏请你人工打开看一眼，不要只信我的文字描述。
> - `lid opening` 的搜索结果基本都是包装盒样机，对"开盖"没有直接帮助，所以开盖动效没有从 Dribbble 取材，而是来自实物（见 #1）和 PRD 里的物理推导。
> - 没有采集点赞和浏览数，不代表质量高低。借鉴的是"某个具体的点"，不是整个风格。
> - 所有 shot 版权归原作者。这里只借鉴思路，**不要复制素材**。

---

## A. 最值得看的 5 条（先看这 5 条）

> 编号说明：A 区的 # 是推荐顺序；B 区的 # 是完整清单序号；C 区、PRD 里引用的 `#n` 都指 **B 区序号**。

| # | 标题 / 作者 | 链接 | 为什么 |
|---|---|---|---|
| 1 | Deep Meditation App — Foldable iPhone UX/UI Concept · Sigma Software Design | https://dribbble.com/shots/27750746-Deep-Meditation-App-Foldable-iPhone-UX-UI-Concept | 折叠屏半折立在桌面的构图，屏幕只有一个巨大的呼吸圈。**我们的主画面也该这样：一个主角、一个动作。** |
| 2 | Wooden Music Box · Vân Lê | https://dribbble.com/shots/27149755-Wooden-Music-Box | 一台真实手摇八音盒的结构：银色梳齿 + 打点滚筒 + 手摇柄 + 指接木盒。是梳齿和滚筒的比例参照。 |
| 3 | Round And Round · Zhivko Terziivanov | https://dribbble.com/shots/4922993-Round-And-Round | 黄铜 + 白色珐琅底座 + 手摇柄做主角，深酒红背景。**材质搭配和"摇柄就是交互"的思路。**（GIF，仅静帧） |
| 4 | Sounds ON — Clicky Skeumorphic Button · Seto Febriant | https://dribbble.com/shots/24044393-Sounds-ON-Clicky-Skeumorphic-Button | 按下的深度 + 点击声 + 光晕同步。**直接对应我们的"视觉、声音、触觉三者同步"原则。**（动画，仅静帧） |
| 5 | Kitchen Timer iOS App icon · Ivo Ivanov | https://dribbble.com/shots/27253672-Kitchen-Timer-iOS-App-icon | 白色旋钮 + 刻度环 + 红色指示点。**睡眠定时 / 闹钟时间的拨盘就照这个手感做。** |

---

## B. 完整清单（22 条）

### B1. 八音盒与实物质感

| # | 标题 / 作者 | 链接 | 我看到了什么 | 借鉴什么 | 不要照搬什么 |
|---|---|---|---|---|---|
| 1 | Wooden Music Box · Vân Lê | https://dribbble.com/shots/27149755-Wooden-Music-Box | 一台手摇木制八音盒的产品图：激光雕花的盒身、指接（finger joint）盒角、银色梳齿用两颗螺丝固定、旁边是带凸点的金属滚筒，右侧一根手摇柄。 | 梳齿与滚筒的位置关系和比例；盒角的指接木纹；雕花面板可以做成我们的"曲名铭牌"；螺丝作为细节。 | 盒盖里印的祝福语排版（这是礼品定制款）。 |
| 2 | spring · Vivian Wu | https://dribbble.com/shots/27338442-spring | 粉绿色 3D 黏土风场景：一个小木盒八音盒配黑胶唱片，周围是花、彩旗和漂浮的音符。 | 引导页 / 空状态的情绪：温柔、玩具感；音符漂浮的粒子。 | 整体马卡龙色调（和我们的"夜晚木盒"相反，只能用在白天主题或引导页插画）。 |
| 3 | Round And Round · Zhivko Terziivanov（仅静帧） | https://dribbble.com/shots/4922993-Round-And-Round | 一个 3D 人物站在八音盒的旋转底座上，底座是白色珐琅配金色铆钉和镂空格栅，两根黄铜立杆，侧面有手摇柄，背景是深酒红色。 | 黄铜 + 白色珐琅的配色；铆钉作为边缘细节；摇柄是主角。 | 人物（我们没有角色）。 |
| 4 | 3D Music BOX · Mana Akbarzadegan | https://dribbble.com/shots/22022293-3D-Music-BOX | 黑白灰的 3D 渲染：一个掀开盖子的盒子，里面是一个圆盘，单一光源从侧上方打来，背景有明显的渐变。 | **开盖后的剪影**；单光源、明暗过渡很大的布光。 | 里面是转盘 / 唱片式的结构，不是梳齿结构，别学内部。 |
| 5 | The Music Box · Womanintechh | https://dribbble.com/shots/27726803-The-Music-Box | 昏暗的老式场景：一个带条纹顶篷的复古旋转木马式音乐盒，旁边有一个旧玩偶，带胶片颗粒的氛围。 | 夜间模式的氛围：低照度、旧木的颗粒、暗角。 | 恐怖气质——我们要的是安睡，不是惊悚。 |
| 6 | Tornamesa — 3D Illustration & Animation · VAGO | https://dribbble.com/shots/27540148-Tornamesa-3D-Illustration-Animation | 俯视角的手工感转盘，旁边伸进来一只手在拨动。 | **手工制作的温度**；俯视构图可以用在"纸带编辑器"的宣传图。 | 唱片机的主题本身。 |

### B2. 折叠屏 / iPhone Duo 相关

| # | 标题 / 作者 | 链接 | 我看到了什么 | 借鉴什么 | 不要照搬什么 |
|---|---|---|---|---|---|
| 7 | Deep Meditation App — Foldable iPhone UX/UI Concept · Sigma Software Design | https://dribbble.com/shots/27750746-Deep-Meditation-App-Foldable-iPhone-UX-UI-Concept | 一台折叠屏手机呈半折立在反光的桌面上，屏幕里是蓝色渐变背景和一个同心圆，圆里写着 "Inhale"，下面一行 "Tap screen to pause"。 | 半折立放的**宣传构图**（桌面反光、单色背景）；一个主角的画面。 | 这是概念渲染，**铰链位置和 Duo 的实际形态不一定一致**，以 Device Hub 为准。 |
| 8 | Designing for iPhone Duo: the four poses · GoodBarber | https://dribbble.com/shots/27794874-Designing-for-iPhone-Duo-the-four-poses | 横置设备的线框图，右侧有一条绿色的竖向控制栏，内容区是灰色占位块。 | 把"竖向控制栏（rail）"放进草图的画法，设计时就留出右侧 84pt。 | 线框本身没有设计内容。 |
| 9 | Blok · AI Day Planner for iPhone Duo · Puji Ari (North) / Dipa Inhouse | https://dribbble.com/shots/27796547-Blok-AI-Day-Planner-for-iPhone-Duo | 横置的 Duo，左右两栏（任务列表 + 日程时间线），右边缘有竖向控制栏，整体偏深色。 | 展开状态的**双栏安排**，以及内容怎么避开竖向栏。 | 数据密度——我们是情绪产品，不要这么满。 |
| 10 | iPhone Duo Fold Motion · HeYuan（仅静帧） | https://dribbble.com/shots/27815985-iPhone-Duo-Fold-Motion | 一台折起的 Duo，屏幕是系统主屏，背景是丝绸质感的渐变壁纸。 | 说明有人在专门做"折叠动效"。**请你人工看一下它的动画节奏**——我只能看到静帧。 | — |
| 11 | Wallet Overview: iPhone Duo UI · Imran Khan | https://dribbble.com/shots/27809748-Wallet-Overview-iPhone-Duo-UI | 双手横握一台展开的 Duo，屏幕里是钱包概览的两栏仪表盘，右边有竖栏。 | **营销图里"手持"的取景方式**（小红书封面可以参考）。 | 信息密度。 |
| 12 | iPhone Duo Adaptive App Templates – iOS 27 (Free Figma file) · Ramesh Vishwakarma | https://dribbble.com/shots/27777567-iPhone-Duo-Adaptive-App-Templates-iOS-27-Free-Figma-file | 一套自适应模板的展示图，里面有竖屏、横屏、折叠几种布局组合。 | 免费 Figma 文件可以当作"画板尺寸与布局"的起点（下载前请看它的授权说明，我没有核实）。 | — |

### B3. 拟物、触感、控件

| # | 标题 / 作者 | 链接 | 我看到了什么 | 借鉴什么 | 不要照搬什么 |
|---|---|---|---|---|---|
| 13 | Sounds ON — Clicky Skeumorphic Button · Seto Febriant（仅静帧） | https://dribbble.com/shots/24044393-Sounds-ON-Clicky-Skeumorphic-Button | 深灰背景上一个橙色的按钮，有明显的厚度和柔和的外发光。 | 按下时的高度变化、发光变化和点击声同步。我们的"发条上满"可以套用。 | 橙色霓虹的配色。 |
| 14 | Kitchen Timer iOS App icon · Ivo Ivanov | https://dribbble.com/shots/27253672-Kitchen-Timer-iOS-App-icon | 一个白色圆形旋钮放在浅灰底座上，外圈有刻度，顶部一个红色指示点，中间是播放符号。 | **拨盘**的刻度密度、红色指示点、旋钮的受光面。 | 白色塑料质感（我们用黄铜 + 木头）。 |
| 15 | Wheel UI · Daniella | https://dribbble.com/shots/26221138-Wheel-UI | 黑色圆角面板，右侧一条弧形刻度尺，左边一列选项，当前选中项有金色的指示线。 | 竖向选择器的"刻度 + 选中指示线"，适合曲目转盘 / 时间选择。 | 全黑配色。 |
| 16 | Piano Experiment · Mik Skuza | https://dribbble.com/shots/24354559-Piano-Experiment | 深藏蓝的拟物小钢琴：上方两组旋钮（调制/颤音），下方一排黑白键，边缘有细微的斜面和高光。 | 暗色背景下的**斜面高光**怎么打；旋钮刻字。 | 钢琴键本身。 |
| 17 | Modular Synth App (Part 2) · Mik Skuza | https://dribbble.com/shots/22113667-Modular-Synth-App-Part-2 | 浅灰背景上叠放着几块合成器模块面板（黄色、黑色），有旋钮、开关和连接线。 | 面板上的**小字标签、螺丝、开关**这类硬件细节如何让 UI 显得"是真的"。 | 复杂度。 |
| 18 | AKAI Professional MPC 3000 · Rudy Pratama Agnel | https://dribbble.com/shots/27547689-AKAI-Professional-MPC-3000 | 一台老牌采样器的高精度还原：LCD 屏、一组方形打击垫、按钮上的印刷字。 | **材质细节的密度上限**——做到这种程度才叫"像真的"，我们只在主角（梳齿、发条钥匙、铭牌）上做到这个程度。 | 整台设备的信息量。 |
| 19 | Music Player — Animation · Webshocker（仅静帧） | https://dribbble.com/shots/3100440-Music-Player-Animation | 深色边框的横向播放条：左边是一张带唱臂的黑胶，右边是一排圆形控制键和曲名。 | 在**窄条里排播放控制**的方式；唱臂移动可以类比我们的"梳齿被拨动"。 | 黑胶主题。 |
| 20 | Cassette Made in Figma · Niyas V | https://dribbble.com/shots/26124138-Cassette-Made-in-Figma | 一盘磁带的精细插画，标签区有曲目列表和字体设计，下面写着 "Nostalgia"。 | **纸质标签的排版**，可以变成每首曲子的"纸带标签"。Apple 在发布稿里提过一个磁带机主题的 Duo App（Deck-Man），我们要避开同质化。 | 磁带主题。 |

### B4. 闹钟与时间

| # | 标题 / 作者 | 链接 | 我看到了什么 | 借鉴什么 | 不要照搬什么 |
|---|---|---|---|---|---|
| 21 | Smart Alarm Clock UI · Streaks · Mobile App · Nikita Prokofyev / ScreensLab | https://dribbble.com/shots/27759813-Smart-Alarm-Clock-UI-Streaks-Mobile-App | 暖米色背景，两个手机屏：一个是大号 "06:30" 的响铃页，另一个是闹钟列表，每条有星期圆点和开关。 | 闹钟列表的层级（大号时间 > 重复日 > 开关）；暖色基调与我们契合。 | "连续打卡"的游戏化——会破坏睡前的放松。 |
| 22 | Glass alarm clock · Nata Nova | https://dribbble.com/shots/26129083-Glass-alarm-clock | 蓝色渐变上的磨砂玻璃卡片，大号七段数字 "06:00"，下面是 Snooze 和 Stop 两个按钮。 | **响铃界面里大号数字 + 两个按钮**的信息量就够了，别加别的。 | 蓝色玻璃配色；iOS 27 的 Liquid Glass 我们只用在系统控件上。 |

---

## C. 从这些参考里提炼出的 8 条设计结论

这些结论已经写进 PRD 的第 6 章，这里列出来方便对照：

1. **一个主角、一个动作。** 半折立放时，屏幕只讲一件事：盒子打开了，在唱歌（#7）。
2. **材质搭配：深色核桃木 + 黄铜 + 米色纸。** 黄铜只给"能动的东西"（钥匙、梳齿固定件、铭牌边、铰链），木头给"盒子"，纸给"纸带和标签"（#1、#3、#20）。
3. **细节密度只给主角。** 梳齿、钥匙、铭牌做到 MPC 3000 那种精细度，其余地方留白（#18）。
4. **视觉、声音、触觉三者同步。** 任何一次"按下"，三者都在同一帧里发生（#13）。
5. **拨盘用刻度 + 红色指示。** 睡眠定时、闹钟时间、发条圈数都用同一套拨盘语言（#14、#15）。
6. **夜晚是默认场景。** 低照度、暖光、颗粒、暗角，但是不要惊悚（#4、#5）。
7. **手持 / 立放的营销取景。** 一张图讲清"半折、立在床头"（#7、#11）。
8. **别做成 Deck-Man。** Apple 已经在新闻稿里点名了"开合 = 播放控制"的磁带机思路，我们要做**连续**的铰链响应（盖子角度 → 音色、速度），而不只是开 / 合二值。

---

## D. Apple 官方设计与工艺参考

以下链接都是我这次打开过的页面。

### iPhone Duo 设计与开发

- **Design for iPhone Duo（Tech Talk）** https://developer.apple.com/videos/play/tech-talks/111466/
  - 取到的要点：只针对两个尺寸类别设计（外屏 compact 宽度、内屏 regular 宽度），不要为每个姿态做一套布局；控制项移到侧边（竖向栏）；半折时交互元素避开折痕；**不要把功能绑定在某个姿态上**；桌面立放姿态可以做特殊布局，但必须保留同样的控件和层级。
- **Strike a pose with adaptive layouts on iPhone Duo** https://developer.apple.com/videos/play/tech-talks/111463/
  - 取到的要点："displacement（位移）"模式：元素移到更适合其用途的区域；**桌面立放时，上半区适合远距离可见的内容，下半区适合可交互的控件**；连续滚动的内容不位移；避免元素移动过远。
- **Leverage multiple displays and scenes on iPhone Duo** https://developer.apple.com/videos/play/tech-talks/111464/
  - 取到的要点：`onHingeChange`（SwiftUI）/ `UIHingeInteraction`（UIKit）提供三种状态 + 连续角度；**铰链数据用于交互与效果，布局用 arrangement 和 region API**；演示里用铰链角度做吉他的 pitch bend。
- **Prepare — iPhone Duo** https://developer.apple.com/iphone-duo/prepare/
  - 取到的要点：不要用 `UIScreen.main`、不要用设备方向做布局判断；上架时提交 Duo 截图会显示适配徽章；可以在"Helpful Details"里写明适配所有姿态。
- **Developers bring incredible new app experiences to iPhone Duo（Newsroom，2026-10-22）** https://www.apple.com/newsroom/2026/10/developers-bring-incredible-new-app-experiences-to-iphone-duo/
  - Apple 点名的"把折叠变成玩法"的独立 App：**Deck-Man**（打开选专辑、插磁带，合上开始听）。点名的"半折立放"案例：Flighty 的专用飞行追踪模式、Tiimo 的视觉计时器、NYT Cooking、MLB。**这就是编辑想看的东西：折叠是体验的一部分，不是适配。**
- **Human Interface Guidelines — Playing haptics** https://apple-docs.everest.mt/docs/design/human-interface-guidelines/playing-haptics/ （这是 Apple 文档的镜像站，不是 developer.apple.com 本站）
  - 取到的要点：触觉必须强化清晰的因果；短、一致、可关闭；与视觉和声音协调。
- **Expo：Supporting iPhone Duo** https://expo.dev/blog/supporting-iphone-duo
  - 取到的要点：竖向栏占用 84pt 的左或右 inset；用系统导航而不是 JS 自绘；`expo-hinge`；Split View 左窗口宽 469pt。

### Apple Design Awards 2026（工艺参考）

来源：https://www.apple.com/newsroom/2026/06/apple-reveals-winners-of-the-2026-apple-design-awards/

| 获奖作品 | 类别 | Apple 的评语里值得学的点 |
|---|---|---|
| grug | Delight and Fun | **一个很简单的想法，做到有分寸的愉悦。** 我们的一句话也要这么简单："打开它，它就唱。" |
| Moonlitt: Moon Phase Tracker | Interaction | **简单的引导、对系统控件（Liquid Glass）的优秀整合。** 引导页不要超过 3 步。 |
| Tide Guide: Charts & Tables | Visuals and Graphics | **全屏的定制动画 + 与天空匹配的配色。** 我们的配色应该跟着"一天中的时刻"（白天 / 黄昏 / 夜晚）走。 |
| Guitar Wiz | Inclusivity | **Dynamic Type、增强对比度、"不单靠颜色区分"。** 直接对应我们的无障碍章节。 |
| Pine Hearts | Inclusivity | **调整动效和感官反馈的无障碍设置。** 对应"减少动态效果"和触觉开关。 |
| Sago Mini Jinja's Garden | Interaction | **不需要读说明就能玩。** 对应我们"开盖 → 摇钥匙 → 听"的零说明引导。 |

> 说明：这些评语是 Apple 对**获奖作品**的描述，不是对"什么会被推荐"的承诺。"获 ADA"和"被 App Store 编辑推荐"是两个独立的评选。

---

## E. 建议你接下来手动做的 3 件事

1. 在浏览器里把 #7、#13、#19、#10、#3 这几个有动画的 shot 看一遍，**看节奏**，我只看到了静帧。
2. 用 Dribbble 的"Save"建一个 board（你登录后才能存），把 B 区里你喜欢的存进去，之后找设计师或 AI 出图时，直接给这个 board。
3. 去买或借一个真实的 30 音八音盒，拍一圈微距视频：梳齿、滚筒、棘轮的动态细节，会比任何 Dribbble 参考都有用，**也是采样音色的来源**（见 PRD 第 6.7 节）。
