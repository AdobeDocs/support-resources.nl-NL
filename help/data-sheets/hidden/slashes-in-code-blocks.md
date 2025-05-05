---
title: Slashes in codeblokken UGP-11189
description: Slashes in codeblokken UGP-11189 test
hide: true
hidefromtoc: true
source-git-commit: 4fc9b739d18941d276b88f8799163523c8bd5f85
workflow-type: tm+mt
source-wordcount: '45'
ht-degree: 0%

---

# Slash in codeblokken

1. Voer de opdracht uit:

   ```bash
   vendor/bin/magento-patches -n status |grep "27015\|Status"
   ```

1. Volgende stap

Niet in codeblok

leverancier/bin/magento-patches -n status |grep &quot;27015\|Status&quot;

backslash overgeslagen:

leverancier/bin/magento-patches -n status |grep &quot;27015&bsol;|Status&quot;
