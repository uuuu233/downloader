# 悠悠下载器
## 准备工作
- 搭建 `alist`
- 文件信息

## 文件信息
文件信息是为了告诉下载器从什么地址下载资源, 并如何安装

```properties
# 文件的下载地址, 可以设置为 alist 的文件下载地址
url = http://baidu.com?file=11.zip
# 下载的文件名, 建议尾部加个版本号
filename = uumxd_v122.zip
# 程序安装目录
directory = uumxd_v122
# 创建快捷方式时, 桌面的快捷方式名字
shortcut = uumxd
# 创建快捷方式时, 主程序的名字
app = uumxd.exe
```

## 下载的资源

必须为压缩包的形式, 建议格式为 `zip`, `rar`, `7z` 等主流格式

压缩包内资源禁止套娃, 下载器会自动释放资源到 `文件信息` 的 `directory` 目录下

## 下载源
下载源可使用 `alist` 挂载网盘, 会员基本可以跑满速, 需要一个服务器运行 `alist`

`alist` 提供的下载地址一般会 `302` 转发, 最终不走服务器下载流量

项目链接: https://github.com/alist-org/alist

## 生成下载器
根目录的 `下载器.exe` 只是一个模板

使用 `下载器生成器.exe` 配置基本信息, 会生成一个下载器

## 流程
![image](https://github.com/user-attachments/assets/ff029beb-5412-435c-83bf-659812ba9dec)

## 软件截图
![b4626121a5c44d5aa56f85dc888d5c07](https://github.com/user-attachments/assets/d7b16f59-5b98-4823-a5a5-7b317692ebbe)

## 联系作者 
group 652970366
