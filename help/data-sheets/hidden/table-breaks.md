---
title: Tabeleinden
description: Testen van verschillende tabeleinden
hide: true
hidefromtoc: true
source-git-commit: cd9f841a3f720ee366b33f3a78f7ca731c0b865a
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 6%

---

# Tabeleinden

## Standaardtabel met markeringen `<br>`

**VAST`Green<br>Red<br>Blue`**

|  | Getal | Kleuren |
|---|---|---|
| Juanya | 17 | Groen<br>Rood<br>Blauw |
| Maria | 23 | Geel<br>Bruin |

{style="table-layout:fixed"}

**AUTO`Green<br>Red<br>Blue`**

|  | Getal | Kleuren |
|---|---|---|
| Juanya | 17 | Groen<br>Rood<br>Blauw |
| Maria | 23 | Geel<br>Bruin |

{style="table-layout:auto"}

## Afdruktabel met dubbele waarde `<br>`s

**VAST`Green<br><br>Red<br><br>Blue`**

|  | Getal | Kleuren |
|---|---|---|
| Juanya | 17 | Groen<br><br>Rood<br><br>Blauw |
| Maria | 23 | Geel<br><br>Bruin |

{style="table-layout:fixed"}

**AUTO`Green<br><br>Red<br><br>Blue`**

|  | Getal | Kleuren |
|---|---|---|
| Juanya | 17 | Groen<br><br>Rood<br><br>Blauw |
| Maria | 23 | Geel<br><br>Bruin |

{style="table-layout:auto"}

## Afdruktabel met `<p>`

**VAST`Green<p>Red<p>Blue`**

|  | Getal | Kleuren |
|---|---|---|
| Juanya | 17 | Groen<p>Rood<p>Blauw |
| Maria | 23 | Geel<p>Bruin |

{style="table-layout:fixed"}

**AUTO`Green<p>Red<p>Blue`**

|  | Getal | Kleuren |
|---|---|---|
| Juanya | 17 | Groen<p>Rood<p>Blauw |
| Maria | 23 | Geel<p>Bruin |

{style="table-layout:auto"}

|  | Getal | Kleuren |
|---|---|---|
| Juanya | 17 | Dit is de kleur **groen** en het is bedoeld om de in lid 1 bedoelde punten op een andere regel te testen. <p>Dit is de kleur **rood** en het is bedoeld om de in lid 1 bedoelde punten op een andere regel te testen. <p>Dit is de kleur **blauw** en het is bedoeld om de in lid 1 bedoelde punten op een andere regel te testen. |
| Maria | 23 | Geel<p>Bruin |

{style="table-layout:fixed"}

|  | Getal | Kleuren |
|---|---|---|
| Juanya | 17 | Dit is de kleur **groen** en het is bedoeld om de in lid 1 bedoelde punten op een andere regel te testen. <p>Dit is de kleur **rood** en het is bedoeld om de in lid 1 bedoelde punten op een andere regel te testen. <p>Dit is de kleur **blauw** en het is bedoeld om de in lid 1 bedoelde punten op een andere regel te testen. |
| Maria | 23 | Geel<p>Bruin |

{style="table-layout:auto"}
