---
draft: false
title: "Monsters in the Endless Mode"
---

The pattern of the previous acts repeat now. 

* Between the Round 35 and 39 the monsters of the 1st Act spawn. At round 40 the 1st boss apears again. (with a higher scaling)
* Between the Round 40 and 49 the monsters of the 2nd Act spawn. At round 50 the 2nd boss apears again. (with a higher scaling)
* Between the Round 50 and 59 the monsters of the 3rd Act spawn. At round 60 the 3rd boss apears again. (with a higher scaling)

Each battle different kind of sets of these monsters spawn.

{{< callout type="warning" >}}
  After round 60 the endboss of act 4 apears every round. With each round it scales higher and higher.
{{< /callout >}}

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