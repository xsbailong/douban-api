#### 简要描述

搜索电影



#### 请求描述

`https://api.douban.com/v2/movie/top250`



#### 请求示例

`https://api.douban.com/v2/movie/top250`



#### 返回示例

```json
{
	"count": 20,
	"start": 0,
	"total": 8,
	"subjects": [{
		"rating": {
			"max": 10,
			"average": 8.1,
			"stars": "40",
			"min": 0
		},
		"genres": [
			"动作",
			"科幻",
			"冒险"
		],
		"title": "后天",
		"casts": [{
				"alt": "https://movie.douban.com/celebrity/1002679/",
				"avatars": {
					"small": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p52.webp",
					"large": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p52.webp",
					"medium": "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p52.webp"
				},
				"name": "丹尼斯·奎德",
				"id": "1002679"
			},
			{
				"alt": "https://movie.douban.com/celebrity/1048002/",
				"avatars": {
					"small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p12737.webp",
					"large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p12737.webp",
					"medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p12737.webp"
				},
				"name": "杰克·吉伦哈尔",
				"id": "1048002"
			},
			{
				"alt": "https://movie.douban.com/celebrity/1021998/",
				"avatars": {
					"small": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p629.webp",
					"large": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p629.webp",
					"medium": "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p629.webp"
				},
				"name": "埃米·罗森",
				"id": "1021998"
			}
		],
		"collect_count": 326849,
		"original_title": "The Day After Tomorrow",
		"subtype": "movie",
		"directors": [],
		"year": "2004",
		"images": {},
		"alt": "https://movie.douban.com/subject/1308779/",
		"id": "1308779"
	}]
}
```



#### 返回参数说明

| 名称                   | 说明     |
| ---------------------- | -------- |
| count                  | 一页条数 |
| start                  | 起始位置 |
| total                  | 总条数   |
| subjects(subject 数组) | 电影信息 |
| subject.rating         | 评价     |
| subject.genres         | 流派     |
| subject.title          | 标题     |
| subject.casts          | 演员阵容 |
| subject.directors      | 导演     |
| subject.year           | 发行年份 |
| subject.images         | 封面     |

