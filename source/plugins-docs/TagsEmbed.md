---
title: 标签插件
description: 自己用的一些标签插件
---

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

