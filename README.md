# Bug修復
```
 [Server thread/WARN]: [FluffyMachines] Task #604711086 for FluffyMachines vBuild 40 (git 7583dd9) generated an exception
java.lang.IllegalArgumentException: missing required data class java.lang.Float
	at com.google.common.base.Preconditions.checkArgument(Preconditions.java:217) ~[guava-33.5.0-jre.jar:?]
	at org.bukkit.craftbukkit.CraftParticle.createParticleParam(CraftParticle.java:70) ~[paper-1.21.11.jar:1.21.11-131-6d5b910]
	at org.bukkit.craftbukkit.entity.CraftPlayer.spawnParticle(CraftPlayer.java:2675) ~[paper-1.21.11.jar:1.21.11-131-6d5b910]
	at org.bukkit.entity.Player.spawnParticle(Player.java:3285) ~[paper-api-1.21.11-R0.1-SNAPSHOT.jar:?]
	at org.bukkit.entity.Player.spawnParticle(Player.java:3199) ~[paper-api-1.21.11-R0.1-SNAPSHOT.jar:?]
	at org.bukkit.entity.Player.spawnParticle(Player.java:3121) ~[paper-api-1.21.11-R0.1-SNAPSHOT.jar:?]
	at org.bukkit.entity.Player.spawnParticle(Player.java:3089) ~[paper-api-1.21.11-R0.1-SNAPSHOT.jar:?]
	at org.bukkit.entity.Player.spawnParticle(Player.java:3075) ~[paper-api-1.21.11-R0.1-SNAPSHOT.jar:?]
	at FluffyMachines-Build 40 (git 7583dd9).jar//io.ncbpfluffybear.fluffymachines.utils.Events.lambda$onPlayerWarp$0(Events.java:164) ~[?:?]
	at org.bukkit.craftbukkit.scheduler.CraftTask.run(CraftTask.java:78) ~[paper-1.21.11.jar:1.21.11-131-6d5b910]
	at org.bukkit.craftbukkit.scheduler.CraftScheduler.mainThreadHeartbeat(CraftScheduler.java:474) ~[paper-1.21.11.jar:1.21.11-131-6d5b910]
	at net.minecraft.server.MinecraftServer.tickChildren(MinecraftServer.java:1756) ~[paper-1.21.11.jar:1.21.11-131-6d5b910]
	at net.minecraft.server.MinecraftServer.tickServer(MinecraftServer.java:1611) ~[paper-1.21.11.jar:1.21.11-131-6d5b910]
	at net.minecraft.server.dedicated.DedicatedServer.tickServer(DedicatedServer.java:427) ~[paper-1.21.11.jar:1.21.11-131-6d5b910]
	at net.minecraft.server.MinecraftServer.processPacketsAndTick(MinecraftServer.java:1667) ~[paper-1.21.11.jar:1.21.11-131-6d5b910]
	at net.minecraft.server.MinecraftServer.runServer(MinecraftServer.java:1335) ~[paper-1.21.11.jar:1.21.11-131-6d5b910]
	at net.minecraft.server.MinecraftServer.lambda$spin$2(MinecraftServer.java:388) ~[paper-1.21.11.jar:1.21.11-131-6d5b910]
	at java.base/java.lang.Thread.run(Unknown Source) ~[?:?]
```
問題出現在傳送裝置的粒子上，我只是把產生粒子的代碼刪除掉了

---
# FluffyMachines 蓬松机器

这些是我随手做的一些机器。我添加了我能想得到的，或是别的附属不想添加的东西。

可以在 `plugins/Slimefun/Items.yml` 内调整设置。

<!-- 魔改内容:
- 手摇发电机可启用频率限制(如果使用汉化版构建#4及以前的版本，请注意更新配置文件，建议删除旧配置文件) -->

## 下载

点击这里下载 FluffyMachines: [下载 FluffyMachines](https://builds.guizhanss.net/baoad/FluffyMachines/master)

<p align="center">
  <a href="https://github.com/baoad/FluffyMachines/actions/workflows/maven.yml">
    <img src="https://github.com/baoad/FluffyMachines/actions/workflows/maven.yml/badge.svg" alt="Java CI"/>
  </a>

  <a href="https://builds.guizhanss.net/baoad/FluffyMachines/master">
    <img src="https://builds.guizhanss.net/f/baoad/FluffyMachines/master/badge.svg" alt="Build status"/>
  </a>
</p>

## 机器

**全自动工作台**: 自动合成原版配方

**全自动盔甲锻造台**: 自动合成盔甲锻造台配方

**全自动魔法工作台**: 自动合成魔法工作台配方

**全自动古代祭坛**: 自动合成古代祭坛配方

**全自动台锯**: 自动合成台锯配方

**洒水机**: 洒水机可以加速2格内的作物生长

**背包装载机**: 把东西放到背包中

**背包卸载机**: 从背包中拿出东西

**高级全自动驱魔机 & 远古之书**: 允许玩家从物品中提取特定的附魔，需要使用古代书籍。

**粉尘制造机**: 可直接将圆石制作成矿粉

**粉尘回收机**: 可以将矿粉变成筛矿

**高级充电台 & 高级充电台升级卡片**: 可以用升级卡片来升级的充电台

## 发电机

**手摇发电机**: 多方快结构，可以在点击拉杆时发电

## 物品

**喷壶**: 给植物或树苗浇水来加速成长

**直升机帽**: 起飞~~~~

**防火符文**: 给物品附上防火属性

**运输车**: 允许玩家拿起箱子并放到别的地方。保留箱子里的物品。

## 工具

**改进爆炸镐 & 爆炸铲**: 破坏前方5x5所有方块，而不是以自身为中心的3x3的方块。可以触发mcMMO的技能。这些可以在`Items.yml`内配置。

**改进伐木斧**: 可以破坏两个内任何相邻的原木，在砍大橡树、金合欢树或丛林树时特别有用。

**镰刀**: 一下子收获5个植物

**多功能工具**: 镐、斧、铲三合一工具。

## 其它

**末影箱提取节点**: 将物品从末影箱提取到普通箱子中

**末影箱输入节点**: 将物品从普通箱子输入到末影箱中

*提取与输入节点不会堆叠物品，这会带来更多的性能消耗。你可以使用货运来处理。*

**铸造厂 & 超热炉**: 允许存储矿粉，也可以直接烧成矿锭取出。

**蓬松箱子**: 存储容器，可以存储一种物品

**传送装置 & 传送装置配置器**: 短途传送装置

**备用电梯板**: 与 Slimefun 电梯板一致。

**便携充电器**: 多个等级的手持版充电站，让玩家可以在任何地方充电。

## 常见问题 (FAQ)

#### 铸造厂可以接入货运系统吗?

可以，不过你不能直接对着超热炉放置节点。  
在原本要放置超热炉的地方放上箱子，接入货运节点。然后，将箱子替换为超热炉即可。
