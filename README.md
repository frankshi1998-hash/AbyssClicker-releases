# AbyssClicker

一款只用鼠标玩的暗黑像素风 Roguelike：每一次点击都会被听见。
A dark pixel-art roguelike played with the mouse, where every click is heard.

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
- **噪音**：攻击会出声，声音会在地图上传开，把怪物引过来、惊醒它们。噪音越高，怪物越疼；到 100，收账人会来收账。安静地离开一层，回复的生命最多。
  **Noise:** attacks are heard; the sound spreads over the board, drawing monsters out and waking them. The louder the floor, the harder they hit; at 100 the Tollkeeper comes to collect. A quiet exit heals the most.
- **连锁**：每次击杀都是一环，每环让伤害和击杀金币 +10%；一次行动什么都没杀死，连锁就断。
  **The chain:** every kill is a link, each +10% damage and kill Gold; an action that kills nothing breaks it.
- **成长**：击杀给经验，下楼时升级，每次升级在角色的三条路线里选一步。遗物来自精英、商人和事件，会改变规则。
  **Growth:** kills give experience; you level up on the stairs and take a step on one of your character's three routes. Relics come from elites, merchants and events, and change the rules.

## 四个角色 / The four characters

| 角色 / Character | 武器 / Weapon | 被动 / Passive | 技能 / Skill |
| --- | --- | --- | --- |
| **背誓骑士** Oathbroken Knight | 镰刀：一刀斩过一整条线 / Scythe: slashes a line | 负伤之怒：越受伤越疼 / Wounded Fury | 最后的誓言 / Last Oath |
| **盗墓贼** Grave Robber | 刺剑：无声，单体 / Rapier: silent, single | 独猎者：打落单的怪 +40% / Lone Hunter | 暗影突袭 / Shadow Strike |
| **聆听修女** Listening Nun | 香炉提灯：安静的小范围 / Censer Lantern | 渐强圣咏：越吵越强 / Rising Hymn | 安魂钟 / Requiem Bell |
| **歌铠** Cantor | 装模作样：伤人的是歌 / All for Show | 空壳：音符与裂甲 / Hollow | 哼唱 / Hum |

### 背誓骑士 / Oathbroken Knight
*曾立誓封印深渊，却以失败告终。 / Swore to seal the Abyss and failed.*
生命最多（135）。镰刀沿着横线或竖线斩过目标，哪边怪多斩哪边；被一起斩到的怪以一半伤害反击。每损失 2% 生命，伤害 +1%（最多 +50%）。技能「最后的誓言」恢复 20% 生命，接下来 4 次行动受到的伤害减半，受伤时充能。**玩法：**把怪引成一排一刀斩完，残血时打得最狠，靠誓言撑过去。
The most HP (135). The Scythe slashes a line through its target, across or down, wherever more monsters stand; the others it catches strike back at half. +1% damage for every 2% HP missing (up to +50%). Last Oath heals 20% and halves every hit for 4 actions; it charges when you are hurt. **How to play:** line them up and cut them down; you hit hardest when hurt, and the oath carries you through.

### 盗墓贼 / Grave Robber
*出身贵族的千金小姐，私底下的爱好却是盗墓。 / A noble heiress whose secret hobby is robbing tombs.*
生命 105，暴击率最高。刺剑不出声，只打一只。打身边没有其他怪的怪 +40%，身边只有一只时 +20%。技能「暗影突袭」让接下来 3 次攻击必定暴击、不会被反击，靠翻格子、开宝箱和打落单的怪充能。**玩法：**安静地翻图，把怪一只只挑出来打，噪音压得低低的。
105 HP and the highest crit chance. The Rapier is silent and hits one monster. +40% damage to a monster standing alone, +20% with one beside it. Shadow Strike makes your next 3 attacks crit with no strike-back; it charges from revealing tiles, opening chests and striking a lone monster. **How to play:** explore quietly, pick them off one at a time, keep the Noise low.

