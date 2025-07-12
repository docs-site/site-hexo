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
