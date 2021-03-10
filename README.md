## About

104, 1111 and cakeresume are the most frequently used job search websites in Taiwan.

Nowadays, job search information are huge and change rapidly. It is always effective and necessary to quickly collect job search information through crawlers. Besides, storing the crawled data into the database can be search at any time.

In this project, different from the previous linear execution method, I use an asynchronous method to crawl the job websites. This application will increase the crawler speed and shorten the waiting time.

### Built With
* python
* SQLite
* asyncio
* Pandas

## Getting Started
### Installation
Clone the repo
```
git clone https://github.com/DysonMa/JobSearch.git
```
## Usage
1. Define the required parameters. `web` can also choose `1111` and `cakeresume`. `end_page` means the number of page for crawling.
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

## License
Distributed under the MIT License.

## Contact
Dyson Ma - madihsiang@gmail.com
Project Link: https://github.com/DysonMa/JobSearch
