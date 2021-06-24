# 橙 狐 (OFRP) for Redmi 10X 5G（atom）
使用红米 10X 5G，MIUI 12.5（安卓11）制作，提取官方安卓11内核，适用于橙狐安卓10分支

![OFRP](https://image.ibb.co/cTMWux/logo.jpg "OFRP")

====================================================

# 目前进度
更新中......

不支持Data解密，需要格式化Data分区后才能正常读写（由于官方miui有强制加密，建议使用官改）

震动功能无效

等一个大佬来帮忙解决上面两个问题

感谢ymdzq大佬指点。

# 如何构建
下载OFRP源代码，克隆这个仓库放到相应的位置

例如OFRP源代码根目录为~/OrangeFox_10/fox_10.0，则保存为~/OrangeFox_10/fox_10.0/device/xiaomi/atom/:

```bash
cd ~/OrangeFox_10/fox_10.0
mkdir -p device/xiaomi
cd device/xiaomi
git clone https://github.com/sumiort/OFRP-device_xiaomi_atom.git atom
```

打开源代码根目录运行:

```bash
. build/envsetup.sh && lunch omni_atom-eng && mka recoveryimage
```
