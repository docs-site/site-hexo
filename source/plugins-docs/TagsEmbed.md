---
title: 标签插件
description: 自己用的一些标签插件
---

> 这部分可以参考：[Tag Plugins Plus | Akilarの糖果屋](https://akilar.top/posts/615e2dec/)，我只引用了部分自己需要的标签。

## <font size=3>一、折叠框 folding</font>

### <font size=3>1. 带颜色的折叠框</font>

```markdown
{% folding, 这是一个默认的折叠框 %}
苏木
{% endfolding %}

{% folding cyan, 这是一个青色的折叠框 %}
苏木
{% endfolding %}

{% folding red, 这是一个红色的折叠框 %}
苏木
{% endfolding %}

{% folding blue, 这是一个蓝色的折叠框 %}
苏木
{% endfolding %}

{% folding purple, 这是一个紫色的折叠框 %}
苏木
{% endfolding %}

{% folding green, 这是一个绿色的折叠框 %}
苏木
{% endfolding %}

{% folding yellow, 这是一个黄色的折叠框 %}
苏木
{% endfolding %}

{% folding orange, 这是一个橙色的折叠框 %}
苏木
{% endfolding %}
```

{% folding, 这是一个默认的折叠框 %}
苏木
{% endfolding %}

{% folding cyan, 这是一个青色的折叠框 %}
苏木
{% endfolding %}

{% folding red, 这是一个红色的折叠框 %}
苏木
{% endfolding %}


{% folding blue, 这是一个蓝色的折叠框 %}
苏木
{% endfolding %}


{% folding purple, 这是一个紫色的折叠框 %}
苏木
{% endfolding %}


{% folding green, 这是一个绿色的折叠框 %}
苏木
{% endfolding %}


{% folding yellow, 这是一个黄色的折叠框 %}
苏木
{% endfolding %}

{% folding orange, 这是一个橙色的折叠框 %}
苏木
{% endfolding %}

### <font size=3>2. 默认打开的折叠框</font>

```markdown
{% folding cyan open, 这是一个青色的默认打开的折叠框 %}
苏木
{% endfolding %}
```

{% folding cyan open, 这是一个青色的默认打开的折叠框 %}
苏木
{% endfolding %}

### <font size=3>3. 嵌套折叠框</font>

```markdown
{% folding red, 查看嵌套测试 %}
{% folding blue, 查看嵌套测试2 %}
{% folding 查看嵌套测试3 %}
苏木
{% endfolding %}
{% endfolding %}
{% endfolding %}
```

{% folding red, 查看嵌套测试 %}
{% folding blue, 查看嵌套测试2 %}
{% folding 查看嵌套测试3 %}
苏木
{% endfolding %}
{% endfolding %}
{% endfolding %}

## <font size=3>二、行内文本样式</font>

```markdown
这是一个带 {% u 下划线 %} 的文本
这是一个带 {% emp 着重号 %} 的文本
这是一个带 {% wavy 波浪线 %} 的文本
这是一个带 {% del 删除线 %} 的文本
这是一个键盘样式的文本 {% kbd command %} + {% kbd D %}
这是一个密码样式的文本：{% psw 密码是没有密码 %}
```

这是一个带 {% u 下划线 %} 的文本

这是一个带 {% emp 着重号 %} 的文本

这是一个带 {% wavy 波浪线 %} 的文本

这是一个带 {% del 删除线 %} 的文本

这是一个键盘样式的文本 {% kbd command %} + {% kbd D %}

这是一个密码样式的文本：{% psw 密码是没有密码 %}

## <font size=3>三、github卡片 ghcard</font>

### <font size=3>1. 用户信息卡片</font>

```markdown
| {% ghcard anuraghazra %} | {% ghcard anuraghazra, theme=vue %} |
| -- | -- |
| {% ghcard anuraghazra, theme=buefy %} | {% ghcard anuraghazra, theme=solarized-light %} |
| {% ghcard anuraghazra, theme=onedark %} | {% ghcard anuraghazra, theme=solarized-dark %} |
| {% ghcard anuraghazra, theme=algolia %} | {% ghcard anuraghazra, theme=calm %} |
```

| {% ghcard anuraghazra %} | {% ghcard anuraghazra, theme=vue %} |
| -- | -- |
| {% ghcard anuraghazra, theme=buefy %} | {% ghcard anuraghazra, theme=solarized-light %} |
| {% ghcard anuraghazra, theme=onedark %} | {% ghcard anuraghazra, theme=solarized-dark %} |
| {% ghcard anuraghazra, theme=algolia %} | {% ghcard anuraghazra, theme=calm %} |

### <font size=3>2. 仓库信息卡片</font>


```markdown
| {% ghcard anuraghazra/github-readme-stats %} | {% ghcard anuraghazra/github-readme-stats, theme=vue %} |
| -- | -- |
| {% ghcard anuraghazra/github-readme-stats, theme=buefy %} | {% ghcard anuraghazra/github-readme-stats, theme=solarized-light %} |
| {% ghcard anuraghazra/github-readme-stats, theme=onedark %} | {% ghcard anuraghazra/github-readme-stats, theme=solarized-dark %} |
| {% ghcard anuraghazra/github-readme-stats, theme=algolia %} | {% ghcard anuraghazra/github-readme-stats, theme=calm %} |
```

| {% ghcard anuraghazra/github-readme-stats %} | {% ghcard anuraghazra/github-readme-stats, theme=vue %} |
| -- | -- |
| {% ghcard anuraghazra/github-readme-stats, theme=buefy %} | {% ghcard anuraghazra/github-readme-stats, theme=solarized-light %} |
| {% ghcard anuraghazra/github-readme-stats, theme=onedark %} | {% ghcard anuraghazra/github-readme-stats, theme=solarized-dark %} |
| {% ghcard anuraghazra/github-readme-stats, theme=algolia %} | {% ghcard anuraghazra/github-readme-stats, theme=calm %} |

### <font size=3>3. 配置项</font>

使用`,`分割各个参数。写法为：`参数名=参数值`，下面是几个常用参数值。

| 参数名        | 取值                                                         | 释义                             |
| :------------ | :----------------------------------------------------------- | :------------------------------- |
| hide          | stars,commits,prs,issues,contribs                            | 隐藏指定统计                     |
| count_private | true                                                         | 将私人项目贡献添加到总提交计数中 |
| show_icons    | true                                                         | 显示图标                         |
| theme         | 可以参考[Available Themes](https://github.com/anuraghazra/github-readme-stats/blob/master/themes/README.md) | 主题                             |

