#BetterArrows v0.1

`Weapon` `Improvement` `Arrow` `TippedArrow`

調整藥箭效果，使其「可用」

## 基礎

#### 藥箭
> 藥箭效果的持續時間是相應的藥水的1⁄8，持續時間不會被弓的強力影響。
>
> 箭的狀態效果與藥水正常的效果相同。


    | 藥水 | 噴濺藥水 | 滯留藥水 | 藥水箭
:-- | :-: | :-: | :-: | :-:
立即效果（比例） | 2 | 2[¹](#note1) | 1 | 1
持續效果（比例） | 8 | 8[¹](#note1) | 2 | 1

##### 釀造藥水不會同時擁有立即效果或持續效果
    
<a name="note1"></a>
###### 註¹ 效果以中心為 100% 線性減少到 4 個方塊外的 0%

## 調整

大部分藥箭不再造成直接傷害，包含直接傷害將特別標註。

被不具直接傷害之藥箭擊中時將受到 `0` 點傷害，並且不被擊退。

---
#### 新合成公式

> TODO: [img]

##### 藥箭合成

> 箭矢: `8` --> `4`
> 
> 產物: `8` --> `4`
> 
> 類型為「持續」的藥箭，持續時間調整為原來的 `2` 倍

---
#### 個別調整

##### 藥箭種類 ![arrow] - 類型
> 
> __藥箭原始效果__
> > 藥箭新特性

###### 回復之箭 ![arrow-regen] - 持續
###### 迅捷之箭 ![arrow-speed] - 持續
###### 抗火之箭 ![arrow-fire-resistance] - 持續
##### 治療之箭 ![arrow-instant-heal] - 立即
> > 若目標為不死生物，擊中時將造成與治療量相等的傷害
>
> __立即治療 (![heart])__
> > 基礎治療量 3 (![heart]![half_heart])
> >
> > 依照弓的 `強力` 等級以及蓄力時間獲得額外治療量 1 (![half_heart]) ~ 5 (![heart]![heart]![half_heart])  
> > `火焰` 附魔能提升 2 (![heart]) 額外治療量
>
> __立即治療 II (![heart]![heart])__
> > 基礎治療量 6 (![heart]![heart]![heart])
> >
> > 依照弓的 `強力` 等級以及蓄力時間獲得額外治療量 2 (![heart]) ~ 11 (![heart]![heart]![heart]![heart]![heart]![half_heart])  
> > `火焰` 附魔能提升 4 (![heart]![heart]) 額外治療量

###### 夜視之箭 ![arrow-night-vision] - 持續
###### 力量之箭 ![arrow-strength] - 持續
###### 跳躍提升之箭 ![arrow-jump] - 持續
###### 隱形之箭 ![arrow-invisibility] - 持續
##### 劇毒之箭 ![arrow-poison] - 持續
> > 現在會依照弓的 `強力` 等級立即造成 2 (![heart]) ~ 6 (![heart]![heart]![heart]) 的穿透傷害（不計蓄力時間）  
> > 對不死生物仍能造成穿透傷害，但無法使其中毒

###### 虛弱之箭 ![arrow-weakness] - 持續
###### 緩速之箭 ![arrow-slowness] - 持續
##### 傷害之箭 ![arrow-instant-damage] - 立即
> > 將繼承原有的傷害  
> > 若目標為不死生物，額外傷害轉為傷害減免，當總傷害小於零將回復其生命
>
> __立即傷害 ( ![heart]![half_heart] )__
> > 調整傷害增量為 5 (![heart]![heart]![half_heart])
>
> __立即傷害 II ( ![heart]![heart]![heart] )__
> > 調整傷害增量為 9 (![heart]![heart]![heart]![heart]![half_heart])

##### 水下呼吸之箭 ![arrow-water-breathing] - 持續
> > 擊中時恢復已損失的氧氣槽

###### 幸運之箭 ![arrow-luck] - 持續

## 參考資源
- [Minecraft - 箭](http://minecraft-zh.gamepedia.com/%E7%AE%AD)
- [Minecraft - 藥水](http://minecraft-zh.gamepedia.com/%E8%8D%AF%E6%B0%B4)
- [Minecraft - 噴濺藥水](http://minecraft-zh.gamepedia.com/%E5%96%B7%E6%BA%85%E8%8D%AF%E6%B0%B4)
- [Minecraft - 滯留藥水](http://minecraft-zh.gamepedia.com/%E6%BB%9E%E7%95%99%E8%8D%AF%E6%B0%B4)

[heart]: status/heart.png "Heart"
[half_heart]: status/half-heart.png "Half heart"

[arrow]: items/arrow.png "arrow"
[arrow-regen]: items/arrow-regen.png "arrow-regen"
[arrow-speed]: items/arrow-speed.png "arrow-speed"
[arrow-fire-resistance]: items/arrow-fire-resistance.png "arrow-fire-resistance"
[arrow-instant-heal]: items/arrow-instant-heal.png "arrow-instant-heal"
[arrow-night-vision]: items/arrow-night-vision.png "arrow-night-vision"
[arrow-strength]: items/arrow-strength.png "arrow-strength"
[arrow-jump]: items/arrow-jump.png "arrow-jump"
[arrow-invisibility]: items/arrow-invisibility.png "arrow-invisibility"
[arrow-poison]: items/arrow-poison.png "arrow-poison"
[arrow-weakness]: items/arrow-weakness.png "arrow-weakness"
[arrow-slowness]: items/arrow-slowness.png "arrow-slowness"
[arrow-instant-damage]: items/arrow-instant-damage.png "arrow-instant-damage"
[arrow-water-breathing]: items/arrow-water-breathing.png "arrow-water-breathing"
[arrow-luck]: items/arrow-luck.png "arrow-luck"
