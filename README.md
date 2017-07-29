# node-getui
由于个推没有发布node包，个人管理一个node包维护。

# 安装方法
		npm install --save git+https://github.com/msi008/getui.git

# 使用方法（）
		var getui = require("./index").init(HOST, APPID, APPKEY, MASTERSECRET)


- 单点推送		
``` 
	 getui.pushMessageToSingle(clientId, "内容测试"), "测试通知", 0, null).then(function(data){
			console.log(data)
		}, function(err){
			console.error(err)
		})
```
 		

- 按APP推送	
``` 
	  module.exports.pushMessageToApp = function (appId, system, content, alertMessage, badge, sound, TransmissionType) {
             return pushMessageToApp(appId, system, content, alertMessage, badge, sound, TransmissionType)
         }
```


- 获取CID	
``` 
	 module.exports.queryClientId = function (appId, alias) {
             return queryClientId(appId, alias)
         }
```


- 获取别名	
``` 
	 module.exports.queryAlias = function (appId, clientId) {
            return queryAlias(appId, clientId)
        }
```


- 获取在线状态	
``` 
	 module.exports.getClientIdStatus = function (appId, clientId) {
            return getClientIdStatus(appId, clientId)
        }
```

- 获取在线状态	
``` 
	 module.exports.getClientIdStatus = function (appId, clientId) {
            return getClientIdStatus(appId, clientId)
        }
```

- 绑定别名	
``` 
	 module.exports.bindAlias = function (appId, alias, clientId) {
            return bindAlias(appId, alias, clientId)
        }
```

- 解绑别名	
``` 
	 module.exports.unBindAlias = function (appId, alias, clientId) {
            return unBindAlias(appId, alias, clientId)
        }
```

- 获取推送结果信息	
``` 
	 module.exports.getPushResult = function (taskId) {
            return getPushResult(taskId)
        }
```





		
