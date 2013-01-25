rails
=====

Saving wrappers to '/home/qiailin/.rvm/bin'.

ruby-1.9.3-p374 - #importing default gemsets, this may take time ...

qiailin@localhost:~$ ruby --version

ruby 1.8.7 (2011-06-30 patchlevel 352) [i686-linux]

qiailin@localhost:~$ rvm use --default 1.9.3

Using /home/qiailin/.rvm/gems/ruby-1.9.3-p374

ruby-1.9.3-p374 - #validate archive
ruby-1.9.3-p374 - #extract
ruby-1.9.3-p374 - #validate binary
ruby-1.9.3-p374 - #setup
mkdir: 无法创建目录"": 没有那个文件或目录
mkdir: 无法创建目录"": 没有那个文件或目录
Saving wrappers to '/home/qiailin/.rvm/bin'.
ruby-1.9.3-p374 - #importing default gemsets, this may take time ...
qiailin@localhost:~$ ruby --version
ruby 1.8.7 (2011-06-30 patchlevel 352) [i686-linux]
qiailin@localhost:~$ rvm use --default 1.9.3
Using /home/qiailin/.rvm/gems/ruby-1.9.3-p374
qiailin@localhost:~$ ruby --version
ruby 1.9.3p374 (2013-01-15 revision 38858) [i686-linux]
qiailin@localhost:~$ gem install passenger
Fetching: fastthread-1.0.7.gem (100%)
Building native extensions.  This could take a while...
Fetching: daemon_controller-1.1.1.gem (100%)
Fetching: rack-1.5.0.gem (100%)
Fetching: passenger-3.0.19.gem (100%)
Successfully installed fastthread-1.0.7
Successfully installed daemon_controller-1.1.1
Successfully installed rack-1.5.0
Successfully installed passenger-3.0.19
4 gems installed
Installing ri documentation for fastthread-1.0.7...
Installing ri documentation for daemon_controller-1.1.1...
Installing ri documentation for rack-1.5.0...
Installing ri documentation for passenger-3.0.19...
Installing RDoc documentation for fastthread-1.0.7...
Installing RDoc documentation for daemon_controller-1.1.1...
Installing RDoc documentation for rack-1.5.0...
Installing RDoc documentation for passenger-3.0.19...
qiailin@localhost:~$ rvmsudo passenger-install-nginx-module
Warning: can not check `/etc/sudoers` for `secure_path`, falling back to call via `/usr/bin/env`, this breaks rules from `/etc/sudoers`. export rvmsudo_secure_path=1 to avoid the warning.[sudo] password for qiailin: 
Welcome to the Phusion Passenger Nginx module installer, v3.0.19.

This installer will guide you through the entire installation process. It
shouldn't take more than 5 minutes in total.

Here's what you can expect from the installation process:

 1. This installer will compile and install Nginx with Passenger support.
 2. You'll learn how to configure Passenger in Nginx.
 3. You'll learn how to deploy a Ruby on Rails application.

Don't worry if anything goes wrong. This installer will advise you on how to
solve any problems.

Press Enter to continue, or Ctrl-C to abort.


--------------------------------------------

Checking for required software...

 * GNU C++ compiler... found at /usr/bin/g++
 * The 'make' tool... found at /usr/bin/make
 * A download tool like 'wget' or 'curl'... found at /usr/bin/wget
 * Ruby development headers... found
 * OpenSSL support for Ruby... found
 * RubyGems... found
 * Rake... found at /home/qiailin/.rvm/wrappers/ruby-1.9.3-p374/rake
 * rack... found
 * Curl development headers with SSL support... not found
 * OpenSSL development headers... not found
 * Zlib development headers... not found

Some required software is not installed.
But don't worry, this installer will tell you how to install them.

Press Enter to continue, or Ctrl-C to abort.
^C/home/qiailin/.rvm/gems/ruby-1.9.3-p374/bin/ruby_noexec_wrapper: Interrupt
qiailin@localhost:~$ sudo apt-get install libcurl4-openssl-dev
正在读取软件包列表... 完成
正在分析软件包的依赖关系树       
正在读取状态信息... 完成       
有一些软件包无法被安装。如果您用的是 unstable 发行版，这也许是
因为系统无法达到您要求的状态造成的。该版本中可能会有一些您需要的软件
包尚未被创建或是它们已被从新到(Incoming)目录移出。
下列信息可能会对解决问题有所帮助：

下列软件包有未满足的依赖关系：
 libcurl4-openssl-dev : 依赖: libkrb5-dev 但是它将不会被安装
                        依赖: libldap2-dev 但是它将不会被安装
                        依赖: librtmp-dev 但是它将不会被安装
                        依赖: libssl-dev 但是它将不会被安装
E: 无法修正错误，因为您要求某些软件包保持现状，就是它们破坏了软件包间的依赖关系。
qiailin@localhost:~$ rvmsudo passenger-install-nginx-module
Warning: can not check `/etc/sudoers` for `secure_path`, falling back to call via `/usr/bin/env`, this breaks rules from `/etc/sudoers`. export rvmsudo_secure_path=1 to avoid the warning.Welcome to the Phusion Passenger Nginx module installer, v3.0.19.

This installer will guide you through the entire installation process. It
shouldn't take more than 5 minutes in total.

Here's what you can expect from the installation process:

 1. This installer will compile and install Nginx with Passenger support.
 2. You'll learn how to configure Passenger in Nginx.
 3. You'll learn how to deploy a Ruby on Rails application.

Don't worry if anything goes wrong. This installer will advise you on how to
solve any problems.

Press Enter to continue, or Ctrl-C to abort.


--------------------------------------------

Checking for required software...

 * GNU C++ compiler... found at /usr/bin/g++
 * The 'make' tool... found at /usr/bin/make
 * A download tool like 'wget' or 'curl'... found at /usr/bin/wget
 * Ruby development headers... found
 * OpenSSL support for Ruby... found
 * RubyGems... found
 * Rake... found at /home/qiailin/.rvm/wrappers/ruby-1.9.3-p374/rake
 * rack... found
 * Curl development headers with SSL support... not found
 * OpenSSL development headers... not found
 * Zlib development headers... not found

Some required software is not installed.
But don't worry, this installer will tell you how to install them.

Press Enter to continue, or Ctrl-C to abort.

--------------------------------------------

Installation instructions for required software

 * To install Curl development headers with SSL support:
   Please run apt-get install libcurl4-openssl-dev or libcurl4-gnutls-dev, whichever you prefer.

 * To install OpenSSL development headers:
   Please run apt-get install libssl-dev as root.

 * To install Zlib development headers:
   Please run apt-get install zlib1g-dev as root.

If the aforementioned instructions didn't solve your problem, then please take
a look at the Users Guide:

  /home/qiailin/.rvm/gems/ruby-1.9.3-p374/gems/passenger-3.0.19/doc/Users guide Nginx.html
qiailin@localhost:~$ 

