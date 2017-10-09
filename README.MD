## EasyEngine Commands

* site
  * create
    * `ee site create example.com --html` # Simple 
    * `ee site create example.com --php` # PHP + No DB 
    * `ee site create example.com --mysql` # PHP + MySQL 
    * `ee site create example.com --letsencrypt` # Encryption 
    * `ee site create example.com --wp` # install wordpress without any page caching
    * `ee site create example.com --w3tc` # install wordpress with w3-total-cache plugin
    * `ee site create example.com --wpsc` # install wordpress with whisp-super-cache plugin
    * `ee site create example.com --wpfc` # install wordpress + nginx fastcgi_cache
    * `ee site create example.com --wpredis` # install wordpress + nginx redis_cache
    * `ee site create example.com --wpsubdir` # install wpmu-subdirectory without any page caching
    * `ee site create example.com --wpsubdom` # install wpmu-subdomain without any page caching
    * `ee site create example.com --user=admin --pass=password --email=admin@example.com`
    * `ee site create example.com --wp --hhvm` # HHVM
    * `ee site edit example.com --pagespeed` # PageSpeed
    * `ee site create example.com --wp --php7` # PHP7 + WP
    * `ee site create example.com --php7` # PHP7 website
    * `ee site create example.com --proxy=host[:port]` # Proxy
  * delete
    * `ee site delete example.com` # all
    * `ee site delete example.com --no-prompt` #without prompt
    * `ee site delete example.com --files` # files only
    * `ee site delete example.com --db` # database only
  * edit
    * `ee site edit example.com` # Open files in default editor
    * `ee site edit example.com --pagespeed` # Edit pagespeed conf
  * list
    * `ee site list`
    * `ee site list --enabled`
    * `ee site list --disabled`
  * info
    * `ee site info example.com`
  * show
    * `ee site show example.com`
  * update
    * `ee site update`
    * `ee site update example.com --password`
    * `ee site update example.com --wp` # Turn into WP site
    * `ee site update example.com --wp --wpfc` # Update cache type
    * `ee site update example.com --wpsubdir` # WP single to multi
    * `ee site update example.com --wp --wpfc`
    * `ee site update example.com --wp --w3tc`
    * `ee site update example.com --wp --wpsc`
    * `ee site update example.com --wpsubdir`
    * `ee site update example.com --wpsubdir --wpfc`
    * `ee site update example.com --wpsubdir --w3tc`
    * `ee site update example.com --wpsubdir --wpsc`
    * `ee site update example.com --wpsubdomain`
    * `ee site update example.com --wpsubdomain --wpfc`
    * `ee site update example.com --wpsubdomain --w3tc`
    * `ee site update example.com --wpsubdomain --wpsc`
  * enable
    * `ee site enable example.com`
  * disable
    * `ee site disable example.com`
  * log
    * `ee site log example.com` # Ctrl^C to exit
* debug
  * `ee debug --all`
  * `ee debug --nginx --rewrite --fpm --php --mysql`
  * `ee debug --php
  * `ee debug --php7`
  * `ee debug --nginx`
  * `ee debug --rewrite`
  * `ee debug --fpm`
  * `ee debug --fpm7`
  * `ee debug --mysql`
  * `ee debug --mysql --import-slow-log-interval=5`
  * `ee debug --all=off`
  * `ee debug example.com --all`
  * `ee debug example.com --wp --nginx --rewrite`
  * `ee debug example.com --wp`
  * `ee debug example.com --nginx`
  * `ee debug example.com --rewrite`
  * `ee debug example.com --wp=off`
  * `ee debug example.com --all=off`
* clean
  * `ee clean`
  * `ee clean --fastcgi`
  * `ee clean --memcache`
  * `ee clean --opcache`
  * `ee clean --pagespeed`
  * `ee clean --redis`
  * `ee clean --all`
* log
  * `ee log show`
  * `ee log show example.com`
  * `ee log show --access`
  * `ee log show example.com --access`
  * `ee log show --fpm`
  * `ee log show --mysql`
  * `ee log show example.com --wp`
  * `ee log reset`
  * `ee log reset example.com`
  * `ee log reset --access`
  * `ee log reset example.com --access`
* stack
  * `ee stack install` # web
  * `ee stack install --web`
  * `ee stack install --nginx`
  * `ee stack install --php`
  * `ee stack install --mysql`
  * `ee stack install --postfix`
  * `ee stack install --wpcli`
  * `ee stack install --adminer`
  * `ee stack install --phpmyadmin`
  * `ee stack install --utils`
  * `ee stack install --mail`
  * `ee stack install --all`
  * `ee stack remove` # WEB
  * `ee stack purge`
  * `ee stack purge --php`
* secure
  * `ee secure --auth [Optional user name] [Optional password]`
  * `ee secure --port [Optional port no]`
  * `ee secure --ip [Optional comma separated IPs]`
* info
  * `ee info --nginx`
  * `ee info --php`
  * `ee info --mysql`
  * `ee info`
* `ee import-slow-log`
* `ee update`
