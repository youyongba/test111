# 游戏列表页面

## 游戏列表接口
### 接口地址

> get


- https://api.xxx.com/user/setEditUser

### header

```javascript
{
    "Authorization": "Bearer xxx"
}
```

### 参数

字段 | 类型  | 说明
:--- | :--- | :---
offset | Number | 1,2,3第几页
limit | Number | 一页显示几条

```javascript 
{
    offset: 1,
    limit: 10
}
```

### 响应

字段 | 类型  | 说明
:--- | :--- | :---
name | String | 游戏名称
type | String | stop:停售, start：销售中， down：下架
size | String | 用户头像
status | String | 用户头像

#### 成功
```javascript
{
    "status": true,
    "msg": "成功",
    "data": [{
        "name": "游戏名称",
        "size":"游戏大小",
        "status":"stop"
    }],
    total: 51
}
```
#### 失败
```javascript
{
    "status": false,
    "msg": "少传一个字段",
}
```



