# node-getui
由于个推没有发布node包，个人管理一个node包维护。

# 安装方法
		npm install --save git+https://github.com/msi008/getui.git

# 使用方法（暂时只有一个向单人发推送的方法，后续看需要补充）
		var getui = require("./index").init(HOST, APPID, APPKEY, MASTERSECRET)
		
		getui.pushMessageToSingle(clientId, "内容测试"), "测试通知", 0, null).then(function(data){
			console.log(data)
		}, function(err){
			console.error(err)
		})
		
