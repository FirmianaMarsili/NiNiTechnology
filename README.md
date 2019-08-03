# NiNiTechnology  
ff14时间轴和触发器  
时间轴使用ACT.Timeline和FZTimeline插件。  
触发器使用Triggernometry插件。  
温馨提示：  
插件经过测试的环境：  
国服整合版ACT + FFXIV_ACT_Plugin1.7.2.4 + 国服客户端 √  
国际服纯净版ACT + FFXIV_ACT_Plugin2.0.2.9 + 英文客户端 √  
本插件不给玩家进行标点。不播报热风点名玩家，请结合其它TTS插件使用。  
本插件不播报 死亡宣告点名，凶鸟台词，旋风。请整合其它TTS插件使用。  
如果插件不正常工作，请检查FFXIV_Plugin是否启动，能否读出数据，插件日志中的小队列表与游戏中是否一致，然后重启本插件。  
播报规则：  
=============《伊甸》========================  
12层：蓝标点名播报职业。  
=============《欧米茄幻境9-12层》============  
11层：  
●6人踩塔：按顺序报出3组踩塔人员的职业，如：战骑，龙召，忍机  
●3-4人易伤光束炮：按顺序播报出所有被点名人员的名字。  
12层：  
●易伤死刑：播报被点名人员的职业，如“战”。  
●转向浮游炮：以场地12点为基准，播放上下左右。如“左下左下”，那么请往左下安全区域移动。  
●全存档：以boss面向为基准，播放“左左左”或“右右右”。注意，插件先播报，boss后转向，请等待boss转向后再进行移动。  
●冰火雷分摊+分散：播报分散人员的职业。被点名的职业请按团队散位安排远离中央。  
=============《究极神兵绝境战》==============  
●场地标点方式：  
　　Ａ  
  
Ｄ　　　Ｂ  
  
　　Ｃ  
  
●一杆进洞：	以泰坦为12点。报安全点位置。如果是左边安全，就报“左左左”，右边安全，就报“右右右”。  
●石牢顺位：	连续播报从前到后3个人的职业。如“战忍学”。顺位按如下规则：  
		前←MT ST D1 D2 D3 D4 H2 H1 →后  
		其中 MT←暗战骑→ST    H2←学星白→H1  D1←龙武侍忍诗机赤召黑→D4  
●泰坦落地点预告：警告，由于读取内存方式的不成熟，目前只能在落地前2秒判断出位置，无法作为提前移动的依据，请自己看清泰坦的转向。插件的播报方式：“AAAA，BBBB，CCCC，DDDD”。如果插件错误，会报“自己看”。  
●追击安全点：	播报格式：A点偏B，A点偏B，（原地危险，疾跑穿十字火。）  
		追击的安全点有8个，都在8个连续小字图案的中心，也就是第4个字的位置。如插件报A点偏B，请先向A点移动，然后向B方向寻找8个连续小字，并站在第四个字的位置。如果插件报“原地危险”，则起始位置并非最终安全点，需要在火神冲结束后迅速移动到同侧的另外8个小字安全点区域。  
		如果团队采用减伤盾硬吃火神冲的方式，可直接向第二安全点移动。此时的移动位置请独立判断。  
=============《巴哈姆特绝境战》================  
●雷左右：左←THD→右  
●拘束器：1人无提示，2人，3人无序报职业。  
●龙神的加护读条时：按顺序播报俯冲三个标点的位置。如”2点，6点，10点"。  
●俯冲点名：报职业。报方位（可选）  
●进军3振翅：报除了奶妈以外，被振翅点名的职业。  
●连击4振翅：将根据玩家位置分配最优站位，第一次在场地12点散开，从左到右播报。第二次在场地6点散开，从左到右播报。  
●连击拘束器：按如下形式，其中H1，D1和MT为1号补位，H2，D2和ST为2号补位，D3和D4为自由人。  
站位中D1D2为近战职业，按D1←龙武侍忍→D2的顺序分配，D3D4为远程职业，按D3←诗机赤召黑→D4的顺序分配。  
H1H2为奶妈职业，按H1←白占学→H2的顺序分配。MT，ST为T职业，按MT←暗战骑→ST的顺序分配。  
基本规则：1号被点，2号补位。2号被点，1号补位，1,2全点，自由人补位。  
　　　　　Ａ  
　　　　　H1  
　　　D3　○　H2  
　　　　　↑  
Ｄ　D2　 奶圈 　D4　Ｂ  
 D圈→○　　　○←T圈  
　　　D1　　　MT  
　　　　　ST  
　　　　　Ｃ  
●群龙：面向巴哈，按语音提示行动。  
1.巴哈位置，如“巴哈5点”，请将视角转到5点。  
2.行动位置，如“左下左下”，表示面向巴哈，朝左下移动为安全区。  
3.凶鸟情况，“凶鸟在前”，表示马拉松前方有凶鸟。“凶鸟在后”表示后方有凶鸟。  
4.马拉松方向，“顺时针”或“逆时针”  
5.小龙情况，如提示“前方有龙”，表示走到巴哈位置需要暂停等待第一条龙俯冲过后再走。  
6.双塔引导，会报双塔点名职业和双塔位置，请及时去引导双塔俯冲。  
注意：如果群龙发生减员，则无法预测双塔点名职业。它将是随机点名，请所有人尽可能去场边引导。  
●群龙4塔：以双塔脚下为顺时针1塔，报各职业踩塔顺位。顺位为"近战&gt;远程&gt;奶妈&gt;T"  
例如1龙2召3学4暗，表示顺时针1塔由龙骑踩，以此类推。  
双塔俯冲不踩塔，如果俯冲无分摊标，则由点名分摊的T和奶负责补位踩顺4位的塔。此时会报”T奶补位“  
●黄金巴哈：以12点为正北方向播报Exaflare的出现位置。  
