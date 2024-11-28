---
draft: false
title: "Monsters Act 3"
---

| Balanced Stats | High Health | High Damage |
|--------|--------|--------|
| ![landscape](/images/enemies/monsters/monsters_act3_0.png)  |  ![landscape](/images/enemies/monsters/monsters_act3_1.png) | ![landscape](/images/enemies/monsters/monsters_act3_2.png) |
| {{< center-small >}}
2 + x{{< icon "dmg" >}}
{{< /center-small >}} {{< center-small >}}
2 + x {{< icon "hp" >}}
{{< /center-small >}}| {{< center-small >}}
1 + y {{< icon "dmg" >}}
{{< /center-small >}} {{< center-small >}}
3 + x + y {{< icon "hp" >}}
{{< /center-small >}} | {{< center-small >}}
3 + x + y {{< icon "dmg" >}}
{{< /center-small >}} {{< center-small >}}
1 + y {{< icon "hp" >}}
{{< /center-small >}}|

Each battle different kind of sets of these monsters spawn.

{{% details title="Scaling" closed="true" %}}

**Calculations**: 

if damage is equal to hp:
 - the damage and hp is multiplied by 25;

else:
 - the damage is multiplied by 20 and the hp is multiplied by 40


dam increases by 5 multiplied by the current round number

hp increases by 15 multiplied by the current round number

**Variables**: 

RKF is equal to the round number minus 20 divided by 2

x is equal to the RKF divided by 2 plus the RKF divided by 5

y is equal to the RKF divided by 3 multiplied by 2

{{% /details %}}