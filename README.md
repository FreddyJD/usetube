# usetube-improved
Production-ready integrated with the most used scrapper [scrapper-api](https://www.scraperapi.com/?fp_ref=freddyfalso)  so you can scrape YouTube data without any issues of getting blocked. 

[![image info](https://i.imgur.com/ew6uFeQ.png)](https://www.scraperapi.com/?fp_ref=freddyfalso)

# providers
scraperapi = [https://www.scraperapi.com](https://www.scraperapi.com/?fp_ref=freddyfalso)
(SOON) ScrapeBee = [https://www.scrapingbee.com/](https://www.scrapingbee.com/)

# install
```shell
npm install usetube-improved
```

# Working example 
```js
const usetube = require('usetube-improved');

const data = await usetube.searchVideo('hello world', 'api-key-123');

console.log(data);
```

# Usage
```js
// Example
await searchVideo(terms, api_key, token)
await searchVideo('awesome cats', 'cool-api-123')

// Example
await searchChannel(terms, api_key, token)
await searchChannel('FinanceChannel123', 'cool-api-123')

// Example
await getChannelVideos(channel_id, api_key, published_after)
await getChannelVideos('UCkHja3RPRoq3e_YNp1IEyEA', 'cool-api-123', new Date())

// Example
await getPlaylistVideos(playlist_id, api_key)
await getPlaylistVideos('RDQMgEzdN5RuCXE', 'cool-api-123')

// Example
await getChannelDesc(channel_id, api_key)
await getChannelDesc('UCkHja3RPRoq3e_YNp1IEyEA', 'cool-api-123')

// Example
await getVideoDesc(video_id, api_key)
await getVideoDesc('a9xHJjMxQ8', 'cool-api-123')

// Example
await getVideoDate(video_id, api_key)
await getVideoDate('a9xHJjMxQ8', 'cool-api-123')

// Example
await getVideosFromDesc(video_id, api_key)
await getVideosFromDesc('a9xHJjMxQ8', 'cool-api-123')

```