# AbyssClicker

一款暗黑像素风 Roguelike：每一次点击都会被听见。
A dark pixel-art roguelike where every click is heard.

## 在浏览器里直接玩 / Play in your browser

**👉 [frankshi1998-hash.github.io/AbyssClicker-releases](https://frankshi1998-hash.github.io/AbyssClicker-releases/)**

电脑浏览器（Chrome / Edge / Firefox）最好，第一次加载约 110 MB，按 F11 全屏更好。手机和平板也能玩：横过来，点一下＝点击，长按＝查看格子说明。存档留在这个浏览器里。
Best in a desktop browser (Chrome / Edge / Firefox); the first load is about 110 MB, and fullscreen (F11) looks best. Phones and tablets work too: turn it sideways, tap to click, hold to read a tile. Your progress is saved in that browser.

## 下载最新版 / Download the latest version

**👉 [Releases → Latest](https://github.com/frankshi1998-hash/AbyssClicker-releases/releases/latest)**

在页面底部的 Assets 里选你的系统：
Pick your system under Assets at the bottom of the page:

| 文件 / File | 系统 / System |
| --- | --- |
| `AbyssClicker_v…_2026-…zip` | Windows 10/11 (64-bit) |
| `AbyssClicker_v…_mac_…zip` | macOS 12+ (Intel 和 Apple 芯片 / Intel and Apple silicon) |

## 怎么运行 / How to run

**Windows：** 解压，双击 `AbyssClicker.exe`。如果 Windows 提示"已保护你的电脑"，点"更多信息"→"仍要运行"（游戏没有付费签名）。
**Windows:** unzip and double-click `AbyssClicker.exe`. If SmartScreen says it protected your PC, click "More info" → "Run anyway" (the game is not code-signed).

**Mac：** 解压后先读 `Mac_先读我.txt`。第一次打开要右键 `AbyssClicker.app` → 打开 → 再点打开；还是打不开就在终端运行 `xattr -cr AbyssClicker.app`。
**Mac:** read `Mac_先读我.txt` first. The first time, right-click `AbyssClicker.app` → Open → Open. If it still refuses, run `xattr -cr AbyssClicker.app` in Terminal.

## 怎么玩 / How to play

一局是 10 层，每层是一张 7×7 的格子地图。第 5 层有守门人（回声骑士或守钥人），第 10 层是最终首领（噬声者或什一圣徒）。第一次玩会先打一层教学关。
A run is 10 floors, each a 7×7 board. Floor 5 holds a gatekeeper (the Echo Knight or the Keywarden), floor 10 the final boss (the Noise Eater or the Tithe-Saint). Your first time starts with a tutorial floor.

- **左键点没翻开的格子**：翻开它。不出声，但算一次行动，怪物会跟着行动。
  **Left-click a hidden tile** to reveal it. It is quiet, but it is an action: the monsters act after it.
- **左键点怪物**：攻击。先把鼠标停在怪物上，可以看到会造成多少伤害、谁会死、谁会反击。
  **Left-click a monster** to attack. Hover first to see the damage, what dies and who strikes back.
- **右键点怪物**：看它的卡片和规则。
  **Right-click a monster** for its card and its rule.
- **噪音**：攻击会发出声音，声音在地图上一格一格传开，传到的怪物会被引出来或察觉你。每层的噪音从 0 开始，分四级：平静（0～24）、警觉（25～49）、搜捕（50～74）、惊动（75～100），怪物造成的伤害分别 +0%、+10%、+20%、+30%。噪音到 100 时收账人出现。下楼时按离开时的噪音等级回复生命：平静 30%、警觉 20%、更高 10%（按最大生命计算）。
  **Noise:** attacks make sound; it spreads over the board tile by tile, and the monsters it reaches come out or notice you. Each floor starts at 0 Noise, in four tiers: Calm (0-24), Alert (25-49), Hunted (50-74), Roused (75-100); monsters deal +0%, +10%, +20% and +30% damage at each. At 100 the Tollkeeper comes. Taking the stairs heals you by the tier you leave at: 30% of your Max HP when Calm, 20% when Alert, 10% above that.
- **连锁**：每次击杀都是一环，每环让伤害和击杀金币 +10%；一次行动什么都没杀死，连锁就断。
  **The chain:** every kill is a link, each +10% damage and kill Gold; an action that kills nothing breaks it.
- **成长**：击杀给经验，下楼时升级，每次升级在角色的三条路线里选一步。遗物来自精英、商人和事件，会改变规则。
  **Growth:** kills give experience; you level up on the stairs and take a step on one of your character's three routes. Relics come from elites, merchants and events, and change the rules.

## 四个角色 / The four characters

| 角色 / Character | 武器 / Weapon | 被动 / Passive | 技能 / Skill |
| --- | --- | --- | --- |
| **背誓骑士** Oathbroken Knight | 镰刀：攻击目标和它左右各 1 格，或上下各 1 格 / Scythe: hits the target and the tile on each side of it, across or down | 负伤之怒：每损失 2% 最大生命，伤害 +1%（最多 +50%）/ Wounded Fury: +1% damage per 2% of Max HP missing (up to +50%) | 最后的誓言 / Last Oath |
| **盗墓贼** Grave Robber | 刺剑：不发出声音，只打目标 / Rapier: silent, hits the target only | 独猎者：目标周围 8 格没有其他怪 +40%，只有 1 只 +20% / Lone Hunter: +40% with no other monster in the 8 tiles around the target, +20% with one | 暗影突袭 / Shadow Strike |
| **聆听修女** Listening Nun | 香炉提灯：目标周围 8 格的怪受到 10% 伤害，只有目标反击 / Censer Lantern: the monsters in the 8 tiles around take 10%; only the target strikes back | 渐强圣咏：噪音每高一级，伤害 +12% / Rising Hymn: +12% damage for each Noise tier | 安魂钟 / Requiem Bell |
| **歌铠** Cantor | 装模作样：只伤害目标，周围 1 格的怪着迷 / All for Show: hurts the target only, entrances the monsters 1 tile around | 空壳：音符每个 +20% 伤害；一次受到最大生命 15% 以上的伤害会裂开 / Hollow: each note +20% damage; a single hit of 15% of Max HP or more cracks the armour | 哼唱 / Hum |

### 背誓骑士 / Oathbroken Knight
*曾立誓封印深渊，却以失败告终。 / Swore to seal the Abyss and failed.*
生命最多（135）。镰刀攻击目标和它左右各 1 格，或上下各 1 格，哪个方向的怪多就打哪个方向（一样多时打左右）；目标以外被打到的怪以一半伤害反击。每损失最大生命的 2%，伤害 +1%（最多 +50%，即生命为 0 时）。技能「最后的誓言」恢复最大生命的 20%，并让接下来 4 次行动中受到的每次伤害减半；主要靠受到伤害充能，攻击、击杀和发现怪物也会充一点。**玩法：**用声音把怪物引到目标的左右或上下相邻格，一次攻击打到 3 只；生命越低，负伤之怒的加成越高，在危险时用「最后的誓言」回血并减伤。
The most HP (135). The Scythe hits the target and the tile on each side of it, across or down, whichever holds more monsters (across on a tie); the others it hits strike back at half. +1% damage for every 2% of Max HP missing (up to +50%). Last Oath heals 20% of your Max HP and halves every hit you take for your next 4 actions; it charges mostly from damage you take, a little from attacks, kills and monsters found. **How to play:** draw monsters beside your target, across or down, with sound so one attack hits three; the lower your HP, the larger Wounded Fury's bonus; use Last Oath to heal and halve the damage when a fight turns dangerous.

### 盗墓贼 / Grave Robber
*出身贵族的千金小姐，私底下的爱好却是盗墓。 / A noble heiress whose secret hobby is robbing tombs.*
生命 105，暴击率 15%（其他角色 10%）。刺剑攻击不发出声音，只打目标一只。目标周围 8 格没有其他怪物时伤害 +40%，只有 1 只时 +20%（召唤出来的怪不算）。技能「暗影突袭」让接下来 3 次攻击必定暴击，被攻击的怪不会反击；靠翻开格子、打开宝箱和攻击落单的怪充能。**玩法：**翻格子和攻击都不发出声音（在已翻开的怪旁边翻格子除外），噪音容易保持在平静；先打周围没有同伴的怪，拿到独猎者的 +40%。
105 HP and a 15% crit chance (the others have 10%). The Rapier makes no sound and hits its target only. +40% damage when no other monster stands in the 8 tiles around the target, +20% with one (summoned monsters do not count). Shadow Strike makes your next 3 attacks crit, and the monsters you hit do not strike back; it charges from revealing tiles, opening chests and striking a lone monster. **How to play:** neither revealing (except beside a revealed monster) nor your attacks make sound, so the floor stays Calm easily; strike monsters with no others around them for Lone Hunter's +40%.

### 聆听修女 / Listening Nun
*听见了深渊的呼唤，并想查明它在呼唤何人。 / Hears the Abyss calling, and wants to know whom.*
生命 125。香炉提灯攻击时，目标周围 8 格的怪也受到 10% 的伤害，但只有目标会反击。噪音每高一级（警觉、搜捕、惊动），伤害 +12%（最多 +36%）。技能「安魂钟」对所有已翻开的怪造成你攻击力 80% 的伤害，它们不会反击，没被打死的陷入眩晕（跳过下一次反击）；它算一次行动，噪音每上升 1 点充能 3%，一次最多 15%。**玩法：**噪音越高，渐强圣咏的加成越高，安魂钟也充得越快；声音会把怪引到一起，再用安魂钟一次打到所有翻开的怪。噪音到 100 收账人会出现，要在那之前离开或打完。
125 HP. When the Censer Lantern attacks, the monsters in the 8 tiles around the target take 10% of the damage too, but only the target strikes back. +12% damage for each Noise tier (Alert, Hunted, Roused; up to +36%). Requiem Bell hits every revealed monster for 80% of your Attack; they do not strike back, and the survivors are dazed (they skip their next strike-back); it is an action and charges 3% for each point of Noise, at most 15% at once. **How to play:** the higher the Noise, the larger Rising Hymn's bonus and the faster the bell charges; sound draws monsters together, and the bell then hits every revealed one at once. At 100 Noise the Tollkeeper comes, so leave or finish before then.

### 歌铠 / Cantor（v0.7.5 新角色 / new in v0.7.5）
*一具会歌唱的盔甲，但是为什么会在这？ / An armour that sings. But why is it here?*
生命最少（85），要用 **60 道刻痕**解锁。武器只是摆设（「装模作样」），伤害来自歌：只伤害目标，目标周围 1 格的怪不受伤害，但会**着迷**：不会抢先出手，反击伤害减半；它反击之后会醒来，直到你下一次攻击才会再着迷。每次没有受到伤害的行动给 1 个音符（最多 5 个）；下一次造成伤害的攻击唱出全部音符，每个 +20% 伤害（5 个即 +100%）。一次受到最大生命 15% 以上的伤害，盔甲裂开：噪音 +5，音符全部丢失，着迷的怪醒来并察觉你。技能「哼唱」给 2 个音符，并让下一次攻击传到的怪必定着迷；不算行动，最多存 5 次。**玩法：**攒满 5 个音符再攻击生命高的怪（+100% 伤害）；攻击会反击的怪之前先用哼唱让它着迷，它的反击伤害减半，你就更不容易因为一次受到 15% 以上的伤害而裂开。
The least HP (85); unlocked with **60 marks**. The weapon is only for show ("All for Show"); the damage comes from the song, which hurts only its target and **entrances** the monsters 1 tile around without hurting them: an entranced monster does not strike first and strikes back at half; striking back wakes it until your next attack. Every action in which you take no damage gives a note (up to 5); your next damaging attack sings them all, +20% damage each (+100% with 5). A single hit of 15% of your Max HP or more cracks the armour: Noise +5, all notes are lost, and the entranced wake and notice you. Hum gives 2 notes and makes your next attack entrance everything it reaches; it is not an action and stores up to 5 uses. **How to play:** gather all 5 notes before attacking a monster with high HP (+100% damage); hum before attacking a monster that will strike back, so it is entranced and strikes back at half, which keeps a single hit below the 15% that cracks you.

## 难度：深渊铭记 / Difficulty: The Abyss Remembers

想更难，就在**选人界面**用箭头选「深渊铭记」的等级（0～4 级，0 是普通难度）。每一级在前一级的基础上再加一条规则：
For a harder run, pick a level of **The Abyss Remembers** with the arrows on **character select** (0 to 4; 0 is the normal game). Each level keeps the rules of the levels below and adds one:

| 等级 / Level | 新规则 / The rule it adds |
| --- | --- |
| 1 | 深渊看得更紧：在已经翻开的怪旁边翻格子，声音传 2 格，噪音 +6（普通是 1 格、+3）。/ The abyss watches harder: revealing a tile beside a revealed monster is heard 2 tiles away, Noise +6 (normally 1 tile, +3). |
| 2 | 猎手倒数 2 次行动就攻击（普通是 3 次）；噪音可以超过 100：超过 100 是「暴露」，怪物造成的伤害 +40%；到 150 清算者出现，它每次攻击命中你，拿走你 10% 的金币。/ Hunters strike after 2 actions, not 3. Noise can pass 100: past it the floor is Exposed and monsters deal +40% damage; at 150 the Reckoner comes, and each of its hits takes 10% of your Gold. |
| 3 | 每一层开局就是「警觉」（噪音 25）。/ Every floor starts at Alert (Noise 25). |
| 4 | 首领在剩四分之一生命时进入第三阶段。/ Bosses gain a third phase at a quarter of their HP. |

- **怎么开启：**每个角色各自算。用某个角色在某一级赢下一局，这个角色就能选下一级。第 1 级也可以在图鉴的「成就」页用 30 道刻痕直接解锁（所有角色都能选）。
  **Opening it:** each character climbs alone: win a run at a level to open the next one for that character. Level 1 can also be bought for 30 marks in the Codex's Achievements tab (for every character).
- **奖励：**在深渊铭记下赢下一局，每一级多给 5 道刻痕。
  **The reward:** a win on The Abyss Remembers gives 5 more marks for each level.

## 无尽模式：更深 / Endless: Deeper

打倒第 10 层的最终首领、赢下一整局之后，结算画面会出现「继续深入」。从这里往下没有尽头：每一层开始时的噪音都更高，怪物一层比一层强，每 3 层有一个宝库，每 5 层会有一个首领挡住楼梯：从回声骑士、守钥人、噬声者、什一圣徒四个里随机出，越深越强。在这里死掉不算失败（这一局已经赢了），每个角色最深到过第几层、用了多久，记在图鉴的「记录」页。
Win a whole run by beating the final boss on floor 10, and the run's end offers "Go Deeper": an endless descent. Each floor starts louder than the last, the monsters keep growing, every third floor is a vault, and every fifth a boss guards the stairs: one of the four (the Echo Knight, the Keywarden, the Noise Eater, the Tithe-Saint), stronger the deeper you go. Dying down there is not a defeat (the run is already won); each character's deepest floor and its time are kept in the Codex's Records tab.

### 分数 / Score

每局结束都会算分：走得多深、打倒了什么（精英、守关首领、最终首领）、通关、最长连锁、拿到的金币都算分；「更深」每一层比上面的楼层分数高得多；深渊铭记每高一级，总分再乘 1.25。结算界面显示这局的分数和在本机的名次，图鉴的「记录」页列出本机前 10 名和用的角色。
Every run scores: how deep you went, what you beat (elites, gatekeepers, the final boss), a win, your best chain and the Gold you found; each Deeper floor is worth far more than one above, and each level of The Abyss Remembers multiplies the total by 1.25. The run end shows the score and its place on this computer; the Codex's Records tab lists the best 10 with their characters.

## 深渊刻痕 / Marks of the descent

刻痕是一直保留的货币。每一局不管输赢都会留下刻痕：每到一层 +2，打倒守门人 +5，打倒最终首领 +10；赢下一局时，深渊铭记每一级再 +5，连胜还有额外刻痕。在图鉴的「成就」页用刻痕解锁一开始锁着的东西：
Marks are the currency that lasts. Every run, won or lost, leaves marks: +2 for each floor reached, +5 for the gatekeeper, +10 for the final boss, and on a win +5 for each level of The Abyss Remembers and a bonus for a winning streak. Spend them in the Codex's Achievements tab on what starts locked:

- **歌铠**（60 道）。/ **The Cantor** (60).
- **深渊铭记第 1 级**（30 道）：不用先赢一局就能选的难度（见上面的「难度」）。
  **The Abyss Remembers, level 1** (30): the harder rules without a win first (see Difficulty above).
- **14 件遗物**（12～40 道）：解锁之后才会出现在奖励里。
  **14 relics** (12-40 each): once unlocked they can appear among the rewards.

刻痕只买新的选择，不会让角色在两局之间变强。成就另外还会解锁铁匠的 3 把武器和几件遗物。
Marks buy new choices, never strength carried between runs. Achievements separately unlock 3 of the blacksmith's weapons and a few relics.

## 存档 / Saves

- **进度**（解锁、刻痕、成就、记录、图鉴、设置、教学关已完成）自动保存。
  **Progress** (unlocks, marks, achievements, records, the codex, settings, the tutorial done) is saved automatically.
- **一局**在每一层开始时存档：标题画面点「继续」接着玩，暂停菜单里有「保存并退出」。一层打到一半退出，再进来会回到这一层刚进来时的样子。
  **A run** is saved at the start of each floor: "Continue" on the title picks it up, and the pause menu has "Save & Quit". Quit halfway through a floor and you come back to that floor as you found it.
- **更新版本**：从 v0.7.5 起，新版本会保留你的进度，只丢掉旧版本里没打完的那一局（规则可能变了）。v0.7.4 及更早的版本每次更新都会清空存档。
  **New versions:** from v0.7.5 on, a new version keeps your progress and drops only a run you had not finished (its rules may have changed). Up to v0.7.4 every new version cleared the saves.

### 换新版本时怎么保留存档 / Keeping your save when you update

进度不在游戏文件夹里，所以换版本不用复制任何文件：
Your progress is not kept in the game's folder, so updating needs no files copied:

1. 想保留正在打的那一局，先在旧版本里打完它（新版本第一次打开会丢掉没打完的一局）。
   To keep a run in progress, finish it in the old version first (a new version's first launch drops an unfinished run).
2. **Windows**：下载新版本的压缩包，解压到任意文件夹（新文件夹或覆盖旧的都行），双击新的 `AbyssClicker.exe`。解锁、刻痕、成就、记录、设置都会自动出现。旧版本的文件夹可以直接删掉。
   **Windows:** download the new zip, unzip it anywhere (a new folder or over the old one), and run the new `AbyssClicker.exe`. Your unlocks, marks, achievements, records and settings are there. The old folder can be deleted.
3. **Mac**：用新的 `AbyssClicker.app` 替换旧的（第一次打开同样要右键「打开」，见 `Mac_先读我.txt`），进度会自动读出来。
   **Mac:** replace the old `AbyssClicker.app` with the new one (open it the first time with right-click → Open, see `Mac_先读我.txt`); your progress is read automatically.
4. **浏览器**：用同一个浏览器打开同一个网址就是新版本，进度还在。如果看到的还是旧版本，按 Ctrl+F5（Mac 上 Cmd+Shift+R）强制刷新。
   **Browser:** open the same address in the same browser; the new version keeps your progress. If the old version still shows, force a refresh with Ctrl+F5 (Cmd+Shift+R on a Mac).

不要做的事：不要点设置里的「重置进度」，也不要删除下面「存在哪里」列出的位置，那样进度才会真的没了。换电脑的话，进度不会跟过去。
Don't: press "Reset Progress" in Settings, or delete the places listed under "Where it lives" below; those really erase it. Progress does not move to another computer.
- 设置里的「重置进度」会清空全部进度，从头开始。
  "Reset Progress" in Settings clears it all and starts over.
- 存在哪里 / Where it lives:
  - Windows：进度在注册表 `HKEY_CURRENT_USER\Software\DefaultCompany\AbyssClicker1`，一局的存档和游戏记录在 `%USERPROFILE%\AppData\LocalLow\DefaultCompany\AbyssClicker1`。
    Windows: progress in the registry under `HKEY_CURRENT_USER\Software\DefaultCompany\AbyssClicker1`; the run save and the play logs in `%USERPROFILE%\AppData\LocalLow\DefaultCompany\AbyssClicker1`.
  - Mac：进度在 `~/Library/Preferences/unity.DefaultCompany.AbyssClicker1.plist`，一局的存档和游戏记录在 `~/Library/Application Support/DefaultCompany/AbyssClicker1`。
    Mac: progress in `~/Library/Preferences/unity.DefaultCompany.AbyssClicker1.plist`; the run save and the play logs in `~/Library/Application Support/DefaultCompany/AbyssClicker1`.
  - 浏览器：存在这个浏览器里；清除网站数据会把它删掉，换一个浏览器也看不到。
    Browser: kept in that browser; clearing the site's data deletes it, and another browser will not see it.

## 反馈 / Feedback

压缩包里有 `测试说明.txt` / `README_EN.md`：玩法、规则和想听的反馈都在里面。游戏记录在设置里的"打开记录文件夹"，打包发回来就是最好的反馈。
The zip holds `测试说明.txt` / `README_EN.md` with the controls, the rules and what feedback helps. Settings → "Open Log Folder" shows your play logs: zipping that folder and sending it back is the most useful feedback of all.

## 制作人 / Made by

**SulyTea** · 联系方式 / Contact: frankshi1998@gmail.com · B站 / Bilibili: https://space.bilibili.com/1324888
