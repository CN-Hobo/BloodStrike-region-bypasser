# BloodStrike-region-bypasser
[![GitHub stars](https://img.shields.io/github/stars/CN-Hobo/BloodStrike-region-bypasser?style=flat-square)](https://github.com/CN-Hobo/BloodStrike-region-bypasser/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/CN-Hobo/BloodStrike-region-bypasser?style=flat-square)](https://github.com/CN-Hobo/BloodStrike-region-bypasser/fork)
[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](LICENSE)
[![Language](https://img.shields.io/github/languages/top/CN-Hobo/BloodStrike-region-bypasser?style=flat-square)]()

> 该项目使用了AI协助完成。

## 📖 工具介绍
针对于Steam端的游戏BloodStrike(译名:血战突袭)中登录时，提示“由于地区限制无法登录”的解决补丁工具，非常-非常简易的IP地区检测绕过工具。
而且在大陆内陆地区裸连亚服也才40ms左右延迟，这样可以解决进游戏必须挂加速器的问题。

## 🚩 如何使用
以下方法按你实际情况选择：
  - 电脑"有"Python环境：直接下载源码中 main.py 文件，并自行方式执行。
  - 电脑"无"Python环境：下载[Release](https://github.com/CN-Hobo/BloodStrike-region-bypasser/releases/latest)中预编译好的exe文件，可直接双击执行。
- 完成以上的启动操作后，点击“选择游戏文件夹”后选择你的 BLOODSTRIKE 游戏根目录，例如 D:\SteamLibrary\steamapps\common\BLOODSTRIKE 即可

## ✨ 主要原理
  1. 游戏启动时会向 `https://mgbnaeast-g83naxx1ena.unisdk.easebar.com/g83naxx1ena/sdk/dlc_sync` 发送POST请求
  2. 其中请求参数中包含参数名为"aim_info"，且参数值中包含"country":"国际代码"，当国际代码为CN时游戏将会提示不支持该地区
  3. 工具通过直接改掉"aim_info"这个标识，让游戏找不到地方来检查玩家的地区，从而实现可全程裸连

## 🚀 使用要求
### 环境依赖
- Windows & Python 3.8+
- 会python main.py

### **⚠️ 免责声明**  
1。 **资源性质**  
   - 本资源仅供**个人学习、技术交流**，禁止用于商业用途。  
   - 根据原作者的许可协议（如GPL/MIT/CC-BY等），**用户需自行遵守相关规定**。    

2。 **用户责任**  
   - 下载后请于24小时内删除，并支持正版或原作者。  
   - 因使用本资源导致的任何法律纠纷或损失，**由使用者自行承担**。   
