#### 简要描述

拉取音乐列表和搜索音乐列表接口



#### 请求描述

`https://api.douban.com/v2/music/search`



#### 参数

| 参数名 | 必选 | 类型   | 说明         |
| ------ | ---- | ------ | ------------ |
| q      | 是   | string | 查询关键词   |
| start  | 否   | number | 从第几条开始 |
| count  | 否   | number | 一页条数     |



#### 请求示例

`https://api.douban.com/v2/music/search?q=因你而在&start=1`



#### 返回示例

```json
{
	"count": 4,
	"start": 0,
	"total": 4,
	"musics": [{
		"rating": {
			"max": 10,
			"average": "7.5",
			"numRaters": 289,
			"min": 0
		},
		"author": [{
			"name": "林俊傑"
		}],
		"alt_title": "Stories Untold",
		"image": "https://img1.doubanio.com/view/subject/s/public/s25814087.jpg",
		"tags": [],
		"mobile_link": "https://m.douban.com/music/subject/21967671/",
		"attrs": {},
		"title": "因你 而在 (正式版)",
		"alt": "https://music.douban.com/subject/21967671/",
		"id": "21967671"
	}]
}
```



#### 返回参数说明

| 名称               | 说明     |
| ------------------ | -------- |
| count              | 一页条数 |
| start              | 起始位置 |
| total              | 总条数   |
| musics(music 数组) | 音乐信息 |
| music.rating       | 书籍评价 |
| music.author       | 作者     |
| music.image        | 封面     |
| music.title        | 歌名     |
| music.mobile_link  | 歌曲链接 |

