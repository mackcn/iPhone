;毒奶博主
; limbopro.xyz
; 04.10.2020   

[一般]
geo_location_checker = http：//ip-api.com/json/？lang = zh-CN，https://raw.githubusercontent.com/limbopro/QuantumultX/master/Scripts/IP_API.js

[DNS]
服务器= 223.5.5.5
服务器= 114.114.114.114
服务器= 119.29.29.29
服务器= 8.8.8.8


[政策]
available =♻️故障切换，无用中断1，无用中断2，img-url = https：//raw.githubusercontent.com/limbopro/Zure/master/IconSet/Available.png
static =✈️机场专线，🎥其他国外流媒体，PROXY，♻️故障切换，DIRECT，img-url = https：//raw.githubusercontent.com/limbopro/Zure/master/IconSet/rocket.png
static =🐟Final，🎥其他国外流媒体，PROXY，♻️故障切换，DIRECT，🛑广告拦截，img-url = https：//raw.githubusercontent.com/limbopro/Zure/master/IconSet/China-map.png
static =📲社交媒体，🎥其他国外流媒体，PROXY，♻️故障切换，img-url = https：//raw.githubusercontent.com/Koolson/Qure/master/IconSet/Twitter.png
static =🍎苹果服务，DIRECT，🎥其他国外流媒体，PROXY，♻️故障切换，img-url = https：//raw.githubusercontent.com/Koolson/Qure/master/IconSet/Apple.png
static =🛑广告拦截，拒绝，代理，直接，img-url = https：//raw.githubusercontent.com/limbopro/Qure/master/IconSet/Advertising.png
static =🎥Netflix，🎥其他国外流媒体，PROXY，img-url = https：//raw.githubusercontent.com/limbopro/Zure/master/IconSet/Netflix_Letter.png
static =🎥其他国外流媒体，PROXY，♻️故障切换，img-url = https：//raw.githubusercontent.com/limbopro/Qure/master/IconSet/GlobalMedia.png

[server_remote]
https://raw.githubusercontent.com/limbopro/Profiles/master/limbopro/Gift/unlesssub.txt，标记=无用例程（❌请不要动它），enabled = true
＃无用订阅（请勿删除）

[filter_remote]
https://raw.githubusercontent.com/NobyDa/Script/master/QuantumultX/AdRule.list，标记=野比去广告（稳定版），force-policy =🛑广告拦截，enabled = true
https://raw.githubusercontent.com/NobyDa/Script/master/QuantumultX/AdRuleTest.list，标记=野比去广告（测试版），force-policy =🛑广告拦截，enabled = false
https://raw.githubusercontent.com/limbopro/Profiles/master/limbopro/QuantumultX.list，标签=机场专线，force-policy =✈️机场专线，enabled = true
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Global.list，标记=社交媒体，force-policy =📲社交媒体，enabled = true
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Apple.list，tag=苹果服务，force-policy =🍎苹果服务，enabled = true
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Media/Netflix.list，tag = Netflix，force-policy =🎥Netflix，enabled = true
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/GlobalMedia.list，tag =其他国外流媒体，force-policy =🎥其他国外流媒体，enabled = true

[rewrite_remote]
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Rewrite.conf，tag=花姐，enabled = true
https://raw.githubusercontent.com/limbopro/Profiles/master/limbopro/Gift/Without/unzip/Js.conf，tag=NoByDa（unzip适合版），enabled = true
https://raw.githubusercontent.com/NobyDa/Script/master/QuantumultX/Rewrite_lhie1.conf，标记= Line1（重写写广告），启用= true
https://raw.githubusercontent.com/NobyDa/Script/master/QuantumultX/Js.conf，tag=NobyDa（远程配置文件和替换），enabled = false
＃考虑到Quantumult X关闭远程JS，野比完整的远程脚本配置文件在Quantumutx.v.1.3版本后替换位置；

[server_local]

[filter_local]
geoip，cn，直接
ip-cidr，10.0.0.0 / 8，直接
ip-cidr，127.0.0.0 / 8，直接
ip-cidr，172.16.0.0 / 12，直接
ip-cidr，192.168.0.0 / 16，直接
ip-cidr，224.0.0.0 / 24，直接
决赛，🐟决赛


[rewrite_local]

＃美区tiktok（v14.7.0）解锁

（。* video_id = \ w {32}）（。* watermark =）（。*）网址302 $ 1
（？<=（（carrier | sys）_region =）CN网址307 US
（？<= version_code =）\ d {1，}。\ d {1} \。\ d {1}网址307 14.0.0

＃Appstore港区下载的tiktok（v8.4.0）解锁                              
＃若需解锁​​Appstore港区下载⏬的tiktok把上面的规则的14.0.0改为8.4.0即可
＃其中US为国别代码，可以看美国🇺🇸用户上传⏫的视频
＃你可以按需将其修改为🇯🇵JP，🇰🇷KR

############################
##引用NobyDa本地脚本开始##
##########################

＃去微博应用内广告（由yichahucha）
^ https？：// m？api \ .weibo \ .c（n | om）/ 2 /（状态/（未读|扩展|正/得到|（朋友|视频）（/ | _）时间轴）|故事/ （video_stream | home_list）|（groups | fangle）/ timeline | profile / statuses |评论/ build_comments |照片/推荐列表|服务/ picfeed | searchall | cardlist |页面| \！/ photos / pic_recommend_status）url脚本-响应-正文QuantumultX /File/wb_ad.js
＃^ https？：//（（sdk | wb）app \ .uve \ .weibo \ .com（/interface/sdk/sdkad.php|/wbapplua/wbpullad.lua）url脚本-响应体QuantumultX / File / wb_launch .js

############################
##引用NobyDa本地脚本结束##
##########################

##其他更多本地脚本配置已经在Js.conf实现
##查看[重写]-[引用]-[NoByDa（毒奶unzip适配版）]
## https://raw.githubusercontent.com/limbopro/Profiles/master/limbopro/Gift/Without/unzip/Js.conf
##未来如果有新的解锁🔓立即更新重写Js.conf即可
##不再需要重新生成并认证证书📄

[mitm]
