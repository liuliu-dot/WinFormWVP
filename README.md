# WinFormWVP

## 项目简介

这是一个基于 WinForm-MVP 架构模式的上位机应用程序，采用 .NET Framework 4.6.1 目标框架，并使用工厂设计模式来管理多种设备。

## 支持的设备

- **VDC_32** - 设备型号1
- **GJ750_4_60A** - 设备型号2

## 项目结构

```
WinFormWVP/
├── src/
│   ├── Models/                    # 数据模型层
│   │   └── .gitkeep
│   │
│   ├── Views/                     # 视图层 (WinForm 窗体)
│   │   └── .gitkeep
│   │
│   ├── Presenters/                # 表示器层 (业务逻辑)
│   │   └── .gitkeep
│   │
│   ├── Devices/                   # 设备相关类
│   │   ├── VDC_32/               # VDC_32 设备实现
│   │   │   └── .gitkeep
│   │   │
│   │   └── GJ750_4_60A/          # GJ750_4_60A 设备实现
│   │       └── .gitkeep
│   │
│   ├── Factory/                   # 工厂模式相关类
│   │   └── .gitkeep
│   │
│   ├── Interfaces/                # 接口定义
│   │   └── .gitkeep
│   │
│   └── Common/                    # 公共工具类和辅助方法
│       └── .gitkeep
│
└── README.md
```

## 架构说明

### MVP 模式

- **Model (模型)**: 负责数据的存储和业务逻辑
- **View (视图)**: 负责用户界面展示，仅处理 UI 相关逻辑
- **Presenter (表示器)**: 作为 Model 和 View 之间的桥梁，处理业务逻辑

### 工厂模式

使用工厂模式来创建不同类型的设备实例，便于扩展新设备类型。

## 技术栈

- .NET Framework 4.6.1
- Windows Forms
- MVP 架构模式
- 工厂设计模式

## 开发环境要求

- Visual Studio 2017 或更高版本
- .NET Framework 4.6.1 SDK