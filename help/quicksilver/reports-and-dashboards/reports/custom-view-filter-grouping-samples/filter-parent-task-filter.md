---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Übergeordnete Aufgaben anzeigen'
description: Sie können die folgenden Aufgabenfilter anwenden, um Arbeitsaufgaben anzuzeigen. Arbeitsaufgaben sind Aufgaben, die unabhängig voneinander bearbeitet werden können und anderen Aufgaben nicht übergeordnet sind. In einem Beispiel identifiziert ein Filter untergeordnete Aufgaben, die selbst übergeordnet sein könnten. In diesem Fall handelt es sich nicht um funktionierende Aufgaben.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 1%

---

# Filter: Übergeordnete Aufgaben anzeigen

<!--Audited: 10/2024-->

Sie können die folgenden Aufgabenfilter anwenden, um Arbeitsaufgaben anzuzeigen. Arbeitsaufgaben sind Aufgaben, die unabhängig voneinander bearbeitet werden können und anderen Aufgaben nicht übergeordnet sind. In einem Beispiel identifiziert ein Filter untergeordnete Aufgaben, die selbst übergeordnet sein könnten. In diesem Fall handelt es sich nicht um funktionierende Aufgaben.

>[!TIP]
>
>* Wenn Sie erwägen, einem Bericht mehr als einen Filter hinzuzufügen, empfehlen wir, alle Ihre Filter über die Benutzeroberfläche von Report Builder hinzuzufügen und auf Zum Textmodus wechseln zu klicken, nachdem alle anderen Filterregeln hinzugefügt wurden. Anschließend können Sie den Code für den Filter der übergeordneten Aufgabe wie oben beschrieben hinzufügen. 
>* Es wird außerdem empfohlen, eine Gruppierung für Projektname hinzuzufügen, um die Lesbarkeit des Berichts zu vereinfachen. Weitere Informationen zum Hinzufügen von Gruppierungen zu Ihren Berichten finden Sie im Artikel [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkender zum Ändern eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filter ändern </p></li>
   <li><p>Planen der Änderung eines Berichts</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aufgaben ohne untergeordnete Elemente anzeigen (möglicherweise mit einem übergeordneten Element)

Sie können den folgenden Filter auf einen Aufgabenbericht anwenden, um Aufgaben ohne untergeordnete Elemente anzuzeigen. Sie könnten eigene Eltern haben und Kinder anderer Aufgaben sein.

1. Klicken Sie im **Hauptmenü** ![Hauptmenüsymbol](assets/main-menu-icon.png) in der oberen rechten Ecke oder im **Hauptmenü** ![Hauptmenüsymbol](assets/lines-main-menu.png) in der oberen linken Ecke, falls verfügbar, auf **Berichte**.

1. Klicken Sie **Neuer Bericht**.
1. Wählen Sie einen **Aufgabenbericht**.
1. Klicken Sie **Filter**.
1. Klicken Sie **Filterregel hinzufügen**.
1. Beginnen Sie in der Zeile **Feldname eingeben…** mit der Eingabe von **Anzahl der untergeordneten Elemente** und klicken Sie dann auf **Aufgabe >> Anzahl der untergeordneten Elemente** wenn es in der Liste angezeigt wird.

1. Wählen Sie **Gleich (Groß- und Kleinschreibung** für Ihren Modifikator aus und geben Sie **0** für die Anzahl der untergeordneten Elemente ein.\
   ![Filter der übergeordneten Aufgabe](assets/parent-task-filter-from-the-ui-350x76.png)

   Oder

   Klicken Sie **Wechseln Sie in den Textmodus**, kopieren Sie im Textbearbeitungsfenster den folgenden Text und fügen Sie ihn ein

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Klicken Sie auf **Speichern + schließen**.

   Dadurch wird ein Bericht für alle Aufgaben abgerufen, die in Ihrem System laufende Aufgaben sind. Einige dieser Aufgaben könnten eine übergeordnete Aufgabe haben, sie sind jedoch selbst keine übergeordneten Aufgaben.

## Aufgaben mit übergeordneten Elementen anzeigen (möglicherweise untergeordnete Elemente)

Sie können den folgenden Filter auf einen Aufgabenbericht anwenden, um Aufgaben mit übergeordneten Elementen anzuzeigen, d. h. es handelt sich um untergeordnete Aufgaben. Diese Aufgaben können jedoch auch eigene untergeordnete Elemente haben, da der Filter deren untergeordnete Elemente nicht ausschließt. Untergeordnete Aufgaben, die anderen Aufgaben ebenfalls übergeordnet sind, werden nicht als Arbeitsaufgaben betrachtet.

1. Klicken Sie im **Hauptmenü** ![Hauptmenüsymbol](assets/main-menu-icon.png) in der oberen rechten Ecke oder im **Hauptmenü** ![Hauptmenüsymbol](assets/lines-main-menu.png) in der oberen linken Ecke, falls verfügbar, auf **Berichte**.

1. Klicken Sie **Neuer Bericht**.
1. Wählen Sie einen **Aufgabenbericht**.
1. Klicken Sie **Filter**.
1. Klicken Sie **Filterregel hinzufügen**.
1. Beginnen Sie in der Zeile **Feldname eingeben …** mit der Eingabe **Übergeordnete ID** und wählen Sie dann **Aufgabe >> Übergeordnete ID** aus, wenn sie in der Liste angezeigt wird.
1. Wählen Sie **Modifikator** Ist nicht leer“ aus.

   ![Übergeordnete ID ist nicht leer](assets/filter-parent-id-not-blank-350x100.png)

   Oder

   Klicken Sie **Wechseln Sie in den Textmodus**, kopieren Sie im Textbearbeitungsfenster den folgenden Text und fügen Sie ihn ein: 

   `parentID_Mod=notblank`

1. Klicken Sie auf **Speichern + schließen**.

   Dadurch wird ein Bericht für alle Aufgaben in Ihrem System abgerufen, die Eltern haben und untergeordnete Aufgaben dieser Eltern sind. Einige dieser Aufgaben können auch selbst übergeordnet sein.

## Aufgaben ohne untergeordnete Elemente und ohne übergeordnete Elemente anzeigen (eigenständige Aufgaben)

Sie können den folgenden Filter auf einen Aufgabenbericht anwenden, um eigenständige Arbeitsaufgaben anzuzeigen. Diese Aufgaben haben keine Eltern und keine eigenen Kinder.

1. Klicken Sie im **Hauptmenü** ![Hauptmenüsymbol](assets/main-menu-icon.png) in der oberen rechten Ecke oder im **Hauptmenü** ![Hauptmenüsymbol](assets/lines-main-menu.png) in der oberen linken Ecke, falls verfügbar, auf **Berichte**.

1. Klicken Sie **Neuer Bericht**.
1. Wählen Sie einen **Aufgabenbericht**.
1. Klicken Sie **Filter**.
1. Klicken Sie **Filterregel hinzufügen**.
1. Geben Sie in **Feldname eingeben …** Zeile **Anzahl der untergeordneten Elemente** ein und wählen Sie dann **Aufgabe >> Anzahl der untergeordneten Elemente** aus der Liste aus.
1. Wählen Sie **Gleich (Groß- und Kleinschreibung** für Ihren Modifikator aus und geben Sie **0** für die Anzahl der untergeordneten Elemente ein.
1. Klicken Sie **Weitere Filterregel hinzufügen**.
1. Geben Sie in **Feldnamen eingeben …** Zeile beginnen Sie mit der Eingabe **Übergeordnete ID** und wählen Sie dann **Aufgabe > Übergeordnete ID** aus der Liste aus.
1. Wählen Sie **Modifikator &quot;**&quot; aus.

   ![Übergeordnete ID ist leer und keine untergeordneten Elemente](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Oder

   Anstelle der Schritte 6-10 <!--ensure steps above stay accurate--> klicken Sie auf **Wechseln zum Textmodus** und kopieren Sie im Textbearbeitungsfenster den folgenden Text:

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Klicken Sie auf **Speichern + schließen**.

   Dadurch wird ein Bericht für alle Aufgaben in Ihrem System abgerufen, die keine Eltern oder Kinder haben. Hierbei handelt es sich um eigenständige Arbeitsaufgaben.
