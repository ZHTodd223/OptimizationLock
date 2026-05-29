## 翻译
### [Instrucciones en español aqui](https://github.com/Sqooky/OptimizationLock/blob/main/translations/README_spanish.md)
### [Инструкции на русском тута](https://github.com/Sqooky/OptimizationLock/blob/main/translations/README_russian.md)
### [Instruções em Português aqui](https://github.com/Sqooky/OptimizationLock/blob/main/translations/README_portuguese.md)
### [Инструкции на български тук](https://github.com/Sqooky/OptimizationLock/blob/main/translations/README_bulgarian.md)
### [Istruzioni in italiano qui](https://github.com/Sqooky/OptimizationLock/blob/main/translations/README_italian.md)
### [Instructions en français ici](https://github.com/Sqooky/OptimizationLock/blob/main/translations/README_french.md)
### [中文说明](https://github.com/Sqooky/OptimizationLock/blob/main/translations/README_chinese.md)
## 正文
如需请求支持或为项目贡献发现，我们的Discord服务器可在此处找到[这里](https://discord.gg/EF3Jq57jQv)。  
如果你在游戏中看到我，请打个招呼！我的用户名是"I want to eat flowers!"

### 捐赠
我可能在这个项目上投入了*至少*五百个小时。我希望它永远免费，但我很穷，如果你想以捐赠的方式表示感谢，我有一个kofi链接！https://ko-fi.com/sqooky（我会永远爱你）  

**捐赠者们！**
我非常爱你们所有人
- Soulx
- Boot
- Xeno
- Sonny

<div>
  <img src="https://github.com/Sqooky/OptimizationLock/blob/main/media/joy.png?raw=true" alt="一张图片，上面写着Sqooky's .gi，一个性能配置的拼贴画，旨在优化游戏。"/>
</div>

# 基本说明
要安装性能配置，请将`steamapps/common/deadlock/game/citadel`中的gameinfo.gi替换为从本仓库下载的文件。
**此处有视频教程**可供安装参考[这里](https://youtu.be/TbjLbQVN2kE)

# 表格
以下是本仓库中提供的每个配置的列表。
| 配置文件 | 用途 | 截图 |
| --- | --- | --- |
| [Sqooky's Config/Optimizationlock Default](https://github.com/Sqooky/OptimizationLock/blob/main/Sqooky's%20.gi/gameinfo.gi) | 以性能为导向，同时不使游戏变得难看。我推荐大多数用户使用。 | 截图可在此处查看[这里](https://github.com/Sqooky/OptimizationLock/tree/main/Sqooky's%20.gi) |
| [Test_Cfg](https://github.com/Sqooky/OptimizationLock/blob/main/test_cfg/gameinfo.gi) | Sqooky的配置但为测试分支。可能会导致小问题，但性能应该更好。 | 暂无截图。 |
| [Boot's Max Fps](https://github.com/Sqooky/OptimizationLock/blob/main/boot's%20maxium%20fps%20config/gameinfo.gi) | 高度以性能为导向，目前此配置在所有测试配置中提供最佳fps。 | 截图可在此处查看[这里](https://github.com/Sqooky/OptimizationLock/tree/main/boot's%20maxium%20fps%20config) |
| [Kaizuchaneru's Minimum Spec](https://github.com/Sqooky/OptimizationLock/blob/main/kaizuchaneru's%20minimum%20spec/gameinfo.gi) | 此配置将fps置于一切之上，并大幅降低图形质量。推荐用于配置较差的电脑。 | 截图可在此处查看[这里](https://github.com/Sqooky/OptimizationLock/tree/main/kaizuchaneru's%20minimum%20spec) |
| [Piggy's gameinfo.gi](https://github.com/Sqooky/OptimizationLock/tree/main/piggy's%20config) | 目前piggy的配置已过时，但如果你想使用他的配置，它在这里。 | |
| [Convars.txt](https://github.com/Sqooky/OptimizationLock/blob/main/convars.txt) | 游戏代码中的每一个convar。不是正式配置，而是参考。 | |
| [Base_convars.txt](https://github.com/Sqooky/OptimizationLock/blob/main/base_convars.txt) | 优化锁默认使用的所有convars，如果你想手动添加它们。 | |



要手动添加convars，你需要打开gameinfo.gi，ctrl+f搜索`convars`，然后将命令粘贴在`{`之后。  
手动添加convars时，请确保不要删除`rate {`或将其放入其括号中，否则会导致游戏无法启动。
```
Convars {
//你希望你的convars从这一行开始-


// 并在这一行结束。
rate {
```

# "安装配置后地图变得奇怪且黑暗"
将游戏中的阴影设置降低到中等或低。
# 常见问题
- "如何在配置中找到某个值？"  
在文本编辑器中按ctrl+f，然后输入你想要的字符串。  
- "如何将某个值恢复为默认？"  
将其注释掉。  
- "注释是什么意思？"  
要注释一行，请在行首加上`//`。这将使其不被配置执行。  
- "为什么我的角色在结束画面和商店中的肖像中是暗的？"  
将`lb_enable_dynamic_lights`设置为`true`
- "为什么建筑物会突然出现和消失？"  
将`r_farz`或`r_mapextents`注释掉。  
- "如何更改我的视野？"  
将`citadel_camera_hero_fov`或`r_aspectratio`注释掉或降低其值。  
- "这个补丁的配置坏了"  
每次重大更新都会覆盖gameinfo.gi。你需要手动再次替换它。  
- "我看不到一定距离外的箱子"  
`r_size_cull_threshold "0.7"`
- "我看不到一定距离外的步兵血条"  
更改`r_size_cull_threshold`和`sc_fade_distance_scale_override`的值。
- "看不到门卫的大招指示器"  
将`cl_ragdoll_limit`设置为`"-1"`
- "在某些角度下victor和paige有孔洞"  
注释掉`sc_screen_size_lod_scale_override`或增加其值。
- "罪人的灯光是小三角形"  
注释掉`sc_screen_size_lod_scale_override`或增加其值。  
- "我使用的是boot's/kaiz's配置，在商店或结束画面中看不到英雄"  
将`citadel_portrait_world_renderer_off`注释掉或设置为false  
- "我使用的是boot's/kaiz's配置，看不到lash的地面猛击"  
将`r_drawdecals`注释掉或设置为true  
- "看不到远处的爆炸通风口风"  
将`sc_fade_distance_scale_override`注释掉  

# 模组支持
本仓库中包含的每个配置变体都添加了模组支持。对于那些希望移除或重新添加它的人，请从searchpaths括号中移除`Game citadel/addons`。

# 致谢
虽然我很想说我独自完成了这个项目，但我并没有。这些是应得与我同样多赞扬（如果不是更多）的了不起的人们。  
衷心感谢以下所有人。他们都很可爱。  
- Sqooky:             我是项目的主要开发者和维护者，但如果没有这里的其他人，这个项目不会被维护到这个程度。  
- JasperP:            我的个人英雄。（Valve开发者因我在项目上的工作而联系我。）  
- Boot:               提供了csm cvars，这带来了显著的性能提升。  
- Brullee:            移除了虚假的cvars、冗余命令，添加了cvarlist.md，并重新格式化了配置。  
- Kaizuchaneru:       虽然没有直接参与开发，但他们测试了大多数cvars。  
- Tamara Mochaccina:  贡献了vindicta瞄准镜修复和雾效修复。  
- RoseyLemonz:        移除了重复的cvars

## 捐赠者
非常感谢你们。即使考虑到你们认为我的工作值得任何捐赠，这也是令人难以置信的。我爱你们所有人  
- Boot:   给了我五美元，从根本上就是一个很棒的人和朋友
- Sonny:  给了我五美元，并等待我设置贝宝账户，而且没有改变主意
- Soulx:  给了我五美元，并告诉我关于螺内酯的事情
- Xeno:   非常礼貌地等我弄清楚如何接受捐赠，并且非常礼貌

## 翻译者
- Egyptianscale:                    翻译为俄语
- Tamara Mochaccina and Heathen:    翻译为西班牙语
- Linaa and anartoast:              翻译为葡萄牙语
- Macchiako:                        翻译为保加利亚语
- Cyvoid:                           翻译为意大利语
- Vi:                               翻译为法语

## 杂项
- Artemon121:     制作了Citadel cvar隐藏器，帮助Abdalla获取cvars并在游戏中测试。
- Dacooder:       贡献了一个修复，复制了配置，将其作为自己的分发，当我问他为什么删除了致谢（尽管他之前称我为"项目的大脑"）时，他称我为骚扰者，并制作了两个视频和一份谷歌文档来揭露我。老实说，这让我很开心。
- Kin:            主动进行了大量基准测试。
- Kunet:          为gameinfo语法制作了格式化器！这就是为什么内容有适当的缩进！太棒了。
- Maihdenless:    发起了最初的OptimisationLock及其Discord。
- Piggy:          让我镜像他的配置。

## 因这个项目而认识的酷人们，无论如何我都想感谢他们
- 6Daves
- Achira
- Anartoast
- Boot
- GoreDaughter
- Jaden
- Jasper
- Jb
- Kin
- Krisha
- Masteroms
- PeachCebo
- Tamara Mochaccina
- 还有你，感谢你使用这个项目，让我开心<3。请照顾好自己。

## 为我提供截图的优秀人们 <33333
- Abooo
- Dirtkiller23/Aricole
- Thai
- Boot
- Lina 🜏


# 非常重要的公告
在之前的补丁中，citadel_main_english.txt中有一项更改，指出"当任何队伍成员对Gameinfo.gi中的ConVars进行了更改或正在运行工具模式时，无法进入匹配。"目前，此功能尚未完全实现。
除此之外，Valve将来可能会正确实施此功能，从而限制游戏中的convars使用。在那之前（以及很可能在那之后）我仍将致力于这个项目。  

在此之前，你应该考虑写一篇[论坛帖子](https://forums.playdeadlock.com/)，内容为"嘿，我害怕如果convars被正确禁用，我将无法以约+60fps的速度玩这个游戏"，因为这是向开发者提供反馈的最直接方式。