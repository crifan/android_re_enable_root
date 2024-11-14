# Kitsune Mask中root相关设置

同理，`Kitsune Mask`和`Magisk`中的配置和逻辑：

[Magisk中root相关设置](../../phone_root/android_13_pixel_5/magisk_root_config.md)

几乎一样。

但也还是再仔细介绍一下：

---

正常进入已root后的`Kitsune Mask`的界面是：

![kitsune_mask_rooted_ui](../../assets/img/kitsune_mask_rooted_ui.png)

常规的逻辑和功能：

## 如何判断是否已经root成功？

`超级用户`和`模块`：不是灰色，是白色，且可以点击，表示：已获取了root权限

## 超级用户

* `超级用户`
  * ![kitsune_mask_root_white](../../assets/img/kitsune_mask_root_white.png)

## 模块

* `模块`
  * ![kitsune_mask_module_empty](../../assets/img/kitsune_mask_module_empty.png)

## 设置

* 设置
  * 进入方式：点击`Kitsune Mask`主页的右上角**齿轮⚙**按钮
  * 默认的一些设置
    * ![kitsune_mask_settings_1](../../assets/img/kitsune_mask_settings_1.png)
    * ![kitsune_mask_settings_2](../../assets/img/kitsune_mask_settings_2.png)
    * ![kitsune_mask_settings_3](../../assets/img/kitsune_mask_settings_3.png)

### 改动一些配置

* 自动响应
  * 之前：`提示`
    * 图
      * ![kitsune_mask_root_notice](../../assets/img/kitsune_mask_root_notice.png)
    * 效果和逻辑：别人应用申请获取root后，此处会弹框提示，需要用户手动点击允许，才能真正获取root权限 =》比较麻烦
  * 现在改为：`（自动）允许`
    * 图
      * ![kitsune_mask_root_auto_allow](../../assets/img/kitsune_mask_root_auto_allow.png)
    * 效果和逻辑：别人应用申请获取root后，自动就同意，无需用户手动同意，更加方便

## 日志

* 日志
  * ![kitsune_mask_log_1](../../assets/img/kitsune_mask_log_1.png)
  * ![kitsune_mask_log_2](../../assets/img/kitsune_mask_log_2.png)
  * ![kitsune_mask_log_3](../../assets/img/kitsune_mask_log_3.png)
