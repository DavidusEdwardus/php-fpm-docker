A set of PHP 7.0, 7.1 and 7.2 FPM images including Composer, which take their config from environment variables. Environment variables currently supported :

OUTPUT_BUFFERING
MAX_EXECUTION_TIME
MAX_INPUT_TIME
MAX_INPUT_VARS
MEMORY_LIMIT
POST_MAX_SIZE
FILE_UPLOADS
UPLOAD_MAX_FILESIZE
MAX_FILE_UPLOADS
MYSQL_DEFAULT_SOCKET

Examples of how to run :

git clone https://github.com/DavidusEdwardus/php-fpm-docker

cd php-fpm-docker

docker pull rayel/php-fpm-docker:7.2-fpm

docker run --env-file .env -v /run:/run -v /srv:/srv -p 127.0.0.1:9000:9000 rayel/php-fpm-docker:7.2-fpm

Modules included :

[PHP Modules]
bcmath
Core
ctype
curl
date
dom
exif
fileinfo
filter
ftp
gd
gettext
hash
iconv
imagick
imap
intl
json
libxml
mbstring
mysqli
mysqlnd
openssl
pcntl
pcre
PDO
pdo_mysql
pdo_sqlite
Phar
posix
pspell
readline
Reflection
session
shmop
SimpleXML
soap
sockets
sodium
SPL
sqlite3
standard
sysvmsg
sysvsem
sysvshm
tokenizer
wddx
xml
xmlreader
xmlrpc
xmlwriter
xsl
Zend OPcache
zip
zlib
zmq

