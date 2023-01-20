# the-offline-ops
A **[MCDReforged](https://github.com/Fallen-Breath/MCDReforged) plugin**<br>
More plugins click *[here](https://github.com/MCDReforged/PluginCatalogue)*

## Description
Provides a method to protect admin and normal player's account in game server, which <font color=orange>'online-mode' is 'false'</font><br>
为<font color=orange>未开启在线模式（正版验证）</font>的服务器提供了管理员和普通玩家账号保护的一种方法<br>
## How the plugin work
这个插件会在玩家进入服务器时检查玩家的IP地址，如果与记录不符，则将玩家踢出并全服广播<br>
![image](image.png)

如果你不喜欢去摆弄一些让人看不懂的配置文件，并且觉得检测玩家的IP就足够的话，可以试试这个插件<br>
通过`!!offlineops`查看配置命令。无需动手改config文件<br>
即插即用<br>

但是如果你对安全性有较高的需求的话，可以去[插件仓库](https://github.com/MCDReforged/PluginCatalogue/blob/master/readme_cn.md)寻找安全性更高的插件
## Commands
**所有命令都需要MCDR 2级权限**<br>

`!!offlineops`:查看命令列表<br>
`!!offlineops` `notOpsPlayerProtect`| `nopp`:非管理员玩家保护开关<br>
`!!offlineops` `protectPlayer`| `pp`:添加受保护的玩家<br>
`!!offlineops` `allPlayerProtect`| `app`:全体玩家保护开关<br>
`!!offlineops` `delIP`:清除对应或全部玩家的IP记录<br>
## Config
``` json
{
    "notOpsPlayerProtect": true,    //nomal player protect普通玩家保护
    "allPlayerProtect": false,      //all players protect所有玩家保护
    "protectivePlayer": {           //
        "example": "127.0.0.1"
    }
}
```
## Details