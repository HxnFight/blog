<!-- MarkdownTOC -->

- [msmtp+mutt 配置说明](#msmtpmutt-配置说明)
  - [msmtp 配置](#msmtp-配置)
  - [补充说明](#补充说明)
  - [和shell脚本一起使用](#和shell脚本一起使用)
  - [ssh,scp 免密操作](#sshscp-免密操作)

<!-- /MarkdownTOC -->

<a name="msmtpmutt-配置说明"></a>
# msmtp+mutt 配置说明
<a name="msmtp-配置"></a>
##  msmtp 配置
* [官网][msmtp]  文件的下载、配置、配置文件样例，都可以在官网上找到。
* [网络教程一][网络教程一]、[网络教程二][网络教程二]
* 按照这两个教程安装即可
 
<a name="补充说明"></a>
## 补充说明
* /usr/local/msmtp/bin/msmtp --version 可以查看你配置文件应防置的地方，所有文件都需要手动创建
* 如果mutt安装的是1.6.6 版本，则测试发附件命令为：mutt -s "test" -a ./a.txt -a ./b.txt -- 11111@qq.com < sayword.txt 在邮箱名前需要添加 --
* mutt 的配置文件需要有 设置  **from** ，教程二中没有显示
* msmtp 的样例文件可以直接 wget http://msmtp.sourceforge.net/doc/msmtprc.txt  下载后取名 msmtprc  即可
* mutt,msmtp 的配置文件都很长，本人建议备份一下，然后将注释部分删除，这样开着清晰明了   

<a name="和shell脚本一起使用"></a>
## 和shell脚本一起使用
* 以后一些自动化脚本就可以通过mutt给自己或者他人发送邮件通知
* 再加上crontab ，可以做很多有意思的事情。。。 

<a name="sshscp-免密操作"></a>
## ssh,scp 免密操作
* [网络教程][网络教程三] 
* [expect使用总结  ][网络教程四]
* [sshpass+ssh+expect非交互密码登陆][网络教程五]
* 我主推 sshpass, 因人而异




[msmtp]: http://msmtp.sourceforge.net/
[网络教程一]: http://blog.csdn.net/gaoxuqiang5/article/details/42638229
[网络教程二]: http://storysky.blog.51cto.com/628458/293005
[网络教程三]: http://blog.csdn.net/nfer_zhuang/article/details/42646849
[网络教程四]: http://blog.chinaunix.net/uid-22570852-id-5745486.html
[网络教程五]: http://blog.chinaunix.net/uid-22570852-id-5086201.html
