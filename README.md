# fps-lineup-tool

用于 fps 游戏的 lineup 记录和复习。

## 部署

需要准备：
- mongodb
- nodejs 环境

可指定的环境变量，可使用 dotenv 的方式指定：
- MONGODB_URL，连接的后端数据库
- PORT，后端服务监听端口

```shell
npm install
npm run start
```

lineup 访问地址: `http://localhost:${PORT}/home`
英雄地图管理界面:  `http://localhost:${PORT}/manage`

## 使用

### 添加地图，英雄，技能

在英雄地图管理界面进行操作

### 添加 lineup

前端进行如下操作：

- 选择需要添加的`地图`，`英雄`和`技能`
- 点击侧栏的`添加起始点和终点`，在地图上点击两个点，作为 lineup 的投掷点和生效点
- 点击侧栏的`添加图片及描述`，添加描述文字，通过粘贴将剪贴板中复制的图片上传。如果填错可以点击图标删除这一条描述并重新添加。
- 点击提交

### 查看 lineup

前端进行如下操作：

- 选择需要添加的`地图`，`英雄`和`技能`
- 点击地图上的点，进行 lineup 筛选
- 随后点击会进入 lineup 详情界面，包含 lineup 描述。


## todo

- [ ] 自动生成的 api doc
- [ ] 管理页面用于管理英雄地图和技能
