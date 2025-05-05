---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Objekte zwischen Umgebungen vergleichen
description: Sie können Objekte über Umgebungen hinweg vergleichen, um sicherzustellen, dass Ihre Umgebungs-Promotion-Pakete die benötigten Objekte enthalten.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 085b0f04-5a9c-49b9-86d7-2363731ee067
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Objekte zwischen Umgebungen vergleichen

Sie können Objekte zwischen Umgebungen vergleichen, um sicherzustellen, dass Ihre Umgebungspakete die benötigten Objekte enthalten.

Sie wählen die Umgebungen und Objekttypen aus, die verglichen werden sollen. Workfront vergleicht alle Objekte der ausgewählten Typen in beiden Umgebungen und zeigt Daten zu den Objektunterschieden an.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] Plan</strong>
   </td>
   <td> Prime oder Ultimate (nur neue Pläne)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] Lizenzen</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td>Sie müssen [!DNL Workfront] sein.
   </td>
  </tr>
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Ihr Unternehmen muss auf der Adobe-Geschäftsplattform sein, um Objekte zwischen Umgebungen zu vergleichen.

## Generieren eines Objektvergleichs

1. Wechseln Sie zu einer Umgebung, in der Sie ein Objekt vergleichen möchten.
1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **&#x200B;**&#x200B;Setup![Setup-Symbol](/help/_includes/assets/gear-icon-setup.png).
1. Wählen Sie **linken Navigationsbereich die Option** System“ und dann **Umgebungs-Promotion** aus.
1. Klicken **oben rechts** Bildschirm auf „Umgebungen vergleichen“.
1. Wählen Sie im Feld **Source** Umgebung die Umgebung aus, in der Sie das Paket erstellen möchten. Dies ist die Umgebung, aus der Sie Objekte **&#x200B;**.
1. Wählen Sie im Feld **Zielumgebung** die Umgebung aus, in der Sie das Paket installieren möchten. Dies ist die Umgebung, in die Sie Objekte **kopieren**.
1. Wählen Sie im Bereich **Zu vergleichende Objekte** die Objekttypen aus, die Sie zwischen Umgebungen vergleichen möchten.
1. Klicken **oben rechts** Bildschirm auf „Vergleich generieren“.

   Je nach Anzahl und Größe der verglichenen Objekte kann es einige Zeit dauern, bis der Vergleich durchgeführt wird.

## Objektvergleich anzeigen

Nach Abschluss der Vergleichserstellung wird der Vergleich angezeigt.

Die Liste enthält Objekte des ausgewählten Typs bzw. der ausgewählten Typen, die in der Quellumgebung vorhanden sind, ob diese Objekte in der Zielumgebung fehlen und ob es Feldunterschiede zwischen den beiden gibt.

>[!BEGINSHADEBOX]

![Vergleichsbeispiel](assets/environment-promotion-comparison.png)

In diesem Beispiel:

* Die erste Zeile zeigt ein Objekt an, das in der Zielumgebung vorhanden ist, sich jedoch von der Quellumgebung unterscheidet.
* Die zweite Zeile zeigt ein Objekt an, das in der Zielumgebung vorhanden und mit dem in der Quellumgebung identisch ist.
* Die dritte Zeile zeigt ein Objekt an, das nicht in der Zielumgebung vorhanden ist.

>[!ENDSHADEBOX]

So zeigen Sie bestimmte Objektunterschiede an:

1. Klicken Sie auf das Lupensymbol ![Vergleichssymbol](assets/compare-icon.png) in der Zeile für dieses Objekt.

   Ein Fenster mit allen Feldern dieses Objekts wird geöffnet. Unterschiede sind rot markiert.

## Erstellen eines Pakets aus einem Objektvergleich

Sie können ein Paket direkt aus einem Objektvergleich erstellen.

Anweisungen finden Sie unter [Erstellen eines Pakets aus einem Objektvergleich](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-a-package-from-an-object-comparison) im Artikel Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets.
