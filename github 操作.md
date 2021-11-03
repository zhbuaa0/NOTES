### github 操作



```
git config --global user.name "zhdeskbook"
git config --global user.email "zhbuaa0@buaa.edu.cn"
```

##### 生成ssh-key

```
ssh-keygen -t rsa -C "zhbuaa0@buaa.edu.cn"
```

##### 验证

```
ssh -T git@github.com
```

##### 出现错误

```
fatal: unable to access 'https://github.com/zhbuaa0/zhbuaa0.github.io.git/': OpenSSL SSL_read: Connection was aborted, errno 10053
```

```
git config --global http.proxy
git config --global --unset http.proxy
```

### HEXO 配置

- node.js 12.14安装

- 添加环境变量

  ```
   C:\Program Files\nodejs
  ```

- clone 框架仓库

  ``` 
  
  ```