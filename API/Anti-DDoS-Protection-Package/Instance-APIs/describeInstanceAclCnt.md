# describeInstanceAclCnt


## 描述
查询已添加的访问控制规则数量

## 请求方式
POST

## 请求地址
https://antipro.jdcloud-api.com/v1/regions/{regionId}/instances/{instanceId}:describeInstanceAclCnt

|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**regionId**|String|True| |地域 Id, DDoS 防护包目前支持华北-北京, 华东-宿迁, 华东-上海|
|**instanceId**|String|True| |防护包实例 Id|

## 请求参数
无


## 返回参数
|名称|类型|描述|
|---|---|---|
|**result**|[Result](describeinstanceaclcnt#result)| |
|**requestId**|String| |
|**error**|[Error](describeinstanceaclcnt#error)| |

### <div id="error">Error</div>
|名称|类型|描述|
|---|---|---|
|**err**|[Err](describeinstanceaclcnt#err)| |
### <div id="err">Err</div>
|名称|类型|描述|
|---|---|---|
|**code**|Long|同http code|
|**details**|Object| |
|**message**|String| |
|**status**|String|具体错误|
### <div id="result">Result</div>
|名称|类型|描述|
|---|---|---|
|**cnt**|Integer|已添加的访问控制规则数量|

## 返回码
|返回码|描述|
|---|---|
|**200**|OK|
