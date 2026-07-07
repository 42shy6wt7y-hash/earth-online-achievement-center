# 地球online成就中心

一个本地离线的黑金 Steam 风人生成就陈列馆。

## 普通用户

下载发布页里的 `EarthOnlineAchievementCenter-Setup.exe`，双击安装。安装完成后桌面会自动生成 `地球online成就中心` 快捷方式，图标使用项目徽章图。

应用默认安装在：

```text
C:\Users\<你的用户名>\AppData\Local\Programs\EarthOnlineAchievementCenter
```

用户成就档案默认保存在：

```text
C:\Users\<你的用户名>\AppData\Local\EarthOnlineAchievementCenter\achievement-archive
```

界面里的删除只是写入删除事件，不会移除旧文件。

## 开发启动

运行本地网页服务：

```powershell
npm start
```

然后打开：

```text
http://localhost:3217
```

## 开发模式本地档案

网页服务开发模式的数据保存在项目里的 `achievement-archive/`：

- `events/`：创建、修改、删除事件，只增不删
- `assets/`：上传过的图片，只增不删

## 打包 Windows 安装包

```powershell
npm run build:windows
```

产物会生成在 `dist/EarthOnlineAchievementCenter-Setup.exe`。
