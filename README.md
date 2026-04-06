# touying-pres-cdu Touying 成都大学模板

## 特点
使用莫奈取色完成色彩调配，自动排版

## 演示样例

```typ
#import "@preview/touying-pres-cdu:1.0.0": *

#show: cdu-theme.with(
  config-info(
    title: [标题],
    subtitle: [子标题],
    author: [作者],
    institution: [计算机学院],
    date: datetime.today(),
  ),
)

#title-slide()

#outline-slide(title: "目录")

= 一级标题（no focus）

== 二级标题
#lorem(200)

= 一级标题（focus and repeat)
#focus-slide()

= 一级标题（focus but no repeat)
#focus-slide(title: "一级标题")

== 二级标题
#lorem(200)

#end-slide(content: "Thanks for listening!")
```