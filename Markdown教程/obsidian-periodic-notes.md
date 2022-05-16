---
created: 2022-05-06T11:57:38 (UTC +08:00)
tags: []
source: https://github.com/liamcain/obsidian-periodic-notes
author: liamcain
---

# liamcain/obsidian-periodic-notes：在 Obsidian 中创建/管理您的每日、每周和每月笔记

> ## Excerpt
> Create/manage your daily, weekly, and monthly notes in Obsidian - liamcain/obsidian-periodic-notes: Create/manage your daily, weekly, and monthly notes in Obsidian

---
## Periodic Notes

Create and manage all of your time-based notes within Obsidian.

___

**Note:** This README has been preemptively updated in anticipation for v1.0. Not all features described here are available in the current stable release 0.0.17.

___

This plugin allows you to:

-   Create notes for any periodic of time (daily, weekly, monthly, etc)
-   Jump to any time-based notes with natural language using the Date Switcher (requires [NL Dates plugin](https://github.com/argenos/nldates-obsidian))
-   Easily orient yourself in a sea of `202204101611 Zettelkasten Prefixed notes` using the Timeline complication

## Features

### ![calendar](https://github.githubassets.com/images/icons/emoji/unicode/1f4c6.png) Calendar sets

A **calendar set** describes a collection of periodic notes. Now you no longer need to have a single daily note; instead, you can have one for each pillar of your life. Have a clean break between personal and work. Track a project. Track client work. Organize your school work. Calendar sets offer _flexibility_ for you to live more strict.

[开始设置 →](https://github.com/liamcain/obsidian-periodic-notes#setting-up-your-first-calendar-set)

### ![扎普](https://github.githubassets.com/images/icons/emoji/unicode/26a1.png)日期切换器

涉及定期笔记和 Zettelkasten-ish 笔记的工作流程中的两个最大痛点是 **笔记召回** 和 **导航** 。 日期切换器试图解决这两个问题。 使用自然语言快速查找定期笔记和其他与日期相关的笔记。

寻找上周的会议记录？ 只需搜索： `last week ⇥ meeting`.

[用法 →](https://github.com/liamcain/obsidian-periodic-notes#using-the-date-switcher)

### ![手表](https://github.githubassets.com/images/icons/emoji/unicode/231a.png)时间线并发症

日期切换器将让您快速从一个音符切换到另一个音符，您可能会开始迷路。 但不要担心！ 现在，您的定期笔记右上角有一个时间线“复杂功能”，可以用自然语言准确显示您的位置。

[用法 →](https://github.com/liamcain/obsidian-periodic-notes#using-the-timeline-complication)

## 用法

### 设置您的第一个日历集

在定期笔记设置中，您将从“默认”日历集开始。 单击它以打开日历集详细信息视图。

从这里，您可以选择 **笔记类型** 要启用 要开始使用，您可能需要启用： **Daily** 、 **Weekly** 、 **Monthly** 和 **Yearly** 。

每种笔记类型都有相同的配置选项：

-   **格式：** 用作新定期票据文件名的日期格式。 该值不仅用于生成文件名，而且该插件在索引您的保管库以查找定期注释时也使用此格式。
-   **基本文件夹：** 将保存此日历集的所有定期笔记的文件夹。 对于个人日常笔记，您可以选择 `Journal/`文件夹，例如。
-   **模板位置：** 笔记模板的路径。 查看 [模板标签](https://github.com/liamcain/obsidian-periodic-notes#template-tags) 部分了解更多信息。

### 了解日历集

[![图片](https://user-images.githubusercontent.com/693981/163569851-0280a2eb-fe9b-49db-a48a-93b4cfbd93ec.png)](https://user-images.githubusercontent.com/693981/163569851-0280a2eb-fe9b-49db-a48a-93b4cfbd93ec.png)

每个日历集都有一个完全独立的配置。 最常见的用例是创建两个集合：“个人”和“工作”。 这样，您可以将日常工作日志保存在单独的文件夹中，而不会被个人信息污染。

当您有多个日历集时，一个集被设置为 **活动日历集** 。 所有涉及创建或查看特定定期笔记的命令将只查看当前活动日历集中的笔记。 您可以在设置中切换活动集或使用命令“切换活动日历集...”。

### 使用日期切换器

使用命令“定期笔记：显示日期切换器...”访问日期切换器。 打开它后，日期切换器将显示一组快速日期条目。

[![图片](https://user-images.githubusercontent.com/693981/163502230-b26950b2-be74-4e77-a823-cc4d599b8e33.png)](https://user-images.githubusercontent.com/693981/163502230-b26950b2-be74-4e77-a823-cc4d599b8e33.png)

在每个条目上，它会显示活动日历集是否具有相应的注释、该注释的路径以及该时间段内相关注释的数量。 选择一个条目将打开现有笔记，如果不存在则创建一个新笔记。 您可以通过单击 或 选择注释 Enter. 按住 ctrl选择条目时将在新窗格中打开该注释。

##### 相关说明

紧迫 Tab将为突出显示的条目打开相关注释视图。 这将显示对应于该时间段的所有非精确匹配。 在“今天”条目上，它将显示文件名中出现今天日期的所有注释。 对于“本月”条目，它将显示所有以 `YYYY-MM`.

##### 扩展搜索

在相关注释视图中，您可以按 `*`以扩大搜索。 扩展搜索意味着列表将包括该时间段内的所有 _条目_ 。 因此，“本月”条目将包括该月的所有每周和每日笔记。

当寻找一个特定的 Zettlekasten 笔记时，这变得特别强大，你记得它是从上周开始的，但可能不是特定的一天。

### 使用时间线复杂功能

并发症将显示打开笔记的相对日期。

| 笔记 | 外貌 |
| --- | --- |
| `2022-04-14.md` | [![图片](https://user-images.githubusercontent.com/693981/163503952-a8619a42-a91a-43ea-af49-eb77744c5048.png)](https://user-images.githubusercontent.com/693981/163503952-a8619a42-a91a-43ea-af49-eb77744c5048.png) |
| `202204141213 Meeting Notes.md` | [![图片](https://user-images.githubusercontent.com/693981/163503975-7a8f9798-5644-4d3d-8eeb-49c2e07d0884.png)](https://user-images.githubusercontent.com/693981/163503975-7a8f9798-5644-4d3d-8eeb-49c2e07d0884.png) |

#### 每周日历

单击时间线复杂功能将切换每周内联日历。

[![时间线](https://user-images.githubusercontent.com/693981/163504193-064dbb30-0890-4708-86c8-49b50e86da35.gif)](https://user-images.githubusercontent.com/693981/163504193-064dbb30-0890-4708-86c8-49b50e86da35.gif)

## 配置

### 分类日期

Periodic Notes 在指定的文件夹中搜索并索引所有类型的时间相关文件。

-   匹配的注释 **完全** 设置中指定的日期格式 所以如果格式是 `YYYY-MM-DD`，它会找到并索引 `2022-04-10.md`
-   文件名中带有日期的注释。 这包括以 Zettelkasten 为前缀的注释（例如 `202204101611 Meeting Notes.md`) 还有像 `Budget cuts made in 2021.md`.
-   票据 [根据frontmatter确定为定期票据的](https://github.com/liamcain/obsidian-periodic-notes#parsing-frontmatter)

使用 frontmatter 来识别笔记为您提供了最大的灵活性，可以随意命名笔记，这意味着您不再局限于 Moment.js 可以解析的固定格式。

当打开特定日期的笔记时，算法总是寻找精确匹配，并且它更喜欢前端匹配而不是文件名匹配。

#### 解析文件名

Periodic Notes 将查看嵌套在 **文件夹** 您配置

所以你可以拥有：

```
- daily_notes/
  # all-notes within one folder
  - 2022-04-01.md

  # or nested within separate folders
  - 2020/
    - 03/
      - 2022-03-01.md
    - 04/
      - 2022-04-02.md
```

Periodic Notes 还索引任何包含类似日期模式的文件名。 这意味着它将捕获：

-   202204101611 会议纪要
-   2021.02.04 锻炼日志
-   2001 太空漫游
-   1995 年最佳电子游戏

#### 解析frontmatter

您还可以使用 frontmatter 将笔记分类为定期笔记。 它将检查所有文件的 frontmatter 以查找以下键及其对应的值：

| 关键关键 | 格式 |
| --- | --- |
| 天 | `YYYY-MM-DD` |
| 星期 | `GGGG-[W]WW` |
| 月 | `YYYY-MM` |
| 季 | `YYYY-[Q]Q` |
| 年 | `YYYY` |

例如：

带有这些 frontmatter 键的音符将被归类为 **完全匹配** 。 这意味着打开周期性笔记的命令将打开带有相应frontmatter的笔记。

#### 重新协调多个 **完全** 匹配

对于期望单个 **精确匹配** ，例如“打开今天的每日笔记”，该插件将支持“frontmatter”匹配的笔记，而不是按文件名匹配的笔记。

### 模板标签

| 标签 | 支持的笔记类型 | 描述 | 接受日期计算 |
| --- | --- | --- | --- |
| `title` | _全部_ | 它将插入笔记的标题 | ![X](https://github.githubassets.com/images/icons/emoji/unicode/274c.png) |
| `date`, `time` | _全部_ | 它将插入当前日期/时间。 可选择接受格式。 例如 `{{date:YYYY-MM-DD}}` | ![white_check_mark](https://github.githubassets.com/images/icons/emoji/unicode/2705.png) |
| `yesterday`, `tomorrow` | 日常 | 插入相应的日期。 可选择接受格式。 例如 `{{tomorrow:YYYY-MM-DD}}` | ![white_check_mark](https://github.githubassets.com/images/icons/emoji/unicode/2705.png) |
| `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday` | 每周 | 指一周中的特定日子 `{{sunday:gggg-MM-DD}}`注意，您 **必须** 指定日期格式！ | ![white_check_mark](https://github.githubassets.com/images/icons/emoji/unicode/2705.png) |
| `month` | 月刊 | 指每月的第一天。 可选择接受格式。 例如 `{{month:YYYY-MM}}` | ![white_check_mark](https://github.githubassets.com/images/icons/emoji/unicode/2705.png) |
| `quarter` | 季刊 | 指季度的第一天。 可选择接受格式。 例如 `{{quarter:YYYY-[Q]Q}}` | ![white_check_mark](https://github.githubassets.com/images/icons/emoji/unicode/2705.png) |
| `year` | 每年 | 指一年的第一天。 可选择接受格式。 例如 `{{year:YYYY}}` | ![white_check_mark](https://github.githubassets.com/images/icons/emoji/unicode/2705.png) |

#### 日期计算

Periodic Notes 在模板中提供了非常基本的日期计算。 如果您想链接到周期性模板中的不同日期，这将非常有用。

通过示例可以最好地理解日期计算的语法。 以下是如何 **在 5 天内** ：

您可以添加或减去任意天数（ `d`), 周 ( `w`), 月 ( `m`), 或年 ( `y`).

此功能适用于简单的用例，例如链接后续的日常笔记。 如果您的模板需要更复杂的内容，我强烈建议您将 [Templater](https://github.com/SilentVoid13/Templater) 插件与 Periodic Notes 结合使用。

## 命令

[![图片](https://user-images.githubusercontent.com/693981/163568986-a30bfb3e-3a64-49fe-bdf1-d46ace8c2649.png)](https://user-images.githubusercontent.com/693981/163568986-a30bfb3e-3a64-49fe-bdf1-d46ace8c2649.png)

| 命令名称 | 描述 |
| --- | --- |
| 打开日期切换器 | 打开 [日期切换器](https://github.com/liamcain/obsidian-periodic-notes#%EF%B8%8F-date-switcher) 。 _需要安装自然语言日期插件_ 。 |
| 切换活动日历集... | 从您的日历集列表中选择应该处于 _活动状态_ 。 |
| 打开今天的每日笔记 | 打开或创建当前活动日历集的每日笔记 |
| 打开本周的笔记 | 打开或创建当前活动日历集的周记 |
| 打开本月的笔记 | 为当前活动的日历集打开或创建月度笔记 |
| 打开本季度的笔记 | 打开或创建当前活动日历集的季度注释 |
| 打开今年的笔记 | 打开或创建当前活动日历集的年度注释 |

## 相关插件

-   [自然语言日期插件](https://github.com/argenos/nldates-obsidian) 的 [阿根廷 Ortega Sáinz](https://github.com/argenos)
-   [日历插件](https://github.com/liamcain/obsidian-calendar-plugin)

## FAQ

### 这个和日常笔记插件有什么区别？

每日笔记插件内置于 Obsidian _核心_ 中。 这意味着您可以在不禁用 [安全模式](https://help.obsidian.md/Advanced+topics/Community+plugins) 。 它也很简单：它可以打开或创建今天的每日笔记。 另一方面，Periodic Notes 努力增加与其他插件的更多互操作性。 即使您只对日常笔记感兴趣，定期笔记也能提供很多东西。 它可以创建未来或历史的每日笔记，提供卓越的导航，并允许每天创建多个每日笔记。

### 如何让周数与 Google 日历、Outlook、Fantastical 中的周数匹配？

这些程序符合 **ISO-8601** 周编号规范。 要遵循此标准，请确保您使用的是 `GGGG`和 `WW`您指定格式的令牌。

[![图片](https://user-images.githubusercontent.com/693981/163471298-5c63da1b-7cba-4c94-b0e9-c54818703889.png)](https://user-images.githubusercontent.com/693981/163471298-5c63da1b-7cba-4c94-b0e9-c54818703889.png)

### 如何使用 Templater 完成这项工作？

要在您的定期笔记模板中使用 Templater，请确保在 Templater 中启用以下设置：

[![图片](https://user-images.githubusercontent.com/693981/163508864-4f472a1b-9413-4eb6-93dd-530b31553ce1.png)](https://user-images.githubusercontent.com/693981/163508864-4f472a1b-9413-4eb6-93dd-530b31553ce1.png)

### 我希望在我的定期笔记文件夹的子文件夹中创建新笔记。 我怎么做？

如果您希望新的每日笔记显示在文件夹中 `Journal/2022/`例如，您可以在“格式”字段中包含子文件夹。 例如：

[![图片](https://user-images.githubusercontent.com/693981/163474542-f20c469d-95a1-4e7f-afbb-6f858a9aff32.png)](https://user-images.githubusercontent.com/693981/163474542-f20c469d-95a1-4e7f-afbb-6f858a9aff32.png)

**重要提示：** 请注意，插件将查看 **文件夹** 您提供 因此，即使您希望将日记分成子文件夹， **文件夹** 也应该只引用基本文件夹。

```
journal
  ├── 2021
  │   ├── 2021-12-30.md
  │   └── 2021-12-31.md
  └── 2022
      ├── 2022-04-01.md
      └── 2022-04-02.md
```

对于此配置， **文件夹** 应为 `journal/`是 **格式** 应该 `YYYY/YYYY-MM-DD`.

___

## ![电影带](https://github.githubassets.com/images/icons/emoji/unicode/1f39e.png)学分

对于帮助测试新功能和报告错误的每个人来说都是一件大事。 特别感谢阿根廷 Ortega Sáinz 为 [Natural Language Dates 插件](https://github.com/argenos/nldates-obsidian) 日期切换器

## 说谢谢 ![祈祷](https://github.githubassets.com/images/icons/emoji/unicode/1f64f.png)

如果你喜欢这个插件并且想给我买杯咖啡，你可以！

[![买MeACoffee](https://camo.githubusercontent.com/9098104e5daafdc329a70518b45ded656f305d1043fa6454ce405aec84509740/68747470733a2f2f63646e2e6275796d6561636f666665652e636f6d2f627574746f6e732f76322f64656661756c742d76696f6c65742e706e67)](https://www.buymeacoffee.com/liamcain)

喜欢我的作品并希望看到更多类似的作品？ 你可以赞助我。

[![GitHub 赞助商](https://camo.githubusercontent.com/4ce8053d4717aac49922c22006a22e85a38043da6dcae6f97cefac9b13676b6e/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f73706f6e736f72732f6c69616d6361696e3f7374796c653d736f6369616c)](https://github.com/sponsors/liamcain)
