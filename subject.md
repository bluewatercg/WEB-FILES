# 初级实战【IP地址查询】
## 项目要求：
FILES实战教程中，getFile云函数的实现采用了腾讯验证码进行用户行为校验，而验证码校验需要获取用户IP地址。
请根据getFile云函数的实现原理，制作一个简单的web网页，功能为打开页面自动查询显示本机的IP地址。
你可以有如下的实现方法：
- 1.参照云函数http触发的集成响应，直接返回html代码。当访问云函数触发链接时，直接渲染页面显示。
- 2.制作一个简单的html网页，使用request请求向云函数发起获取ip地址，然后显示。html文件放到静态托管中，也可以放到文件存储中。
## 本级项目注意点：
在使用html发起request请求的方法中，会遇到跨域的问题。
## 本级项目考验点：
- 云函数的HTTP触发配置
- 云函数HTTP触发的集成响应
## 提交材料：
- 1.可访问的功能展示地址
- 2.功能视频录屏
- 3.代码核心的压缩文件：云函数的代码和html文件代码，不需要传所有项目目录代码。

# 中级实战【文件下载区】
## 项目要求：
制作一个文件下载专页，用于某些机构特定场景下的文件下载。比如学校或者公司专门的下载站点。
构建一个web页面，进入后展示文件列表。文件列表有数据库做维持，可以动态的新增和删除。
当用户点击列表中文件时，需要后台转换临时链接进行下载，需要保证文件只有创建者可读，只能通过临时url链接获取，防止盗链。
## 附加条件（可选做）：
可以在专区页面记录并展示每个文件的下载次数，并可以根据下载次数或者更新时间进行排序。
## 本级项目注意点：
在使用文件存储时，注意配置文件权限为仅创建者可读，防止其他人直接转换网址盗用。
## 本级项目考验点：
- web端匿名登录
- web端调用数据库
- 云函数内转换文件临时地址
- 云存储权限管理
## 提交材料：
- 1.可访问的功能展示地址
- 2.功能视频录屏
- 3.代码核心的压缩文件：云函数的代码和web代码文件夹，以及数据库名称结构描述文件。
# 高级实战【后台管理】
## 项目要求：
为中级项目的文件下载区开发web后台管理页面。包含文件列表的基本维护操作
文件的上传，设置文件名，链接保存数据库
文件的重新更新上传，以及文件的更新历史
文件的删除
文件下载数据的后台查看（自行发挥，比如总下载次数，当日下载次数，下载人数）
相应的更改中级实战的web页面，增加文件的更新历史，以及旧文件链接的展示。
web管理的功能设计可以自由发挥。
## 本级项目注意点：
在web管理登录时，需要用到权限验证，不能页面打开即可管理，具体实现可以自行脑洞，最差也可以使用普通密码的形式进行设计验证。
## 本级项目考核点：
- web端上传文件
- web端调用数据库
- web端匿名登录
- 云函数http触发
## 提交材料：
- 1.可访问的功能展示地址
- 2.功能视频录屏
- 3.代码核心的压缩文件：包含实现完整项目的云函数和web端代码，以及数据库名称结构描述文件。