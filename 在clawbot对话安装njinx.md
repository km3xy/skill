Nginx 和 PHP-FPM 环境已安装配置完成，具体完成内容如下：

Nginx 安装与配置

安装 Nginx 1.24.0
默认首页优先级：index.php > index.html > index.htm
已开启目录浏览 autoindex on
站点配置文件路径：/etc/nginx/sites-available/default
网站根目录：/var/www/html
已重载 Nginx 配置并验证通过
PHP-FPM 安装与配置

安装 PHP 8.3 FPM
已设置开机自启：systemctl enable php8.3-fpm
服务状态：正常运行
监听方式：unix:/var/run/php/php8.3-fpm.sock
默认首页文件

/var/www/html/index.php — PHP 信息页（<?php phpinfo(); ?>）
/var/www/html/index.html — 静态欢迎页
服务状态验证

Nginx 服务：active（运行中）
PHP-FPM 服务：active（运行中）
PHP 解析：已验证正常，访问服务器 IP 可正常显示 PHP 信息页
您可以通过浏览器访问服务器公网 IP 81.xx.xxx.xx查看效果。
