# Using ngx_lua in UPYUN

* 2014.11 @ Beijing OSC: `Using ngx_lua in UPYUN` ( [slideshare](http://www.slideshare.net/timebug/using-ngxlua-in-upyun) | [speakerdeck](https://speakerdeck.com/timebug/using-ngx-lua-in-upyun) )
* 2015.11 @ Beijing OpenResty Con: `Using ngx_lua in UPYUN 2` ( [slideshare](http://www.slideshare.net/timebug/using-ngxlua-in-upyun-2) | [speakerdeck](https://speakerdeck.com/timebug/using-ngx-lua-in-upyun-2) )
* blog: <http://io.upyun.com/2015/04/14/using-ngxlua-in-upyun/>

## Run the Code

1) Building and Installing [Openresty](http://openresty.org/)

```
tar xzvf ngx_openresty-VERSION.tar.gz
cd ngx_openresty-VERSION/
./configure
make
make install
```

2) Start the Nginx Server

```
cd work
mkdir logs

export PATH=/usr/local/openresty/nginx/sbin:$PATH
nginx -p `pwd`/ -c conf/nginx.conf
```

3) Hello World

```
curl http://localhost:8080/hello
```

## See Also

* <http://www.aosabook.org/en/nginx.html>
* <https://github.com/openresty/echo-nginx-module>
* <http://nginx.org/en/docs/http/ngx_http_rewrite_module.html>
* <https://github.com/timebug/base64-nginx-module>
* <http://agentzh.blogspot.jp/2011/03/how-nginx-location-if-works.html>
* <https://github.com/openresty/lua-nginx-module>
* <https://github.com/openresty/lua-resty-string/pull/7>
* <https://github.com/cloudflare/lua-resty-shcache>
* <https://github.com/openresty/lua-resty-lrucache>
* <https://github.com/openresty/lua-upstream-nginx-module>
* <https://github.com/upyun/lua-resty-checkups>
