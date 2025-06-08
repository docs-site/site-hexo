## <font size=3>一、site-hexo</font>

### <font size=3>1. 开发环境</font>

[![Static Badge](https://img.shields.io/badge/author-%E8%8B%8F%E6%9C%A8-blue?style=for-the-badge)](https://sumumm.github.io/)&nbsp;&nbsp;&nbsp;&nbsp;[![Static Badge](https://img.shields.io/badge/GITHUB-sumumm-blue?style=for-the-badge&logo=github)](https://github.com/sumumm)&nbsp;&nbsp;&nbsp;&nbsp;[![Static Badge](https://img.shields.io/badge/NPM-sumumm-blue?style=for-the-badge&logo=npm&logoSize=3&labelColor=%23CB3837)](https://www.npmjs.com/~sumumm)

[![node](https://badgen.net/static/node/v22.16.0/F96854)](https://nodejs.org/dist/v22.16.0/node-v22.16.0-win-x64.zip)&nbsp;&nbsp;&nbsp;&nbsp;[![npm](https://badgen.net/static/npm/10.9.2/F96854)](https://badgen.net/static/npm/10.9.2/F96854)&nbsp;&nbsp;&nbsp;&nbsp;[![hexo](https://badgen.net/static/hexo/7.3.0/cyan)](https://github.com/hexojs/hexo/releases/tag/v7.3.0)

### <font size=3>2. 建立site</font>

#### <font size=3>2.1 hexo-cli</font>

```shell
npm install hexo-cli -g # 全局安装hexo
hexo -v
```

#### <font size=3>2.2 初始化site</font>

```shell
hexo init <folder>
cd <folder>
npm install
```

<img src="./README/img/image-20250601194445163.png" alt="image-20250601194445163" />

#### <font size=3>2.3 本地预览</font>

```shell
hexo g # hexo generate 生成静态文件
hexo s # hexo server 启动服务器。 默认情况下，访问网址为： http://localhost:4000/。
```

## <font size=3>二、hexo命令</font>

### <font size=3>1. [hexo init](https://hexo.io/zh-cn/docs/commands#init)</font>

```shell
$ hexo init [folder]
```

新建一个网站。 如果没有设置 `folder` ，Hexo 默认在目前的文件夹建立网站。这个命令相当于执行了以下几步：

- （1）Git clone [hexo-starter](https://github.com/hexojs/hexo-starter) 和 [hexo-theme-landscape](https://github.com/hexojs/hexo-theme-landscape) 主题到当前目录或指定目录。

- （2）使用 [Yarn 1](https://classic.yarnpkg.com/lang/en/)、[pnpm](https://pnpm.io/zh/) 或 [npm](https://docs.npmjs.com/cli/install) 包管理器下载依赖（如有已安装多个，则列在前面的优先）。 npm 默认随 [Node.js](https://hexo.io/zh-cn/docs/index.html#安装-Node-js) 安装。

### <font size=3>2. [hexo new](https://hexo.io/zh-cn/docs/commands#new)</font>

```shell
$ hexo new [layout] <title>
```

新建一篇文章。 如果没有设置 `layout` 的话，默认使用 [_config.yml](https://hexo.io/zh-cn/docs/configuration) 中的 `default_layout` 参数代替。 使用布局 `draft` 来创建草稿。 如果标题包含空格的话，请使用引号括起来。

### <font size=3>3. [hexo generate](https://hexo.io/zh-cn/docs/commands#generate)</font>

```shell
$ hexo generate
```

生成静态文件。

### <font size=3>4. [hexo server](https://hexo.io/zh-cn/docs/commands#server)</font>

```shell
$ hexo server
```

启动服务器。 默认情况下，访问网址为： `http://localhost:4000/`。

### <font size=3>5. [hexo clean](https://hexo.io/zh-cn/docs/commands#clean)</font>

```shell
$ hexo clean
```

清除缓存文件 (`db.json`) 和已生成的静态文件 (`public`)。

## <font size=3>三、参考资料</font>

> - [Hexo](https://hexo.io/zh-cn/)

## <font size=3>四、小徽章</font>

>- [badgen.net](https://badgen.net/)
>- [Shields.io | Shields.io](https://shields.io/)
>- [For the Badge](https://forthebadge.com/)

