---
content-type: api
navigation-topic: api-navigation-topic
title: Escapezeichen in API-Antworten
description: Escapezeichen in API-Antworten
author: Becky
feature: Workfront API
role: Developer
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 8%

---

# Escapezeichen in API-Antworten

Die Syntax einiger API-Antworten kann das Escape-Zeichen enthalten, `\` (umgekehrter Schrägstrich). Ein Escape-Zeichen zeigt an, dass das Zeichen oder die Zeichenfolge der Zeichen, die unmittelbar auf das Maskierungszeichen folgen, einen Sonderwert hat. Beispiel: `\t` teilt dem Lesegerät mit, dass `t` sollten so ausgelegt werden, dass `tab` und nicht als Buchstaben &quot;t&quot;. Eine Zeichenfolge aus einem oder mehreren Zeichen nach dem umgekehrten Schrägstrich wird als Escape-Sequenz bezeichnet.

Hexadezimale Escapesequenzen erfordern die Verwendung gültiger Hexadezimalziffern. In der folgenden Tabelle sind die Escape-Sequenzen aufgeführt, die in Adobe Workfront-API-Antworten kodiert sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Escape-Sequenz</strong> </th> 
   <th><strong>Unicode-Zeichen</strong> </th> 
   <th><strong>Repräsentiert</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>\u000<em>x</em></p> <p>Wo <em>x</em> ist der Hexadezimalcode für die Zahlen 0 bis 7</p> </td> 
   <td>0-7</td> 
   <td>Unicode-Zeichen, dargestellt durch Codepunkte 0 bis 7</td> 
  </tr> 
  <tr> 
   <td>\b</td> 
   <td>8</td> 
   <td>Rücktaste</td> 
  </tr> 
  <tr> 
   <td>\t</td> 
   <td>9</td> 
   <td>Tab.</td> 
  </tr> 
  <tr> 
   <td>\n</td> 
   <td>10</td> 
   <td>Neue Zeile</td> 
  </tr> 
  <tr> 
   <td>\u000b</td> 
   <td>11</td> 
   <td>Vertikaler Tab</td> 
  </tr> 
  <tr> 
   <td>\f</td> 
   <td>12</td> 
   <td>Formular-Feed</td> 
  </tr> 
  <tr> 
   <td>\r</td> 
   <td>13</td> 
   <td>Wagenrücklauf</td> 
  </tr> 
  <tr> 
   <td> <p>\u00<em>xx</em></p> <p><em>Dabei ist xx der Hexadezimalcode für die Zahlen 14 bis 31</em> </p> </td> 
   <td>14 - 31</td> 
   <td>Unicode-Zeichen, dargestellt durch die Codepunkte 14 bis 31</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/ (Schrägstrich)</td> 
  </tr> 
  <tr> 
   <td> <p>\u003c</p> </td> 
   <td>60</td> 
   <td>&lt; (Kleiner als)</td> 
  </tr> 
  <tr> 
   <td> <p>\\</p> </td> 
   <td>92</td> 
   <td>\ (linksseitiger Schrägstrich)</td> 
  </tr> 
  <tr> 
   <td> <p>\u<em>xxxx</em></p> <p>Wo <em>xxxx</em> ist der hexadezimale Code für eine beliebige Zahl über 127</p> </td> 
   <td>128+</td> 
   <td>Unicode-Zeichen für jeden Codepunkt über 127</td> 
  </tr> 
 </tbody> 
</table>
