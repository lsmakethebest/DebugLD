# DebugLD

# 基于Xcode Version 12.1 (12A7403) + Mac OS(10.15.5)

# 编译"ld"target,然后在Product里找到ld的产物，右键finder查看目录

# 某项目使用自定义ld链接
 - Build Setting -> Linking -> Other Linker flags 添加一个参数 -fuse-ld=/Users/<username>/xxx/ld


#调试ld
 - 配置其他项目的参数
    - 在其他项目链接步骤里找到参数,然后在ld64.xcodeproj里设置启动参数
        - ld->edit scheme->Arguments Passed On Launch -> 拷贝上面的所以参数(第一个参数除外，第一个参数是ld无需传参)



# 参考链接
  - https://github.com/dmaclach/ld64
