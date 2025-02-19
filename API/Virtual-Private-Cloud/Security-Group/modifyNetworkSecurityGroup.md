# modifyNetworkSecurityGroup


## 描述
修改安全组属性

## 请求方式
PATCH

## 请求地址
https://vpc.jdcloud-api.com/v1/regions/{regionId}/networkSecurityGroups/{networkSecurityGroupId}

|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**regionId**|String|True| |Region ID|
|**networkSecurityGroupId**|String|True| |NetworkSecurityGroup ID|

## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**networkSecurityGroupName**|String|False| |安全组的名字。名称取值范围：1-32个中文、英文大小写的字母、数字和下划线分隔符|
|**description**|String|False| |安全组的描述，取值范围：0-256个UTF-8编码下的全部字符|


## 返回参数
|名称|类型|描述|
|---|---|---|
|**requestId**|String|请求ID|


## 返回码
|返回码|描述|
|---|---|
|**200**|OK|
|**400**|Request parameter x.y.z is 'xxx', expected one of [yyy,zzz]|
|**404**|Resource not found|

## 请求示例
调用方法、签名算法及公共请求参数请参考[京东云OpenAPI公共说明](https://docs.jdcloud.com/common-declaration/api/introduction)。
- 请求示例: 修改安全组 sg-yjdd312xqk 的属性

PATCH
```
/v1/regions/cn-north-1/networkSecurityGroups/sg-yjdd312xqk
{
    "networkSecurityGroupName":"自定义安全组Rename",
    "description":"安全组测试"
}

```

## 返回示例
```
{
    "requestId": "c45q1wph2rvj0kj68ccfdc24ia8osgo7"
}
```
