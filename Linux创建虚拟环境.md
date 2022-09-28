# Linux创建虚拟环境

## 安装虚拟环境

```
sudo pip install virtualenv
sudo pip install virtualenvwrapper
```

## 配置虚拟环境

```
# 1、创建目录用来存放虚拟环境
mkdir $HOME/.virtualenvs

# 2、打开~/.bashrc文件
gedit ~/.bashrc
# 并添加如下：
export WORKON_HOME=$HOME/.virtualenvs
source /usr/local/bin/virtualenvwrapper.sh

# 3、重启运行
source ~/.bashrc
```

## 创建虚拟环境

```
mkvirtualenv --python=3.7 hello
# or
mkvirtualenv -p /usr/bin/python3.6 torch1.0
```

## 进入虚拟环境

```
workon [name]
```

## 查看虚拟环境

```
workon [name]
```

## 推出虚拟环境

```
deactivate [name]
```

## 删除虚拟环境

```
rmvirtualenv [name]
```

