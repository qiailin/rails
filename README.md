rails
=====

qiailin@localhost:~$ cd workspaces

qiailin@localhost:~/workspaces$ ls

rails
qiailin@localhost:~/workspaces$ cd rails

qiailin@localhost:~/workspaces/rails$ ls
blog
qiailin@localhost:~/workspaces/rails$ cd blog

qiailin@localhost:~/workspaces/rails/blog$ ls

app config.ru  doc	    Gemfile.lock  log	  Rakefile     script  tmp

config	db	   Gemfile  lib		  public  README.rdoc  test    vendor

qiailin@localhost:~/workspaces/rails/blog$ rails server

=> Booting WEBrick

=> Rails 3.2.7 application starting in development on http://0.0.0.0:3000

=> Call with -d to detach

=> Ctrl-C to shutdown server

        SECURITY WARNING: No secret option provided to Rack::Session::Cookie.
        This poses a security threat. It is strongly recommended that you
        provide a secret to prevent exploits that may be possible from crafted
        cookies. This will not be supported in future versions of Rack, and
        future versions will even invalidate your existing user cookies.
        Called from: /home/qiailin/.rvm/gems/ruby-1.9.3-p374/gems/actionpack-3.2.7/lib/action_dispatch/middleware/session/abstract_store.rb:28:in `initialize'.

[2013-01-27 01:53:02] INFO  WEBrick 1.3.1

[2013-01-27 01:53:02] INFO  ruby 1.9.3 (2013-01-15) [i686-linux]

[2013-01-27 01:53:02] INFO  WEBrick::HTTPServer#start: pid=4911 port=3000


Started GET "/assets/rails.png" for 127.0.0.1 at 2013-01-27 01:53:23 +0800

Connecting to database specified by database.yml

Served asset /rails.png - 200 OK (3ms)


Started GET "/rails/info/properties" for 127.0.0.1 at 2013-01-27 01:54:36 +0800

Processing by Rails::InfoController#properties as */*

  Rendered inline template (1.7ms)
  
Completed 200 OK in 8ms (Views: 7.8ms | ActiveRecord: 0.0ms)


Started GET "/rails/info/properties" for 127.0.0.1 at 2013-01-27 01:54:42 +0800

Processing by Rails::InfoController#properties as */*

  Rendered inline template (0.5ms)
  
Completed 200 OK in 2ms (Views: 1.2ms | ActiveRecord: 0.0ms)

[2013-01-27 01:54:42] WARN  Could not determine content-length of response body. Set content-length of the response or set Response#chunked = true


