<h1 align = "center">需求分析文档</h1>

## 1. 引言
本文档描述了Android平台翻译App的用户需求规格，旨在指导开发团队按照这些规格开发应用。

## 2. 项目概述

### 2.1 项目描述

Android平台翻译App旨在提供用户便捷的翻译服务，支持多种语言互译，满足用户在日常生活和工作中的翻译需求。

### 2.2 用户目标

Android平台翻译App的主要用户包括普通用户和专业用户，他们的需求主要包括快速准确的翻译服务、便捷的操作体验和个性化定制功能。

### 2.3 业务目标

Android平台翻译App的业务目标是提供高质量的翻译服务，提升用户体验，增加用户粘性，并通过付费订阅等方式实现商业盈利。

## 3. 功能需求

### 3.1 用户故事

1. **用户故事1：** 
   - 描述：作为一个用户，我希望能够输入需要翻译的文本，并选择目标语言，以便快速获取翻译结果。
   - 优先级：高

2. **用户故事2：**
   - 描述：作为一个用户，我希望能够查看翻译历史记录，方便我回顾之前的翻译内容。
   - 优先级：中

3. **用户故事3：**
   - 描述：作为一个用户，我希望能够收藏常用的翻译结果，以便下次直接使用，节省时间。
   - 优先级：中

4. **用户故事4：**
   - 描述：作为一个用户，我希望能够使用语音输入功能进行翻译，方便我在无法打字的情况下使用。
   - 优先级：高

5. **用户故事5：**
   - 描述：作为一个用户，我希望能够使用图片翻译功能，将拍摄的图片中的文字翻译成目标语言。
   - 优先级：高

### 3.2 功能列表

- **文本翻译：** 用户可以输入文本并选择目标语言进行翻译。
- **翻译历史：** 用户可以查看之前的翻译记录，并选择删除部分历史记录或是全部历史记录。
- **收藏功能：** 用户可以收藏常用的翻译结果，在下次输入时优先匹配。
- **语音翻译：** 用户可以使用语音输入进行翻译。
- **图片翻译：** 用户可以使用拍照或从相册选择图片，将其中的文字进行翻译，并选择以何种方式呈现（在原文字下方显示或覆盖原文字显示）。
- **语言识别：** 用户可以通过语音输入，系统识别出用户的语音内容并显示在屏幕上，并显示出对应的翻译结果。
- **个性化设置：** 用户可以在设置界面进行个性化的配置，例如设置常用翻译语言，设置夜间模式等。

## 4. 非功能需求

### 4.1 性能要求

- 应保证翻译速度快，响应时间在1秒以内。

### 4.2 安全性要求

- 用户数据应进行加密存储，确保用户隐私安全。

### 4.3 可用性要求

- 应提供简洁直观的用户界面，保证用户操作便捷。

## 5. 用户界面设计

### 5.1 页面布局

- 主界面应包含文本输入框、目标语言选择框、翻译按钮等核心元素。
- 翻译历史和收藏夹应以列表形式展示。

### 5.2 界面元素

- 使用清晰易懂的图标和文字，提高用户识别度和操作性。

## 6. 数据模型

### 6.1 数据库设计

- 使用本地数据库存储用户的翻译历史和收藏内容。

### 6.2 数据流程

- 用户输入的文本经过处理后发送给翻译引擎，获取翻译结果后展示给用户。

## 7. 接口需求

### 7.1 外部接口

- 需要接入翻译引擎的API，以实现文本翻译功能。
- 图片翻译功能需要接入图片识别和文字翻译的API。
- 语音翻译功能需要接入语音识别和文字翻译的API。

### 7.2 内部接口

- 与本地数据库进行交互，实现翻译历史和收藏夹的管理功能。

## 8. 系统约束

- 开发语言：Java
- 最低Android版本：Android 11.0

## 9. 用例图

- <img src="https://github.com/CPLASF2049/TranslateApp-Android/blob/main/pics/Use%20Case%20Diagram.png" width="400">

## 10. 原型
<div align = "center">
- <img src="https://github.com/CPLASF2049/TranslateApp-Android/raw/main/pics/Text%20Translation.png" width="18%" />
- <img src="https://github.com/CPLASF2049/TranslateApp-Android/raw/main/pics/Image%20translation.png" width="18%" />
- <img src="https://github.com/CPLASF2049/TranslateApp-Android/raw/main/pics/Speech%20Translation.png" width="18%" />

</div>
 
 <div align = "center">
- <img src="https://github.com/CPLASF2049/TranslateApp-Android/raw/main/pics/Historical%20translation.png" width="18%" />
- <img src="https://github.com/CPLASF2049/TranslateApp-Android/raw/main/pics/My%20(It's%20so%20hard%20to%20translate%20that%20I%20have%20to%20use%20this%20abstract%20name).png" width="18%" />
- <img src="https://github.com/CPLASF2049/TranslateApp-Android/raw/main/pics/Settings.png" width="18%" />
</div>
 
  
