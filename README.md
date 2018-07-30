## Supported tags

[`7.0-fpm`, `7.1-fpm` , `7.2-fpm`]

## Reference

A set of PHP 7.0, 7.1 and 7.2 FPM images including Composer, which take their config from environment variables. 

Shipped config is for example only , and should be modified for production needs. The following environment variables are currently supported, with the supplied values listed for reference.

* OUTPUT_BUFFERING - On
* MAX_EXECUTION_TIME - 30
* MAX_INPUT_TIME - 60
* MAX_INPUT_VARS - 2000
* MEMORY_LIMIT - 123M (this differs from upstream)
* POST_MAX_SIZE - 100M
* FILE_UPLOADS - On
* UPLOAD_MAX_FILESIZE - 100M
* MAX_FILE_UPLOADS - 20
* MYSQL_DEFAULT_SOCKET - /run/mysqld/mysqld.sock

## Usage

git clone https://github.com/DavidusEdwardus/php-fpm-docker

cd php-fpm-docker

docker pull rayel/php-fpm-docker:7.2-fpm

### Simple usage  

```
docker run --env-file .env -v /run:/run -v /srv:/srv -p 127.0.0.1:9000:9000 rayel/php-fpm-docker:7.2-fpm
```

The above example launches the 7.2 variant on port 9000, mapping /srv into the container. The php.ini variables from the .env environemnt variables file are populated at run time.

## PHP Modules

* bcmath
* Core
* ctype
* curl
* date
* dom
* exif
* fileinfo
* filter
* ftp
* gd
* gettext
* hash
* iconv
* imagick
* imap
* intl
* json
* libxml
* mbstring
* mysqli
* mysqlnd
* openssl
* pcntl
* pcre
* PDO
* pdo_mysql
* pdo_sqlite
* Phar
* posix
* pspell
* readline
* Reflection
* session
* shmop
* SimpleXML
* soap
* sockets
* sodium
* SPL
* sqlite3
* standard
* sysvmsg
* sysvsem
* sysvshm
* tokenizer
* wddx
* xml
* xmlreader
* xmlrpc
* xmlwriter
* xsl
* Zend OPcache
* zip
* zlib
* zmq

