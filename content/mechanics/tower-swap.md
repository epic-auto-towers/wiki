---
draft: false
title: "Tower Swap"
---

After the second boss your main tower swaps to a different tower. This can be the [Ancient Tower](/towers/ancient-tower) or the [Divine Tower](/towers/divine-tower).

To make it so that you don't always get the same tower the dev made a mechanic where the game keeps track of your tower spawns. As seen in the code snippet.

``` c
if (_aSize >= 3 && _arr[_aSize - 1] == _arr[_aSize - 2] && _arr[_aSize - 1] == _arr[_aSize - 3] && _arr[_aSize - 1] == 39)
{
    trace("[TwGenTrueTw] last 3 spawns were Ancient. Spawning other towers...");
    return choose(62, 62);
}
else if (_arr[_aSize - 1] == _arr[_aSize - 2] && _arr[_aSize - 1] == 62)
{
    trace("[TwGenTrueTw] last 2 spawns were Divine. Spawning other towers...");
    return choose(39, 39);
}
```
{{< callout type="info" >}}
If this is not the case it will choose like this: choose(39, 39, 62).
This means there is always a higher chance to get the ancient tower
{{< /callout >}}
