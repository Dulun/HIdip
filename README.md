#**简单开启HIDIP**

  下载 **DisplayProductID-a0a4** 重命名放入指定文件夹
  
  **获取显示器ID**
  
  在终端中输入下面命令
  
  `ioreg -l | grep DisplayVendorID`
 

  就可以可以看到DisplayVendorID (显示器制造商ID)
  
  如 ”DisplayVendorID" = 16652

  然后，在终端中输入下面命令
  
  `ioreg -l | grep DisplayProductID`

  就可以看到DisplayProductID (显示器产品ID)
  
  如 "DisplayProductID" = 49297

  这两个数字都是十进制的，用计算器功能或在线转换把它们换算成16进制。
  
  以上面为例

  `16652 ==> 410c`
  
  `49297 ==> c091`

  新建文件夹改名为 **DisplayVendorID-410c**
  
  下载 **DisplayProductID-a0a4** 改为 **DisplayProductID-c091** 放入 **DisplayVendorID-410c** 文件夹
  
  然后把修改好的文件夹放入目录：
  
  `/System/Library/Displays/Contents/Resources/Overrides/`
