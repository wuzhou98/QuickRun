# 更新日志

## 0.7.4.8
- 优化编辑器
- 修复版本`0.7.4.6`中, 文件拖拽至进程Item无效的问题

## 0.7.4.6
- 重写QuickRun加载和调用Item过程, 采用DataTemplate来控制按钮生成 [#9](https://github.com/Zaeworks/QuickRun/pull/9)
- 添加分部(外部)配置支持, 添加DesignPath属性 [#7](https://github.com/Zaeworks/QuickRun/pull/7)
- 添加扩展功能-重载配置 [#8](https://github.com/Zaeworks/QuickRun/pull/8)
- 修复重载配置后, 目录无法回到主页的Bug
- 当属性值长度超过70时, 会作为子Element存入配置文件中
- 现在读写配置文件时只会序列化/反序列化可读可写(CanRead&CanWrite)的Item属性

## 0.7.2.2
- 添加非标准插件支持 [#5](https://github.com/Zaeworks/QuickRun/pull/5)
- 改良键盘操作 [#6](https://github.com/Zaeworks/QuickRun/pull/6)
- 修复编辑器拖拽错乱的Bug
- 修复重载配置文件后, 后退可能导致的崩溃问题

## 0.7.0.0
#### 启动器改动
- 修复右键拖动窗口崩溃问题
- 按下右键可以返回上一页
- 增加Item配置属性Plugin
- 修改配置和样式模板
- 加入程序启动参数`-h`(启动时隐藏界面)
#### 插件相关
- 添加QuickRun.Plugin程序集, 包含插件接口IPlugin, IDragDrop; 包含基类Plugin, DragDropPlugin及两个衍生类
- 允许开发者引用程序集QuickRun.Plugin开发QuickRun插件
- 添加启动器扩展QuickRun.Extension, 包含模板导出和开机启动功能
#### 编辑器改动
- 优化代码
- 修复模板加载问题
- 添加关闭时的保存提示
- 实现节点移除
- 修改新节点位置

## 0.6.2
- 修复标题问题
- 设置程序所在目录为默认工作目录
- 添加Arguments属性, 作为本地进程的启动参数
- 添加Admin属性(以管理员身份运行)

## 0.6.1
- 启动器不再依赖编辑器, 且可以直接加载配置文件, 无需生成
- 启动器监控并自动重载配置文件
- 编辑器现在需要依赖启动器才能运行, 并从启动器中加载模板
- 增加多样式支持
- 配置模板和样式模板更新
- 添加StayOpen和Style属性

## 0.5.5
- 添加Enabled属性
- 添加拖拽支持; 拖拽时可以翻页
- 改良编辑器的配置读写功能, 并可以单独导出样式模板
- 配置和样式寻找优化, 载入优化

## 0.5
- 初发布版本
