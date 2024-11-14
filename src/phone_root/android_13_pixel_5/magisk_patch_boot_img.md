# 用Magisk去给boot.img打patch

将`boot.img`下载到Pixel5手机中（的下载目录）：

```bash
adb push boot.img /sdcard/Download
```

再去Magisk中：

* 概述：`Magisk`->`安装`->`选择并修补一个文件`->（从下载目录中）选择`boot.img`->`开始`->`完成`->输出log中会有打了patch的`boot.img`
* 详解：
  * 点击打开Magisk
    * ![pixel5_home_magisk](../../assets/img/pixel5_home_magisk.png)
  * 点击Magisk中的主页中的：安装
    * ![magisk_home_install](../../assets/img/magisk_home_install.png)
  * 选择并修补一个文件
  * （从下载目录中）选择`boot.img`
    * ![android_download_foder_boot_img](../../assets/img/android_download_foder_boot_img.png)
  * 开始
  * 完成
    * ![magisk_patch_boot_img_done](../../assets/img/magisk_patch_boot_img_done.png)
  * 输出log中会有打了patch的`boot.img`
    ```bash
    Output file is written to 
    /storage/emulated/0/Download/magisk_patched-26100_bMrsR.img
    ```
    * 其中：
      * `/storage/emulated/0/Download/magisk_patched-26100_bMrsR.img`
        * == `/sdcard/Download/magisk_patched-26100_bMrsR.img`
      * 就是我们要的，打好了`patch`的`boot.img`
  * 把打了patch的`boot.img`上传到电脑端，供后续使用
    * 把此处打了patch的`boot.img`是`magisk_patched-26100_bMrsR.img`，从安卓手机中上传到电脑（Mac）中
      ```bash
      adb pull /sdcard/Download/magisk_patched-26100_bMrsR.img .
      ```
