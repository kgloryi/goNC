使用介绍如下:

nc_server
nc_server.exe --help //查看工具使用帮助
nc_server.exe -file/comm "file" -ip "127.0.0.1" -port "5443" -filePath "cmd.exe" -download/execute "execute" //windows 命令执行
nc_server.exe -file/comm "file" -ip "127.0.0.1" -port "5443" -filePath "/bin/sh" -download/execute "execute" //linux命令执行
nc_server.exe -file/comm "file" -ip "127.0.0.1" -port "5443" -filePath "C:/Users/17529/Desktop/test.txt" -download/execute "download" //文件下载
nc_server.exe -file/comm "comm" -ip "127.0.0.1" -port "5443" //通信功能

nc_client
nc_client.exe --help //查看工具使用帮助
nc_client.exe -ip "127.0.0.1" -port "5443" exec/conn/down "conn" //和nc_server端通信
nc_client.exe -ip "127.0.0.1" -port "5443" exec/conn/down "exec" //远程在nc_server端命令执行
nc_client.exe -ip "127.0.0.1" -port "5443" -exec/conn/down "down" -SavefilePath "./test.txt" //远程下载nc_server端服务器上的文件
