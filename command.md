### linux command

### 服务器挂起进程
        nohup command > log.file 2>&1 &
- nohup使command命令不受shell退出的影响，忽略所有的挂起信号。
- command是我们要在linux下执行的命令或程序。
- \>log.file将command命令输出的结果重定向到log.file文件中保存。
- 2>&1表示将错误输出重定向到标准输出。由于标准输出已经重定向到了log.file文件，因此如果命令运行时发生错误，则错误提示也会被发送到log.file文件中。

- 最后的&代表此条命令是后台执行的。
  
        bg %n #使其后台继续执行
        fg %n #n为进行pid
如果将后台命令转为前台命令，使用fg %n。n为任务的pid，使用jobs或者ps均可查到。

### pytorch 安装
- 服务器现在最高支持 
-
                conda install pytorch==1.7.1 torchvision==0.8.2 torchaudio==0.7.2 cudatoolkit=9.2 -c pytorch
- 查看安装情况
                
                import torch
                print(torch.__version__)
                print(torch.version.cuda)
                print(torch.cuda.is_available())

- drop
删除表中的某一行或者某一列更明智的方法是使用drop，它不改变原有的df中的数据，而是返回另一个dataframe来存放删除后的数据。

### jupyterbook
- 设置ipynb转化为py
-     jupyter nbconvert --to script baseline.ipynb
- 设置jupyter 服务              
                jupyter notebook --port 8889