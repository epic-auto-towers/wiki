---
draft: false
title: "Pity Mode"
---

The Game has a mechanic where the monsters in the act 3 of the game get weaker after you loose a round to them.

``` c
if (ScrAscCheckAsc(4))
{
    hp = round(power(hp, 0.992));
    dam = round(power(dam, 0.981));
    
    if (control.act3_pity > 0)
    {
        hp /= (1 + (control.act3_pity * 0.5));
        dam /= (1 + (control.act3_pity * 0.5));
        trace("PITY", control.act3_pity);
        control.act3_pity -= 0.05;
    }
}
else
{
    if (control.act3_pity > 0)
    {
        hp /= (1 + control.act3_pity);
        dam /= (1 + control.act3_pity);
        trace("PITY", control.act3_pity);
        control.act3_pity -= 0.05;
    }
    
    hp = round(power(hp, 0.987));
    dam = round(power(dam, 0.976));
}
```