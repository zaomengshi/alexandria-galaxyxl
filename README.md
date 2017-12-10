# alexandria

alexandria is an ebook auto-uploader for various private trackers. It will
fetch metadata for all of your books and upload them if they haven't
been already.

## Installation

Make sure that mktorrent is not lower than 1.1
# git clone https://github.com/Rudde/mktorrent.git
# cd mktorrent
# make
# make install

# apt-get install mktorrent poppler-utils djvulibre-bin calibre
$ pip install -r requirements.txt


## Usage


$ python alexandria /ebooks(存放待上传电子书的地址，需填写完整目录)

第一次运行需要填写配置文件 ~/.alexandria/config

# vim ~/.alexandria/config
##配置文件详述
1.[global]：
	torrent_dir=制作种子的存放目录，和下载软件的watch目录一致（便于自动做种）
	data_dir=下载软件的默认下载地址。
2.[bibliotik]:空着
3.[red]：
	username=red用户名
	password=red密码
4.[ptpimg]:
	key=ptpimg网站key(登录ptpimg首页，F12调试，搜索key)

## 配置上传间隔
# vim alexandria
# /sleep(100)  自己定义等待时间单位秒

##再次运行：
#python alexandria /ebooks(存放待上传电子书的地址，需填写完整目录)
