# Unity Playground

基于 Unity 的游戏项目模板，集成了 ArkSharp 和多个开源插件，提供完整的游戏开发脚手架。

## 开发环境

- Unity 2022.3.62f2c1 (LTS)
- URP 14.0.2
- Visual Studio 2022 / VSCode / Rider / Cursor

## 集成插件

### 运行时插件

- [ArkSharp](https://github.com/flu3d/arksharp) C# 开发工具箱
- [UniTask](https://github.com/Cysharp/UniTask) 高性能异步编程框架
- [Ingame Debug Console](https://github.com/yasirkula/UnityIngameDebugConsole) 游戏内调试控制台
- [Runtime Inspector](https://github.com/yasirkula/UnityRuntimeInspector) 运行时对象查看器
- [Loop Scroll Rect](https://github.com/qiankanglai/LoopScrollRect) 循环滚动列表优化

### 工具类插件

- [HybridCLR](https://github.com/focus-creative-games/hybridclr_unity) C# 热更新解决方案
- [Tri-Inspector](https://github.com/codewriter-packages/Tri-Inspector) Inspector 增强工具
- [CsprojModifier](https://github.com/Cysharp/CsprojModifier) 项目文件修改器（支持 C# 10）
- [NuGetForUnity](https://github.com/GlitchEnzo/NuGetForUnity) NuGet 包管理
- [ParrelSync](https://github.com/VeriorPies/ParrelSync) 多客户端本地测试

## 项目结构

```
UnityPlayground/
├── Assets/                         # Unity项目主目录
│   ├── Content/                    # 游戏内容资源目录
│   │   └── Blueprints/             # 蓝图脚本
│   ├── Scripts/                    # 项目代码
│   │   ├── Framework/              # 框架层代码，可热更新
│   │   ├── Gameplay/               # 游戏玩法目录，可热更新
│   │   │   ├─ Modules/             # 业务功能模块，每一个业务模块单独一个目录
│   │   │   ├─ Blueprints/          # 蓝图节点代码
│   │   │   └─ Test/                # 游戏玩法测试代码
│   │   └── Editor/                 # 通用编辑器扩展
│   ├── Settings/                   # Unity配置文件
│   └── Plugins/                    # 原生插件与第三方工具
├── Packages/                       # Unity包管理器配置和部分第三方库
├── ProjectSettings/                # Unity项目设置
├── AGENTS.md                       # AI Agent开发指引
└── README.md                       # 本文档
```

## 许可证

本项目模板采用 MIT 许可证，可自由用于商业和非商业项目。
