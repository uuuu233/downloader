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
# 自定义 headers
headers = User-Agent: pan.com
```

站在 `下载器` 视角: 我在启动后会访问一个 `url` 地址, 把响应信息当作 `文件信息`

我要从 `文件信息` 中获取下载文件的 `url`, 并下载文件

所以要为 `文件信息` 配置一个 `url`, 以便能访问

## 下载资源的要求

必须为压缩包的形式, 建议格式为 `zip`, `7z` 等主流格式, `rar` 除外

压缩包内资源禁止套娃, 即让压缩包的根目录就是所有文件, 

下载器会创建一个文件夹(`文件信息` 的 `directory` 决定的文件夹名字), 并把资源解压到这个文件夹下

## 下载源
下载源可使用 `alist` 挂载网盘, 会员基本可以跑满速, 需要一个服务器运行 `alist`

`alist` 提供的下载地址一般会 `302` 转发, 最终不走服务器下载流量

项目链接: https://github.com/alist-org/alist

## 生成下载器
根目录的 `下载器.exe` 只是一个模板, 里面的 `下载信息` 是空的

使用 `下载器生成器.exe` 配置基本信息, 会生成一个新的下载器

# 编译时遇到的问题
因为依赖了 `exui` 需要安装支持库才能使用, `exui` 本身需要收费的

exui 官网: https://exuik.com/

# 可能会报毒, 解决方案
易语言天生就被各种杀软拉黑, 有 2 种解决方案的
1. 使用 `其他资源/虚拟文件打包工具.exe` 将生成的 `下载器.exe` 打包即可

# 萌新使用流程
1. 部署好 `alist`, 并上传所需要下载的文件
2. 获取下载文件的 `url`
3. 编辑好 `文件信息`
4. 上传并复制 `文件信息` 的 `url`
5. 使用 `下载器生成器.exe` 填入 `文件信息` 的 `url` 和背景图片, 并生成

## 流程
<img src="https://github.com/user-attachments/assets/ff029beb-5412-435c-83bf-659812ba9dec" width="50%">

## 软件截图
<img src="https://github.com/user-attachments/assets/d7b16f59-5b98-4823-a5a5-7b317692ebbe" width="80%">

## 卖萌
![296e02d32e5e897284da1c3757649697](https://github.com/user-attachments/assets/fdfd6110-c71a-4587-9098-ca09ededc290)

