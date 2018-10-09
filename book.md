#### 简要描述

拉取图书列表和搜索图书列表接口



#### 请求描述

`https://api.douban.com/v2/book/search`



#### 参数

| 参数名 | 必选 | 类型   | 说明         |
| ------ | ---- | ------ | ------------ |
| q      | 是   | string | 查询关键词   |
| start  | 否   | number | 从第几条开始 |
| count  | 否   | number | 一页条数     |



#### 请求示例

`https://api.douban.com/v2/book/search?q=我是传奇&start=1`



#### 返回示例

```json
{
	"count": 10,
	"start": 1,
	"total": 11,
	"books": [{
		"rating": {
			"max": 10,
			"numRaters": 33,
			"average": "7.6",
			"min": 0
		},
		"subtitle": "",
		"author": ["[美] 理查德·马特森"],
		"pubdate": "2013-5",
		"tags": [],
		"origin_title": "I Am Legend",
		"image": "<https://img3.doubanio.com/view/subject/m/public/s26811480.jpg>",
		"binding": "平装",
		"translator": ["陈宗琛"],
		"catalog": "我是传奇\n埋没的天才\n死亡时间\n猎物\n魔女之战\n死亡之舞\n白丝衣\n疯狂之屋\n葬礼\n黯影\n移魂\n导读跨界编剧与作家的传奇人物——理查德·马特森与《我是传奇》 林翰昌",
		"pages": "425",
		"images": {
			"small": "<https://img3.doubanio.com/view/subject/s/public/s26811480.jpg>",
			"large": "<https://img3.doubanio.com/view/subject/l/public/s26811480.jpg>",
			"medium": "<https://img3.doubanio.com/view/subject/m/public/s26811480.jpg>"
		},
		"alt": "<https://book.douban.com/subject/24700313/>",
		"id": "24700313",
		"publisher": "上海译文出版社",
		"isbn10": "7532761274",
		"isbn13": "9787532761272",
		"title": "我是传奇",
		"url": "<https://api.douban.com/v2/book/24700313>",
		"alt_title": "I Am Legend",
		"author_intro": "理查德·马特森（Richard Matheson），1926年出生于美国新泽西，1951年移居加州工作至今。 理查德·马特森是《纽约时报》畅销书作家，在通俗文学领域，他的作品影响了当代的许多知名作家。曾创作经典科幻小说《华氏451》的布拉德伯里，就尊他为20世纪最重要的作家；而恐怖大师斯蒂芬·金更是公开表示：“一般人们谈论恐怖小说，酋先会提到我的名字；但是，如果没仃理查德·马特森，就根本不会有我这号人。他是我的父亲，这就像贝茜·史密斯是猫王的母亲。”理查德·马特森的作品跨越恐怖、科幻、悬疑和奇幻等多个领域，同时，在影观剧写作方面也缔造了许多传奇如大导演斯皮尔伯格的处女作《飞车杀机》上世纪80年代风靡全球的《时光倒流七十年》，以及热播四十载、被欧荚科幻影迷奉为圣经的《星际迷航》，而其代表作《我是传奇》，更是连续三次被好莱坞搬上大银幕。在横跨50年的文坛生涯中，理查德·马特森获奖无数，其中包括世界奇幻文学协会颁发的终身成就奖、恐怖小说家协会颁发的布莱埘‘斯托克终身成就奖、爱伦·坡奖、雨果奖、鹅毛笔奖、美国编剧工会奖……",
		"summary": "“它们”很奇怪，一到白天就躲着不敢出来，它们怕大蒜，它们会被尖木棍杀死，它们怕十字架是出了名的。而且，它们无法抵御吸食人血的渴望。\n\n\n\n白天，他在死寂的城市中寻找食物、供给和幸存者。天一黑，他就把自己反锁家中。\n\n\n\n“滚出来吧，内维尔！”此刻，它们正在屋外穿梭徘徊，窃窃私语。它们在等待·····",
		"price": "37.00元"
	}]
}
```



#### 返回参数说明

| 名称              | 说明     |
| ----------------- | -------- |
| count             | 一页条数 |
| start             | 起始位置 |
| total             | 总条数   |
| books(book 数组)  | 书籍信息 |
| book.rating       | 书籍评价 |
| book.author       | 作者     |
| book.subtitle     | 副标题   |
| book.pubdate      | 发行时间 |
| book.catalog      | 目录     |
| book.pages        | 页数     |
| book.images       | 封面     |
| book.title        | 书名     |
| book.url          | 详情链接 |
| book.author_intro | 作者简介 |
| book.summary      | 内容简介 |
| book.price        | 价钱     |

