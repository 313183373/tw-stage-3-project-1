# tw-stage-3-project-1
思沃学院第三阶段大作业

## 需求
- 用React重构[TODO LIST](https://github.com/LiuKaixinHappy/tw-stage-2-project-1)的前端

## 要求
- 新建一个仓库，用react新建一个前端工程，完成TODO LIST的全部逻辑，UI可以自定义，学有余力的同学可以尝试使用[Material-UI](https://material-ui.com/getting-started/installation/)
- 服务器端和数据库逻辑已写好，克隆本项目，启动服务器即可测试，接口如下：

||添加todo|
|--|--|
|url|http://127.0.0.1:8080/todo |
|method|POST|
|request|{id:xx, content:xx, status:xx(0或1，0代表未完成，1代表完成)} 例：{id:1, content:'学习react', status:0}|
|response|成功：{'result': SUCCESS, 'message': '添加成功'}失败：{'result': ERROR, 'message': '添加失败'}|

||修改todo|
|--|--|
|url|http://127.0.0.1:8080/todo |
|method|PUT|
|request|{id:xx, status:xx}例：{id:1, status:1}|
|response|成功：{'result': SUCCESS, 'message': '修改成功'}失败：{'result': ERROR, 'message': '修改失败'}|

||获取todo|
|--|--|
|url|http://127.0.0.1:8080/todo |
|method|GET|
|response|成功：{'result': SUCCESS, 'message': [{id:xx， content:xx， status:xx(0或1，0代表未完成，1代表完成)}]} 失败：{'result': ERROR, 'message': '修改失败'}|

||删除todo|
|--|--|
|url|http://127.0.0.1:8080/todo |
|method|DELETE|
|request|删除项的id数组，如{[1, 2, 3, ...]}|
|response|成功：{'result': SUCCESS, 'message': '删除成功'} 失败：{'result': ERROR, 'message': '删除失败'}|
