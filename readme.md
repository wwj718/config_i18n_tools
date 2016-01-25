#config_i18n_tools
##Install
pip install git+https://github.com/edx/i18n-tools.git

git clone https://github.com/wwj718/config_i18n_tools

cd config_i18n_tools

i18n_tool validate --config=./config


如果在mac下执行可能会报错，需要安装gettext

```bash
brew install gettext  
brew link gettext --force
```

---

#使用msgfmt
通过阅读源码我们发现其实真正用于检测po文件语法的命令是 `msgfmt -c FILE`


##Install
###Ubuntu
无需安装

###Windows
<https://blog.longwin.com.tw/2010/08/windows-gettext-2010/>

###Mac

```bash
brew install gettext  
brew link gettext --force
```

##使用
`msgfmt -c django.po` ，这种方式很干净清晰
