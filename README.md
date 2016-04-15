# notebook

2016/4/15

Windows 中Rails 环境搭建

1.下载安装ruby：http://rubyinstaller.org/downloads/

2.下载安装包（gem）管理工具rubygems：下载，cmd切到解压目录,ruby setup.rb直接运行安装

3.安装和ruby版本对应的devkit：下载地址同ruby安装包的下载地址，下载解压后cmd切到解压目录，执行ruby dk.rb init，在生成的config.yml文件中添加ruby的根目录,接着执行 ruby dk.rb install

4.替换rubyGem库源地址：
去除官网的gem库源地址：gem sources --remove https://rubygems.org/
添加墙内服务器的源地址：gem sources -a https://ruby.taobao.org/  #windows下添加会出现ssl证书验证失败的问题，所以我添加的源地址是ruby-china的地址：gem sources -a http://gems.ruby-china.org/
验证：gem sources -l    查看一下

5.安装rails: gem install rails

