### WSL2 + Ubuntu18LTS



#### P1

Boot 🔒  ~🔓  

USB Boot  ❌



![b12955d7cd8e6c1026e8ee2558d9ce5](https://blog-imghost.oss-cn-shanghai.aliyuncs.com/img/20201124125155.jpg)

![38b82b873bfac88f144a28d5eac0262](https://blog-imghost.oss-cn-shanghai.aliyuncs.com/img/20201124125158.jpg)



#### P2



**PS** 管理员身份运行



**HyperV**

```
 bcdedit /set hypervisorlaunchtype auto
```

```
Enable-WindowsOptionalFeature -Online -FeatureName VirtualMachinePlatform
```



Win+X



![Snipaste_2020-11-24_12-53-58](https://blog-imghost.oss-cn-shanghai.aliyuncs.com/img/20201124125426.png)

**WSL2**

```
wsl -l
```



```
wslconfig /l
```

```
wslconfig /u Ubuntu
```



```
wsl -l -v
```

```
wsl --set-default-version 2
```



#### P3

查看已安装 shell

```
cat /etc/shells
```

**安装 oh my zsh**

![Snipaste_2020-11-24_17-23-24](https://blog-imghost.oss-cn-shanghai.aliyuncs.com/img/20201124172333.png)



```
env|grep -I proxy
```



添加  hosts  ！！！

```
sudo vi /etc/hosts
```



```
vi ~/.zshrc
```

```
source ~/.zshrc
```

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```


