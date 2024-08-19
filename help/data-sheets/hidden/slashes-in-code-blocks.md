---
title: Slashes in codeblokken UGP-11189
description: Slashes in codeblokken UGP-11189 test
hide: true
hidefromtoc: true
source-git-commit: 2255dad674f1b4d456ffb50ebec9313bc4b3d7f5
workflow-type: tm+mt
source-wordcount: '46'
ht-degree: 0%

---

# Slash in codeblokken

1. Voer de opdracht uit:

   ```bash
   vendor/bin/magento-patches -n status |grep "27015\|Status"
   ```

1. Voer de opdracht uit (escape):

   ```bash
   vendor/bin/magento-patches -n status |grep "27015&bsol;|Status"
   ```

Niet in codeblok

leverancier/bin/magento-patches -n status |grep &quot;27015\|Status&quot;

Geslaagd:

leverancier/bin/magento-patches -n status |grep &quot;27015&amp;bsol;|Status&quot;

