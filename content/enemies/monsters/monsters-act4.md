---
draft: false
title: "Monsters Act 4"
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

if damage is greater than hp:
 - dam is equal to the RKF multiplied by 0.005 and the eK
 - hp is equal to the RKF multiplied by 0.002 an the eK

else if the damage is smaller than the hp: 
 - dam is equal to the RKF multiplied by 0.005 an the eK
 - hp is equal to the RKF multiplied by 0.015 an the eK

if dam is smaller than 100:
 - dam is equal to 100

if hp is smaller than 50:
 - hp is equal to 50

dam is equal to the dam divided by 50 multiplied 50

hp is equal to the hp divided by 50 multiplied 50

**Variables**: 

RKF is equal to the round number

x is equal to the RKF divided by 2 plus the RKF divided by 5

y is equal to the RKF divided by 3 multiplied by 2

{{% /details %}}