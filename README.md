# hepatitisA

## 项目简介

甲肝暴发流行预测预警模型构建及应用 - 患者信息登记与知情同意书签署系统

这是一个基于 Web 的移动端应用，用于甲型肝炎患者信息采集和电子知情同意书签署，支持手写签名功能。

## 功能特性

- 📝 患者个人信息录入（姓名、手机号、身份证号）
- ✍️ 电子知情同意书在线签署
- 🖊️ Canvas 手写签名功能（支持患者本人及代理人签名）
- 📱 手机验证码验证
- 📋 问卷访问和血样采集同意选项
- 🔒 信息加密与隐私保护

## 技术栈

- **前端框架**: AngularJS + Ionic Framework
- **UI 组件**: MUI (Mobile UI)
- **手写签名**: Tablet.js (Canvas 写字板)
- **其他依赖**:
  - jQuery 2.2.4
  - EXIF.js (图片元数据处理)
  - 微信 JS-SDK (jweixin-1.2.0)
  - Ripple 效果

## 项目结构

```
hepatitisA/
├── index.html                          # 入口文件（重定向到注册页）
├── hepatitisA/
│   ├── register/
│   │   ├── register.html              # 注册主页面
│   │   └── resources/
│   │       ├── css/                   # 样式文件
│   │       ├── js/                    # 业务逻辑
│   │       └── img/                   # 图片资源
│   └── resources/
│       └── js/
│           └── app.js                 # AngularJS 应用配置
└── resources/
    ├── css/                           # 全局样式
    ├── js/                            # 公共 JS
    └── plugin/                        # 第三方插件库
```

## 快速开始

### 本地运行

1. 克隆项目到本地
```bash
git clone [repository-url]
cd hepatitisA
```

2. 使用本地服务器运行（推荐使用 Live Server 或其他 HTTP 服务器）
```bash
# 使用 Python 简易服务器
python -m http.server 8080

# 或使用 Node.js http-server
npx http-server -p 8080
```

3. 在浏览器中访问
```
http://localhost:8080
```

### 移动端调试

建议使用浏览器的移动设备模拟器进行调试，或直接在移动设备上访问。

## 使用流程

1. **输入个人信息** - 填写姓名、手机号、身份证号
2. **签署知情同意书** - 阅读知情同意书内容
3. **手写签名** - 患者本人或代理人进行手写签名
4. **输入验证码** - 接收并输入手机验证码
5. **完成注册** - 提交表单完成注册流程

## 在线预览

<p>预览：<a href='http://demo.xiaowiba.com/demo/hepatitisA/hepatitisA/register/register.html'>http://demo.xiaowiba.com/demo/hepatitisA/hepatitisA/register/register.html</a></p>

## 项目背景

本项目用于支持"甲肝暴发流行的预测预警模型构建及应用"研究项目（方案编号：20181206），由浙江大学第一附属医院和中国疾病预防控制中心病毒病预防控制所联合开展。

## 注意事项

- 本项目需要在移动端浏览器中运行以获得最佳体验
- 手写签名功能依赖 Canvas API，请确保浏览器支持
- 验证码功能需要后端接口支持
- 项目包含患者隐私信息，请注意数据安全和隐私保护

## 浏览器兼容性

- iOS Safari 9+
- Android Chrome 4.4+
- 微信内置浏览器

## 许可证

请遵守相关医疗数据隐私保护法规和伦理委员会要求。
