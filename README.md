# ⭐⭐⭐ Star This Project ⭐⭐⭐

如果您觉得这个项目对您有帮助，请给我一个 ``Star`` 或 ``进行赞助``！您的支持是我持续改进的动力。❤❤❤

如果遇到问题欢迎提交``issue``！也随时欢迎``Pull Requests``！

[![Channel](https://img.shields.io/badge/Follow-Telegram-blue.svg?logo=telegram)](https://t.me/gki_kernels_xiaoxiaow) [![Coolapk](https://img.shields.io/badge/Follow-Coolapk-3DDC84?style=flat-square&logo=android&logoColor=white)](https://www.coolapk.com/u/24701380)

<img width="250" height="250" alt="image" src="https://github.com/user-attachments/assets/55acad97-8fe6-4de7-b9ce-90da9552a212" />

## OnePlus 开源地址

[![OnePlus Repository](https://img.shields.io/badge/OnePlus-Repository-red)](https://github.com/Xiaomichael/kernel_manifest)
Tips: 最近上游内核源码可能会出现刷入不开机的情况，请仔细辨别

## 设备支持

支持欧加真内核版本 `5.10-6.6` 的设备，只要跑出来内核版本号一样(或大于的可以尝试一下)就可以用

内核版本为 `6.12` 的可以去这个 [专用仓库](https://github.com/Xiaomichael/oppo_oplus_realme_sm8850)

## KernelSU管理器支持

支持 ``ReSukiSU`` ``SukiSU Ultra`` ``KernelSU Next`` ``KernelSU Official``, 当然你也可以编译仅加入优化的 ``无 Root`` 内核

Tips: SukiSU 由于长期不更新 编译时容易报错且稳定性较差 已经不推荐使用 建议使用ReSukiSU

## 使用指南

### ① 分支选择

1. 点击 `Branches` 切换处理器分支
2. 选择适合您设备的配置 (Tips: 如果实在找不到代号名称去网上搜搜)

<img width="376" height="77" alt="{B57A09D0-EC2F-4B86-9821-9C6CAC6435CF}" src="https://github.com/user-attachments/assets/0f97b652-b1e4-484d-90c0-9e36bc15cdf0" />

### ② 配置文件说明

- `_b` 后缀：ColorOS/OxygenOS 16
- `_v` 后缀：ColorOS/OxygenOS 15
- `_u` 后缀：ColorOS/OxygenOS 14
- `_t` 后缀：ColorOS/OxygenOS 13

<img width="1122" height="257" alt="image" src="https://github.com/user-attachments/assets/24631b01-ec9d-4f77-a764-476cfe522537" />

### ③ 配置开关建议 & 内核特性

- **SUSFS选项**: SUSFS在编译时已经改为可选，看你的需求进行开关。近期上游在拉💩💩💩, 建议关闭
- **KPM选项**: 仅在 ``SukiSU Ultra`` 支持开启，建议禁用以减少电量消耗，挂🐕去④
- **lz4kd**: 
  - ``6.1系``内核：建议关闭该选项以获得更好的 `lz4 + zstd` 压缩方式
  - ``6.6系``内核：建议关闭该选项以获得更好的 `lz4` 压缩方式
  - ``5.10 - 5.15系``内核：建议保持开启
- **BBR算法**: 对手机日用无太大意义甚至可能``负优化``，推荐关闭
- **BBG基带守护**: 推荐开启，看名字就知道是干啥的
- **⚠️代理优化**: 骁龙芯片可以开，联发科芯片 `千万不要开` ，否则出现恶性Bug！
- **是否添加Unicode零宽绕过修复补丁**: 仅推荐内核KMI版本为``android12-5.10``开启, ``5.15 - 6.12``可以使用 [这个 LSPosed 模块](https://t.me/real5ec1cff/271) 无痛修复

### ④ 作者碎碎念

- **关于元模块**: 推荐[Magic Mount - rs](https://github.com/Tools-cx-app/meta-magic_mount-rs/releases)
