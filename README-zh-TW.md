# job-search

* [English README.md(英文 README.md)](https://github.com/DysonMa/JobSearch/blob/master/README.md)
* 這是一個用 SQLite, asyncio, pandas, pyquery, requests 來建立的爬蟲程式，並部署至 Heroku 平台上，再串接至 Line ChatBot(聊天機器人).

## 關於

104, 1111 和 cakeresume 是台灣求職最常用的網站

104:
![104-demo](https://github.com/DysonMa/JobSearch/blob/master/static/images/104.PNG)

1111:
![1111-demo](https://github.com/DysonMa/JobSearch/blob/master/static/images/1111.PNG)

cakeresume:
![cakeresume-demo](https://github.com/DysonMa/JobSearch/blob/master/static/images/cakeresume.PNG)

現今，求職的資訊非常龐大且瞬息萬變，利用爬蟲的技術來快速地蒐集求職資訊是有相當有效率的方法。 除此之外，將爬取下來的資料存到資料庫也有利於往後查詢的便利性。

在這個專案裏頭，採用不同於以往單線型(linear execution method)的執行方法，改用**非同步(asynchronous)**的方式來爬取這些網站，增加爬蟲的速度，縮短等待的時間。

### 建立環境與套件
* python
* SQLite
* asyncio
* Pandas
* pyquery
* requests

## 如何開始
### 安裝
遠端下載repo
```
git clone https://github.com/DysonMa/JobSearch.git
```
## 使用
1. 設定需要的參數，`web` 參數可以選擇要 `1111` 、 `104` 或是 `cakeresume`，`end_page` 代表爬蟲的頁數。
```
web = '104'
keyword = 'python'
end_page = 3
sqlite_path = './job.db'
```
2. 執行爬蟲
```
start_crawling()
```
歷經6.618713617324829秒<br>
存檔成功

3. 用DataFrame來觀察
```
df
```

## License
Distributed under the MIT License.

## Contact
Dyson Ma - madihsiang@gmail.com
Project Link: https://github.com/DysonMa/JobSearch
