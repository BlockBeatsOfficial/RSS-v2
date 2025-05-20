#  BlockBeats_RSS-v2
Accessing Web3 information via RSS is now more convenient — we’ve added dedicated RSS links for articles and newsflashes, along with a combined feed for all content.

All content: https://api.theblockbeats.news/v2/rss/all

Newsflashes only: https://api.theblockbeats.news/v2/rss/newsflash

Articles only: https://api.theblockbeats.news/v2/rss/article

Makes it easier for you to stay updated with Web3 developments via BlockBeats RSS subscriptions.

📚 BlockBeats RSS Introduction
BlockBeats RSS is an XML-based feed format that provides both real-time newsflashes and in-depth articles. It's designed to help you stay informed about the latest in Web3, blockchain, and crypto directly from theblockbeats.info.

Once subscribed through your preferred RSS reader, the feed automatically delivers new content — including the title, summary, publication date, and link — for quick browsing and reading.

#### Header

```
"language":cn //language cn,en,cht
```


## Response format

The RSS interface returns an XML document containing the following elements:

- `<channel>`: RSS channel information .
  - `<title>`: channel title .
  - `<link>`: channel URL .
  - `<description>`: channel description .
  - `<item>`: Contains information about an article . A `<channel>` can contain multiple `< items >`.
    - `<title>`: title。
    - `<description>`: description .
    - `<link>`:  URL .
    - `<pubDate>`: Publication date of article .
    - `<guid>`: guid .

## Use example

Visit the following URL to get the RSS data:

https://api.theblockbeats.news/v1/open-api/home-xml

Example response：

```xml
<rss xmlns:atom="http://www.w3.org/2005/Atom" version="2.0">
  <script/>
  <channel>
    <title>BlockBeats</title>
    <description>BlockBeats</description>
    <link>https://www.theblockbeats.info</link>
    <image>
        <url>https://image.theblockbeats.info/logo_v2.png</url>
        <title>BlockBeats</title>
        <link>https://www.theblockbeats.info</link>
    </image>
    <item>
        <title>数据：巨鲸地址将超1.9万枚ETH转入Coinbase，约3500万美元</title>
        <description><![CDATA[ BlockBeats 消息，5 月 11 日，据 Etherscan 数据显示，「0xC159」开头匿名地址 6 分钟前将 19,093 枚 ETH 转入链上标记为「Coinbase 10」的地址，约合 3500 万美元。 ]]></description>
        <author>contact@theblockbeats.org (律动BlockBeats)</author>
        <link>https://m.theblockbeats.info/flash/137547</link>
        <pubDate>Thu, 11 May 2023 15:02:29 +0800</pubDate>
        <guid>https://m.theblockbeats.info/flash/137547</guid>
    </item>
  </channel>
</rss>

