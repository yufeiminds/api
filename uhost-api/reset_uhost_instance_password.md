#重置主机密码-ResetUHostInstancePassword

重置UHost实例的管理员密码。
```
该操作需要UHost实例处于关闭状态。
```

#Request Parameters
|Parameter name|Type|Description|Required|
|Region|string|地域，参见 [地域和可用区列表](../summary/regionlist.html)|**Yes**|
|Zone|string|可用区，参见 [可用区列表](../summary/regionlist.html)|No|
|UHostId|string|UHost实例ID|**Yes**|
|Password|string|UHost新密码（密码格式使用BASE64编码）|**Yes**|
|ProjectId|string|项目编号（子帐号用） 请参考GetProjectList接口|No|


#Response Elements
|Parameter name|Type|Description|Required|
|RetCode|int|操作返回码|**Yes**|
|Action|string|操作名称|**Yes**|
|UhostId|string|UHost实例ID|No|

#Request Example
```
http(s)://api.ucloud.cn/?Action=ResetUHostInstancePassword
&Region=cn-bj2
&Zone=cn-bj2-04
&UHostId=uhost-qs20fr
&Password=UCloud123
```
#Response Example
```
{
    "Action": "ResetUHostInstancePasswordResponse",
    "UHostId": "uhost-qs20fr",
    "RetCode": 0
}
```

{{indexmenu_n>1000}}