### 聆听修女 / Listening Nun
*听见了深渊的呼唤，并想查明它在呼唤何人。 / Hears the Abyss calling, and wants to know whom.*
生命 125。香炉提灯很安静，能带到身边的怪（10%），只有目标会反击。噪音每升一级（警觉、搜捕、惊动），伤害 +12%。技能「安魂钟」对所有翻开的怪造成攻击力 80% 的伤害、不会被反击，没死的会眩晕；它算一次行动，靠你发出的噪音充能。**玩法：**故意把楼层弄吵，等怪聚过来，敲钟一起收掉，但别吵到收账人上门。
125 HP. The Censer Lantern is quiet and grazes the monsters beside its target (10%); only the target strikes back. +12% damage for each Noise tier (Alert, Hunted, Roused). Requiem Bell hits every revealed monster for 80% of your Attack with no strike-back and dazes the survivors; it is an action and charges from the Noise you make. **How to play:** make the floor loud on purpose, let them gather, ring the bell, but not so loud that the Tollkeeper comes.

### 歌铠 / Cantor（v0.7.5 新角色 / new in v0.7.5）
*一具会歌唱的盔甲，但是为什么会在这？ / An armour that sings. But why is it here?*
生命最少（85），要用 **60 道刻痕**解锁。拿什么武器都只是摆设，伤人的是歌：只伤害目标，传到的周围 1 格的怪会**着迷**（不抢先出手、反击减半）。每次没受伤的行动给 1 个音符，下一击把音符全部唱出，每个 +20%。一下挨到最大生命 15% 以上，盔甲就会裂开：音符全丢，着迷的怪醒来。技能「哼唱」给 2 个音符、让下一击传到的怪必定着迷，不算行动，最多存 5 次。**玩法：**躲开反击攒音符，打硬骨头前先哼唱，一下打出大伤害；别让大怪一下把你打裂。
The least HP (85); unlocked with **60 marks**. Whatever it holds is only for show: it hurts with the song, which hits only its target and **entrances** the monsters a tile around (they do not strike first and strike back at half). Every action that leaves you unhurt gives a note, and your next hit sings them all, +20% each. A single blow of 15% of your Max HP cracks the armour: the notes are lost and the entranced wake. Hum gives 2 notes and makes the next attack entrance everything it reaches; it is not an action and stores up to 5 uses. **How to play:** avoid strike-backs to gather notes, hum before a tough fight and land one big blow; do not let a big monster crack you.

## 无尽模式：更深 / Endless: Deeper

打倒第 10 层的最终首领、赢下一整局之后，结算画面会出现「继续深入」。从这里往下没有尽头：每一层开始时的噪音都更高，怪物一层比一层强，每 3 层有一个宝库，每 5 层守门人会再出现一次、而且更强。在这里死掉不算失败（这一局已经赢了），成绩按走了多深来算，深度一样再比用时，记录在图鉴的「记录」页。
Win a whole run by beating the final boss on floor 10, and the run's end offers "Go Deeper": an endless descent. Each floor starts louder than the last, the monsters keep growing, every third floor is a vault, and every fifth the gatekeeper returns, stronger. Dying down there is not a defeat (the run is already won): the score is how deep you went, then the time, kept in the Codex's Records tab.

## 深渊刻痕 / Marks of the descent

刻痕是一直保留的货币。每一局不管输赢都会留下刻痕：每到一层 +2，打倒守门人 +5，打倒最终首领 +10，在「深渊铭记」难度下每级再加，连胜还有额外刻痕。在图鉴的「成就」页用刻痕解锁一开始锁着的东西：
Marks are the currency that lasts. Every run, won or lost, leaves marks: +2 for each floor reached, +5 for the gatekeeper, +10 for the final boss, more for each level of The Abyss Remembers, and a bonus for a winning streak. Spend them in the Codex's Achievements tab on what starts locked:

- **歌铠**（60 道）。/ **The Cantor** (60).
- **深渊铭记**（30 道）：每个角色 4 级的难度阶梯，选人时选择（更凶的察觉、更快的猎手、开局就警觉、首领多一个阶段）。
  **The Abyss Remembers** (30): a 4-level difficulty ladder for each character, chosen on character select (a harsher watch, faster hunters, floors that start alerted, bosses with a third phase).
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
