# job-search

* [繁體中文 README.md(Traditional Chinese README.md)](https://github.com/DysonMa/JobSearch/blob/master/README-zh-TW.md)
* Using SQLite, asyncio, pandas, pyquery, requests to build a crawler and deploy on Heroku with connected to Line ChatBot.

## About

104, 1111 and cakeresume are the most frequently used job search websites in Taiwan.

![104-demo](https://github.com/DysonMa/JobSearch/blob/master/static/images/104.PNG)

![1111-demo](https://github.com/DysonMa/JobSearch/blob/master/static/images/1111.PNG)

![cakeresume-demo](https://github.com/DysonMa/JobSearch/blob/master/static/images/cakeresume.PNG)

Nowadays, job search information are huge and change rapidly. It is always effective and necessary to quickly collect job search information through crawlers. Besides, storing the crawled data into the database can be search at any time.

In this project, different from the previous linear execution method, I use an asynchronous method to crawl the job websites. This application will increase the crawler speed and shorten the waiting time.

### Built With
* python
* SQLite
* asyncio
* Pandas
* pyquery
* requests

## Getting Started
### Installation
Clone the repo
```
git clone https://github.com/DysonMa/JobSearch.git
```
## Usage
1. Define the required parameters. `web` can also choose `104`, `1111` and `cakeresume`. `end_page` means the number of page for crawling.
```
web = '104'
keyword = 'python'
end_page = 3
sqlite_path = './job.db'
```
2. Execute crawling
```
start_crawling()
```
歷經6.618713617324829秒<br>
存檔成功

3. Show DataFrame
```
df
```

![demo](https://github.com/DysonMa/JobSearch/blob/master/static/images/demo.PNG)

## License
Distributed under the MIT License.

## Contact
Dyson Ma - madihsiang@gmail.com
Project Link: https://github.com/DysonMa/JobSearch
