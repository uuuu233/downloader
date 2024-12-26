# 悠悠下载器
## 食用方式
下载器下载什么? 解压的文件名是什么? 文件md5是什么? 需要先配置文件信息才行
1. 配置 `文件信息`, 并提供 `http` 接口
2. 在程序中设置 `文件信息` url
3. 编译, 起飞~
```
// 伪代码
function __启动窗口_创建完毕() {
    文件信息_url ＝ "http://localhost/fileinfo"
}
```

## 在线文件信息
```properties
# = 号左右两边不能有空格
# 文件的下载地址, 支持302
url=http://baidu.com?file=11.zip
# 文件的md5, 下载文件后会校验正确性
md5=BFB10A76EB3B379DBD69BEBE2F0F9BB7
# 下载的文件名, 一般来说 可以加个版本号
filename=uumxd_v122.zip
# 选择解压目录时, 自动追加的文件夹名字
directory=uumxd_v122
# 创建快捷方式时, 桌面的快捷方式名字
shortcut=uumxd
# 创建快捷方式时, 主程序的名字
app=uumxd.exe
```

## 下载文件结构
压缩包根目录直接放文件就行, 不要再包裹一层目录, 解压时由 `directory` 控制目录名

## 下载源
下载源可使用 `alist` 挂载网盘, 会员基本可以跑满速, 需要一个服务器运行 `alist`

在使用 `alist` 提取到的文件链接, 其实不是真实下载链接, 最终会 `302`, 不走服务器下载流量

项目链接: https://github.com/alist-org/alist

## 依赖
以下依赖均开源, 除 exui
- 精易模块
- zyJson
- 7z
- aria2
- exui

## 流程
![image](https://github.com/user-attachments/assets/b749ba34-b24a-4db8-8d67-5267e9d0d7ad)

## 软件截图
![b4626121a5c44d5aa56f85dc888d5c07](https://github.com/user-attachments/assets/d7b16f59-5b98-4823-a5a5-7b317692ebbe)


## 联系作者 
group 652970366



