---
title: 首页公告栏
head:
  - - meta
    - name: description
      content: 了解如何使用 @scenlinx 插件，为你的 VitePress 网站首页添加一个引人注目的公告栏组件。轻松配置和展示活动信息、重要通知或快速安装命令，有效提升首页互动性和信息传递效率。
  - - meta
    - name: keywords
      content: VitePress 首页公告栏 公告栏 @scenlinx Vue组件 主题插件 网站首页 通知栏 活动推广 快速安装 VitePress插件 首页定制
  - - meta
    - property: og:image
      content: /logo/announcement-light.webp
---

![首页公告栏 - 效果图|550x0](/logo/announcement-light.webp#light '首页公告栏 - 效果图')

![首页公告栏 - 效果图|550x0](/logo/announcement-dark.webp#dark '首页公告栏 - 效果图')

## 配置公告栏

```yaml [.vitepress/index.md]
---
layout: home

hero:
  name: AI Wantr
  text: 'Enhanced '
  textsuffix: 'Share'
  tagline: ✨ 集成 Vue 功能组件和主题美化的 VitePress 插件
  prelink: # [!code ++]
    title: '🎉 活动不停歇，青云梯四周年双旦特惠' # [!code ++]
    content: '· 月/季/半年付85折 优惠码<span class="promo-text"> qyt85 </span></br>· 年付以及年付以上8折 优惠码<span class="promo-text"> qyt80</span></br>· 年付8折/2年付7折/3年付6折 配合优惠码折上折，最高可达<span class="promo-text"> 48 </span>折' # [!code ++]
    date: '2025年1月7日23时59分' # [!code ++]
    dateIcon: 'mdi:calendar-star' # [!code ++]
    dateText: '活动截止日期' # [!code ++]
    link: 'https://ai.wantr.cn/qyt' # [!code ++]
---
```

### 复制安装命令

```yaml [.vitepress/index.md]
---
layout: home

hero:
  name: AI Wantr
  text: 'Enhanced '
  textsuffix: 'Share'
  tagline: ✨ 集成 Vue 功能组件和主题美化的 VitePress 插件
  prelink:
    copy: true # [!code ++]
    install: 'pnpm add @scenlinx' # [!code ++]
    title: '<iconify-icon class="i-mr" icon="fa6-solid:bolt" style="color:#63E6BE"></iconify-icon> 快速开始' # [!code ++]
    content: '<span class="promo-text">pnpm add @scenlinx</span>' # [!code ++]
---
```

## 数据接口说明

|    字段    |   类型    | 描述                                                                                                                                                                                                                                                            |
| :--------: | :-------: | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|   `link`   | `string`  | <Badge text="可选" /> 链接的 URL。                                                                                                                                                                                                                              |
|  `title`   | `string`  | 链接的标题。                                                                                                                                                                                                                                                    |
| `content`  | `string`  | <Badge text="可选" /> 链接的内容。                                                                                                                                                                                                                              |
|   `date`   | `string`  | <Badge text="可选" /> 活动截止日期。                                                                                                                                                                                                                            |
| `dateText` | `string`  | <Badge text="可选" /> 活动截止内容。默认为 `活动时间: 即日至;`                                                                                                                                                                                                  |
| `dateIcon` | `string`  | <Badge text="可选" /> 活动截止图标。默认为`line-md:calendar`<iconify-icon icon="line-md:calendar" ></iconify-icon>。支持<Pill name="iconify 图标" link="https://icon-sets.iconify.design/" icon="line-md:iconify2-static" color="#1769AA" alt="iconify icon" /> |
|   `copy`   | `boolean` | <Badge text="可选" /> 复制开关，默认为 `false`，设置为 `true` 时，点击链接将复制 `install` 字段中的内容，**并且链接将无任何跳转行为**                                                                                                                           |
| `install`  | `string`  | <Badge text="可选" /> 复制的内容，当 `copy` 为 `true` 时，点击链接将复制该内容到剪贴板。                                                                                                                                                                        |
|   `alt`    | `string`  | <Badge text="可选" /> 图标的 `alt` 文本                                                                                                                                                                                                                         |
