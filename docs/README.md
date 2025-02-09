# EasyGameFramework

![LICENSE](https://img.shields.io/github/license/JoeyBling/hexo-theme-yilia-plus "LICENSE")
![Author](https://img.shields.io/badge/Author-AILHC-red.svg "Author")

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/AILHC/EasyGameFrameworkOpen)

[![ReadCodeIn1s](https://img.shields.io/badge/ReadCode-In1S-blue.svg)](https://github1s.com/AILHC/EasyGameFrameworkOpen)

<!-- [![Gitpod Ready-to-Code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/AILHC/EasyGameFrameworkOpen) -->
![玩转游戏开发-brightgreen.svg](https://img.shields.io/badge/%E5%BE%AE%E4%BF%A1%E5%85%AC%E4%BC%97%E5%8F%B7-%E7%8E%A9%E8%BD%AC%E6%B8%B8%E6%88%8F%E5%BC%80%E5%8F%91-brightgreen.svg)

基于Typescript的渐进式通用游戏前端开发框架

A progressive universal game front-end development framework based on [Typescript](https://www.tslang.cn/)

## 名词解释

**Easy**

用这个框架开发会是很容易很轻松很舒服的。

**Evolutionary(渐进式)**

用这个框架可以让我循序渐进的开发，而不是一上来就给我整一大套东西。在我有需要时就模块库取或者自己开发。

**General(通用)**

国内的游戏引擎有3个：
* [CocosCreator](https://www.cocos.com/products#CocosCreator)
* [Laya](https://www.layabox.com/)
* [Egret](https://egret.com/products)

其他不太常用的有很多
* [PIXI.js](https://www.pixijs.com/)
* [Phaser](http://phaser.io/)
* ...


各有优势，看项目和团队进行技术选型。

我想这个框架可以不受限于引擎，适用于各种项目，不必因为换引擎而重复造🚗子。


关于框架这个话题我写了几篇文章(感兴趣可以看一下)

* [为什么写框架](https://pgd.vercel.app/2020/11/17/The-Birth-of-Frames-Zero%EF%BC%9AWhy-write-framework/)
* [我想要的框架](https://pgd.vercel.app/2020/11/29/The-Birth-of-a-Framework-One-The-Framework-I-Want/)
* [定位](https://pgd.vercel.app/2020/12/02/The-birth-of-the-framework-two-positioning/)

## 文档网址
    
* [Github上](https://ailhc.github.io/EasyGameFrameworkOpen/#/)
* [Gitee上](https://aigamehome.gitee.io/easygameframeworkopen/#/)

## 在线示例

* [Creator2.x主要模块例子演示Gitee](https://aigamehome.gitee.io/easygameframeworkopen/examples/egf-ccc-full/web-desktop)
* [Creator3.x主要模块例子演示Gitee](https://aigamehome.gitee.io/easygameframeworkopen/examples/egf-ccc3-full/web-desktop)

* [Creator2.x主要模块例子演示GitHub](https://ailhc.github.io/EasyGameFrameworkOpen/examples/egf-ccc-full/web-desktop)
* [Creator3.x主要模块例子演示GitHub](https://ailhc.github.io/EasyGameFrameworkOpen/examples/egf-ccc3-full/web-desktop)
## Modules(模块)

### Core

💗**模块管理器**

框架的核心模块是一个极简强大的模块管理器，可以轻松接入任何TS/JS项目

「传送门」:[egf-core](./packages/core/README.md)

📦**构建工具**

框架的核心工具是一个基于rollup的开箱即用的模块构建工具，可以构建出各种模块规范的js+单.d.ts

同时支持监视开发模式哦

「传送门」:[egf-cli](./packages/cli/README.md)

### 🌈UIFramework 

    一个基于TypeScript的零依赖、跨引擎、高效、灵活、高可扩展的显示控制库(UI框架库)

「传送门」:[display-ctrl](https://github.com/AILHC/EasyGameFrameworkOpen/tree/main/packages/display-ctrl)

在仓库中同时提供了基于CocosCreator2.4.2和CocosCreator3D实现的库(包含layer层级管理库的实现),以及与[FairyGUI](https://www.fairygui.com/)相关的2.x实现和3.x实现
1. [dpctrl-ccc](https://github.com/AILHC/EasyGameFrameworkOpen/tree/main/packages/dpctrl-ccc)
2. [dpctrl-c3d](https://github.com/AILHC/EasyGameFrameworkOpen/tree/main/packages/dpctrl-c3d)
3. [dpctrl-fgui](https://github.com/AILHC/EasyGameFrameworkOpen/tree/main/packages/dpctrl-fgui) 适用于Creator2.x上的fgui适配，同时也适用于Laya、Egret等
4. [dpctrl-fguicc](https://github.com/AILHC/EasyGameFrameworkOpen/tree/main/packages/dpctrl-fguicc) 3.x上的fgui适配

### 🤙🤳🏾 Broadcast
    一个基于TypeScript的一套高效灵活的广播系统，可以帮助开发者轻松、有序的构建具有极具复杂性的关联交互和状态变化的游戏和应用。
**特性**
- 基础事件机制的支持
- 消息支持携带任意类型的数据(并有类型提示)
- 支持函数this绑定或任意类型作为环境，一行代码就可以移除环境内所有的接收者
- 易于构建局部/全局的状态管理
- 支持双向通信
- 支持不可思议的粘性广播
- 基于TypeScript并提供极度舒适的类型提示

「传送门」:[broadcast](./packages/broadcast/README.md)



### 🌐NetworkFramework

    一个基于TypeScript的零依赖、跨平台、灵活、高可扩展的网络库

**特性**

1. 跨平台:适用于任意ts/js项目
2. 灵活、高可扩展:可以根据项目需要进行多层次定制
3. 零依赖
4. 强类型:基于TypeScript
5. 功能强大:提供完整的基本实现:握手、心跳、重连
6. 可靠:完善的单元测试

「传送门」:[enet](./packages/enet/README.md)

### 🕳️ ObjectPoolManager

    一个通用的对象池管理模块，简单易用。

**特性**
1. 全局管理多个对象池
2. 对象无需实现对象池对象接口也可进行获取和回收处理
3. 简洁可扩展的API
4. 智能类型提示
   
「传送门」:[obj-pool](./packages/obj-pool/README.md)

### 🥪LayerManager

    通用层级管理模块，简单易用，对业务层透明。

「传送门」:[layer](./packages/layer/README.md)


## Demos(示例)

框架提供大部分模块的Demo示例供参考
「传送门」:[examples](https://github.com/AILHC/EasyGameFrameworkOpen/tree/main/examples)
## Development Env(开发环境)

这是一个monorepo式的项目仓库，使用这种方式可以很好的管理多模块项目

### Use Tools

* [Lerna](https://lerna.js.org/) 
    > Lerna是一种`monorepo`管理工具，可以优化使用`git`和`npm`管理多包存储库的工作流程。

* [Pnpm](https://www.pnpm.cn/)
    > 最快最稳的`nodejs`包管理工具 墙裂推荐
    > 更加适合在基于`monorepo`的`CocosCreator`项目中使用的`nodejs`管理工具
* 为什么从`Lerna+Yarn` 切换为 `Pnpm + Lerna`

    Yarn 安装包的方式，是扁平化，多个包依赖的包被安装到顶层的`node_modules`。

    这样会导致某个包没有依赖顶层`node_modules`的包，也能引用并调用。

    后果就是，依赖关系不准确，暗藏依赖，在协作时可能会出问题。

    而且`CocosCreator3.x`项目会识别错误，导致报找不到某某依赖的错。

    另外一方面，使用感受上，`Yarn+Lerna`很难用，安装速度慢，偶尔会出点问题。而`Pnpm`则非常舒服
### Reference(参考资料)
1. [Pnpm 中文网](https://www.pnpm.cn/)
2. [Pnpm: 最先进的包管理工具](https://zhuanlan.zhihu.com/p/404784010)
3. [为什么使用pnpm可以光速建立好用的monorepo（比yarn/lerna效率高）](https://blog.csdn.net/qq_21567385/article/details/118590143)

### Pnpm WorkSpace 配置
0. 安装`Pnpm`

    ```bash
    npm i pnpm -g
    ```

1. 创建`pnpm-workspace.yaml`

    ```yaml
    packages:
    # all packages in subdirs of packages/ and components/
    - 'packages/**'
    - 'tool-packages/**'
    - 'transed-packages/**'
    - 'examples/**'
    # exclude packages that are inside test directories
    - '!**/test/**'
    ```
2. 兼容处理
因为很多项目(包括`CocosCreator`)，并不兼容下面这种包引用(protocol)

    ```json
        {
            "dependencies": {
                "foo": "workspace:*",
                "bar": "workspace:~",
                "qar": "workspace:^",
                "zoo": "workspace:^1.5.0"
            }
        }
    ```
    a. 需要创建一个`.npmrc`文件

    ```yaml

    save-workspace-protocol = false

    ```
3. 初始化安装
如果旧项目，可能需要删除掉所有的`node_modules`
之前用`lerna+yarn`的，则可以使用`lerna clean`
然后
    ```bash
    pnpm install
    ```


### Basic Commands

**创建包**
1. 快速模式
    ```bash
    lerna create @xxx/xxx -y
    ```
2. 配置模式
   ```bash
    lerna create @xxx/xxx
   ```
**给包添加依赖**

* 给指定包添加内部包依赖
    ```bash
    pnpm add @xxx/xxx
    ```
* 给指定包添加开发时内部包依赖
    ```bash
    pnpm add -D @xxx/b
    ```
* 给指定包添加外部包依赖(在指定包目录下)
    
    ```bash
    pnpm add xxxx
    ```
* 给指定包添加开发时外部包依赖(在指定包目录下)
    ```bash
    pnpm add xxxx -D
    ```
* 给所有包添加依赖(可以使用pnpm过滤，使用参考:https://www.pnpm.cn/filtering)
    ```bash
    pnpm add lodash --filter "@ailhc/*"
    ```
* 给所有包添加开发时依赖(如果是添加内部包，需要加版本号@0.0.x)
    ```bash
    pnpm add lodash -D --filter "@ailhc/*"
    ```
**移除依赖**
* 移除指定包a对xxx包的依赖(到指定包目录下，也可使用--filter)
    ```bash
    pnpm remove xxx 
    ```
    使用fliter
    ```bash
    pnpm remove xxx --filter "a"
    ```
* 移除所有包对指定包xxx的依赖(可以使用pnpm filter 过滤)
    ```bash
    pnpm remove xxx --filter "@ailhc/*"
    ```
* 移除根目录下对xxx包的依赖
    ```bash
    pnpm remove xxx
    ```
* 安装所有依赖
    ```bash
    pnpm install
    ```
* 清除所有依赖
    ```bash
    lerna clean
    ```
### Version(版本发布)
    lerna version
    会遍历所有包，检查修改，然后更新包的版本号，以及自动修改引用的包的引用版本号
    
    生成一个提交，一个tag，以及推送到远程仓库
    
    比如 packageA 修改了，版本号从1.0.0变成了1.0.1
    
    然后引用了packageA的packageB、C的版本号也要递增，以及引用的packageA的版本号也要从1.0.0变成1.0.1

### Used by other projects(仓库外的开发项目使用模块)
1. 使用npm link 或 yarn link将指定包链接到全局

    ```bash
    cd packages/core
    npm link
    ```

2. 到项目里创建链接(这个@egf/core是包名)
    
    ```bash
    cd cocos-example
    npm link @egf/core
    ```

## Who am I?

**游戏开发之路有趣但不易,**

**玩起来才能一直热情洋溢。**


关注我, 一起玩转游戏开发！

在这游戏开发的道路上并肩前行

你的关注是我持续更新的动力~

在以下这些渠道可以找到我和我的分享和创作:

搜索关注:玩转游戏开发

或扫码:<img src="https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/abd0c14c9c954e56af20adb71fa00da9~tplv-k3u1fbpfcp-zoom-1.image" alt="img" style="zoom:50%;" />



一起讨论技术的 QQ 群: 1103157878

博客主页: https://pgd.vercel.app/

掘金: https://juejin.cn/user/3069492195769469

github: https://github.com/AILHC










