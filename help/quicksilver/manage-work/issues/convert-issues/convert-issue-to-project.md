---
product-area: projects
navigation-topic: convert-issues
title: Konvertieren eines Problems in ein Projekt in Adobe Workfront
description: Konvertieren eines Problems in ein Projekt in Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1978'
ht-degree: 0%

---

# Konvertieren eines Problems in ein Projekt in Adobe Workfront

<!--Audited: 01/2024-->

Wenn nach dem Absenden des Problems noch mehr Arbeit erforderlich ist, können Sie das Problem in ein Projekt konvertieren.

Sie können ein Problem in ein neues Projekt konvertieren oder es mithilfe einer Vorlage in ein Projekt konvertieren. In diesem Artikel werden beide Möglichkeiten zum Konvertieren von Problemen in Projekte beschrieben.

>[!IMPORTANT]
>
>Allgemeine Informationen zu Konvertierungsproblemen finden Sie im Artikel [Übersicht über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Beim Erstellen eines Projekts aus einem Problem werden einige Felder im Projekt von anderen Objekten ausgefüllt. Weitere Informationen finden Sie im Abschnitt &quot;Neue Standardeinstellungen für Projekte&quot;im Artikel [Projekt erstellen](../../../manage-work/projects/create-projects/create-project.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard </p>
   <p>Aktuell: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme, Aufgaben und Projekte bearbeiten</p> <p>Zugriff auf Finanzdaten bearbeiten , um Finanzinformationen für einen projizierten, aus dem Problem konvertierten Inhalt zu aktualisieren</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Problem anzeigen</p> <p>Sie erhalten nach der Konvertierung des Problems Verwaltungsberechtigungen für das Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Konvertieren eines Problems in ein Projekt

Sie können ein Problem in ein leeres Projekt konvertieren.

1. Wechseln Sie zu einem Projekt und klicken Sie auf **[!UICONTROL Probleme]** im linken Bereich.
1. Führen Sie in der Liste der angezeigten Probleme einen der folgenden Schritte aus:

   * Um ein Problem in ein leeres Projekt zu konvertieren, klicken Sie auf den Namen des Problems und dann auf das **[!UICONTROL Mehr]** Menü ![](assets/more-icon.png) rechts neben dem Problemnamen klicken Sie auf **[!UICONTROL In ein leeres Projekt konvertieren]**.


     Oder

     Wählen Sie das Problem in der Liste der Probleme aus und klicken Sie auf die Schaltfläche **[!UICONTROL Mehr]** Menü ![](assets/more-icon.png) Klicken Sie oben in der Liste auf **[!UICONTROL In ein leeres Projekt konvertieren]**.

     >[!IMPORTANT]
     >
     >Die Option In ein leeres Projekt konvertieren wird nur angezeigt, wenn Ihr System- oder Gruppenadministrator die Option [!UICONTROL Benutzer können Projekte ohne Verwendung einer Vorlage erstellen] Präferenz im [!UICONTROL Einrichtung] Bereich. Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


     Nach der Konvertierung des Problems müssen Sie dem Projekt manuell Aufgaben hinzufügen oder eine Vorlage anhängen.

     >[!TIP]
     >   
     >* Wenn das Problem mit einer Anforderungswarteschlange erstellt wurde, erbt das neue Projekt die Gruppe der Anforderungswarteschlange.
     >* Wenn das Problem durch Hinzufügen zum Abschnitt Probleme des Projekts erstellt wurde, übernimmt das neue Projekt die Gruppe des Projekts.

     >[!TIP]
     >
     >Wenn das Problem mit einem Genehmigungsprozess verknüpft ist oder bereits mit einem aufgelösten Objekt verknüpft ist, zeigt Workfront oben im Feld In Projekt konvertieren eine Warnung an, um Sie darüber zu informieren, dass die Genehmigung entfernt oder das aufgelöste Objekt bei der Konvertierung überschrieben wird. Weitere Informationen finden Sie unter [Übersicht über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Optional und bedingt) Klicken Sie auf [!UICONTROL **Optionen**] Wählen Sie im linken Bereich eine der verfügbaren Optionen aus:

   * [!UICONTROL **Behalten Sie das ursprüngliche Problem bei und binden Sie die Lösung an dieses Projekt**]

     Wenn diese Option deaktiviert ist, wird das ursprüngliche Problem gelöscht.

     >[!NOTE]
     >
     >Benutzer ohne Zugriff oder Berechtigung zum Löschen von Problemen können das Problem beim Konvertieren nicht löschen, unabhängig vom Status dieser Einstellung. Informationen zum Zugriff auf und zu Berechtigungen für Probleme finden Sie unter:
     >
     >* [Zugriff auf Probleme gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [Problem freigeben](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **Zugriff auf dieses Projekt zulassen (Benutzername)**]

     Wenn die Option nicht ausgewählt ist, wird das Problem [!UICONTROL Primärer Kontakt] hat keinen Zugriff auf die neue Aufgabe.

     >[!NOTE]
     >
     >Die hier verfügbaren Optionen hängen davon ab, wie der Workfront-Administrator sie für alle Benutzer im System oder für Ihre Gruppe konfiguriert hat. Weitere Informationen finden Sie unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >Oder wenn die Gruppen der obersten Ebene in Ihrer Organisation sie separat konfiguriert haben, hängen die hier verfügbaren Optionen davon ab, welche Gruppe Sie in Schritt 6 für das neue Projekt ausgewählt haben. Weitere Informationen finden Sie unter [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. Klicks [!UICONTROL **Benutzerdefinierte Forms**] und führen Sie einen der folgenden Schritte aus:

   * Überprüfen Sie die benutzerdefinierten Formulare, die an das Problem angehängt sind. Sie werden in das neue Projekt übertragen, wenn es sich auch um benutzerdefinierte Formulare für Projekte handelt.
   * Weitere benutzerdefinierte Formulare hinzufügen
   * Stellen Sie sicher, dass alle erforderlichen Felder über gültige Informationen verfügen.
   * Ordnen Sie die benutzerdefinierten Formulare durch Ziehen neu an. ![](assets/drag-object-icon.png) wo Sie sie haben wollen.
   * Klicken Sie auf **x** rechts neben allen Formularen, die Sie nicht in das Projekt übertragen möchten. Dadurch wird das Formular aus dem Projekt entfernt.
   * Falls nötig, übertragen Sie benutzerdefinierte Formulardaten vom Problem an das Projekt.

     >[!TIP]
     >
     >* Wenn ein benutzerdefiniertes Formular mit mehreren Objekten, das an das Problem angehängt ist, für die Verwendung sowohl mit Problemen als auch mit Projekten konfiguriert ist, werden alle im Formular gespeicherten Informationen bei der Konvertierung beibehalten, wenn sowohl die Felder für das Problem als auch die benutzerdefinierten Formulare des Projekts vorhanden sind.
     >* Wenn ein benutzerdefiniertes Formular mit mehreren Objekten und einem berechneten Feld an das Problem sowie an das Projekt angehängt ist, müssen das Problem und das Projekt mit allen Feldern kompatibel sein, auf die in den berechneten benutzerdefinierten Feldern des Formulars verwiesen wird. Wenn eine Inkompatibilität vorliegt, werden Sie durch eine Meldung darauf hingewiesen, dass Sie Anpassungen vornehmen müssen. Weitere Informationen finden Sie im Abschnitt &quot;Berechnete benutzerdefinierte Felder in benutzerdefinierten Formularen mit mehreren Objekten&quot;im [Hinzufügen berechneter Daten zu einem benutzerdefinierten Formular mit dem Legacy-Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

1. Klicks [!UICONTROL **In Projekt konvertieren**].

   >[!TIP]
   >
   >Wenn Sie sich entschieden haben, das ursprüngliche Problem zu löschen, handelt es sich jetzt um ein Projekt.
   >   
   >Oder
   >  
   >Wenn Sie sich entschieden haben, das ursprüngliche Problem beizubehalten, ist das Problem jetzt mit dem neuen Projekt verknüpft und wird nach Abschluss des Projekts abgeschlossen.
   >
   >Informationen in einigen Problemfeldern werden an das Projekt übertragen, wenn Sie sie während der Konvertierung nicht geändert haben.

1. (Optional) Legen Sie bei Bedarf weitere Projektdetails &#x200B; (Projekteigentümer, Projektzeitpunkt) und Aufgaben fest.
1. Klicks [!UICONTROL **In Projekt konvertieren**].

   Das Problem wird jetzt in ein Projekt umgewandelt. Die Projektseite wird angezeigt.

## Konvertieren eines Problems in ein Projekt mithilfe einer Vorlage

Sie können ein Problem mithilfe einer Vorlage in ein Projekt konvertieren.

1. Wechseln Sie zu einem Projekt und klicken Sie auf **[!UICONTROL Probleme]** im linken Bereich.
1. Klicken Sie in der angezeigten Liste der Probleme auf den Namen des Problems und anschließend auf die Schaltfläche **[!UICONTROL Mehr]** Menü ![](assets/more-icon.png) rechts neben dem Problemnamen klicken Sie auf **In Projekt aus Vorlage konvertieren** und beginnen Sie mit der Eingabe des Namens einer Vorlage im **Suchvorlage** und dann auf den Namen der Vorlage klicken, wenn sie in der Liste angezeigt wird. Fahren Sie mit Schritt 3 fort.

   >[!TIP]
   >
   >Wenn Sie der Favoritenliste Vorlagen hinzugefügt haben, können Sie mit dem Mauszeiger über die [!UICONTROL **Favoritenvorlagen**] und klicken Sie auf die gewünschte Vorlage.

   Das Feld Neues Projekt aus Vorlage wird angezeigt.

   ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

   >[!TIP]
   >
   >* Wenn das Problem mit einem Genehmigungsprozess verknüpft ist oder bereits mit einem aufgelösten Objekt verknüpft ist, zeigt Workfront oben im Feld In Projekt konvertieren eine Warnung an, um Sie darüber zu informieren, dass die Genehmigung entfernt oder das aufgelöste Objekt bei der Konvertierung überschrieben wird. Weitere Informationen finden Sie unter [Übersicht über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).
   >   
   >* Wenn das Problem mit einer Anforderungswarteschlange erstellt wurde, erbt das neue Projekt die Gruppe der Anforderungswarteschlange.
   >* Wenn das Problem durch Hinzufügen zum Abschnitt Probleme des Projekts erstellt wurde, übernimmt das neue Projekt die Gruppe des Projekts.

1. Überprüfen Sie die Vorlagendetails auf der rechten Seite.

   Die Vorlagendetails umfassen Folgendes:

   * Vorlagendauer
   * Vorlageninhaber
   * Die Anzahl der Aufgaben auf oberster Ebene, die die Namen der drei wichtigsten Aufgaben enthält
   * Die Anzahl aller Aufgaben in der Vorlage
   * Die Namen der benutzerdefinierten Vorlagen-Formulare

1. (Optional) Bewegen Sie den Mauszeiger über den Namen einer Vorlage und klicken Sie auf **Favoriten** icon ![](assets/favorites-icon-small.png) , um ihn als Favoriten für die zukünftige Verwendung zu kennzeichnen.

   >[!TIP]
   >
   >Sie können bis zu 40 Workfront-Elemente als Favoriten markieren. Dazu gehören Vorlagen und andere Elemente.

1. Klicks [!UICONTROL **Vorlage verwenden**] , um eine Vorlage auszuwählen.

   Die [!UICONTROL In Projekt konvertieren] wird geöffnet.

   ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

1. Wenn ein Feld bereits in der Vorlage ausgefüllt ist, wird das Feld im [!UICONTROL In Projekt konvertieren] ankreuzen. Sie können die vorausgefüllten Werte bearbeiten, um sie besser an Ihr Projekt anzupassen. Weitere Informationen finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!TIP]
   >
   >* Ihr System- oder Gruppenadministrator kann Felder in der [!UICONTROL In Projekt konvertieren, Feld] durch Aktualisierung der Projektinformationen in Ihrer [!UICONTROL Layout-Vorlage].
   >
   >* So aktualisieren Sie die Felder in [!UICONTROL Finanzen] im Abschnitt [!UICONTROL In Projekt konvertieren] müssen Sie [!UICONTROL Bearbeiten] Zugriff auf [!UICONTROL Finanzdaten] in Ihrer Zugriffsstufe. Wenn Sie [!UICONTROL Ansicht] Zugriff auf [!UICONTROL Finanzdaten] in Ihrer Zugriffsebene werden alle Finanzinformationen aus der Vorlage an das neue Projekt übertragen und Sie können sie beim Konvertieren des Problems nicht bearbeiten. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) und [Vorlage freigeben](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Optional und bedingt) Klicken Sie auf [!UICONTROL **Optionen**] Wählen Sie im linken Bereich eine der verfügbaren Optionen aus:

   * [!UICONTROL **Behalten Sie das ursprüngliche Problem bei und binden Sie die Lösung an dieses Projekt**]

     Wenn diese Option deaktiviert ist, wird das ursprüngliche Problem gelöscht.

     >[!NOTE]
     >
     >Benutzer ohne Zugriff oder Berechtigung zum Löschen von Problemen können das Problem beim Konvertieren nicht löschen, unabhängig vom Status dieser Einstellung. Informationen zum Zugriff auf und zu Berechtigungen für Probleme finden Sie unter:
     >
     >* [Zugriff auf Probleme gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [Problem freigeben](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **Zugriff auf dieses Projekt zulassen (Benutzername)**]

     Wenn die Option nicht ausgewählt ist, wird das Problem [!UICONTROL Primärer Kontakt] hat keinen Zugriff auf die neue Aufgabe.

     >[!NOTE]
     >
     >Die hier verfügbaren Optionen hängen davon ab, wie der Workfront-Administrator sie für alle Benutzer im System oder für Ihre Gruppe konfiguriert hat. Weitere Informationen finden Sie unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >Oder wenn die Gruppen der obersten Ebene in Ihrer Organisation sie separat konfiguriert haben, hängen die hier verfügbaren Optionen davon ab, welche Gruppe Sie in Schritt 6 für das neue Projekt ausgewählt haben. Weitere Informationen finden Sie unter [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   1. Klicks [!UICONTROL **Benutzerdefinierte Forms**] und führen Sie einen der folgenden Schritte aus:

      * Überprüfen Sie die benutzerdefinierten Formulare, die an die Vorlage angehängt sind. Sie werden auf das neue Projekt übertragen.
      * Überprüfen Sie die benutzerdefinierten Formulare, die an das Problem angehängt sind. Sie werden auf das Projekt übertragen, wenn es sich auch um Projektformulare handelt.
      * Stellen Sie sicher, dass alle erforderlichen Felder über gültige Informationen verfügen.
      * Ordnen Sie die benutzerdefinierten Formulare durch Ziehen neu an. ![](assets/drag-object-icon.png) wo Sie sie haben wollen.
      * Klicken Sie auf **x** rechts neben allen Formularen, die Sie nicht in das Projekt übertragen möchten.
      * Falls nötig, übertragen Sie benutzerdefinierte Formulardaten vom Problem an das Projekt.

        >[!TIP]
        >
        >* Wenn ein benutzerdefiniertes Formular mit mehreren Objekten, das an das Problem angehängt ist, für die Verwendung sowohl mit Problemen als auch mit Projekten konfiguriert ist, werden alle im Formular gespeicherten Informationen bei der Konvertierung beibehalten, wenn sowohl die Felder für das Problem als auch die benutzerdefinierten Formulare des Projekts vorhanden sind.
        >* Wenn ein benutzerdefiniertes Formular mit mehreren Objekten und einem berechneten Feld an das Problem sowie an das Projekt angehängt ist, müssen das Problem und das Projekt mit allen Feldern kompatibel sein, auf die in den berechneten benutzerdefinierten Feldern des Formulars verwiesen wird. Wenn eine Inkompatibilität vorliegt, werden Sie durch eine Meldung darauf hingewiesen, dass Sie Anpassungen vornehmen müssen. Weitere Informationen finden Sie im Abschnitt &quot;Berechnete benutzerdefinierte Felder in benutzerdefinierten Formularen mit mehreren Objekten&quot;im [Hinzufügen berechneter Daten zu einem benutzerdefinierten Formular mit dem Legacy-Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
        >* Wenn ein benutzerdefiniertes Formular, das an die Vorlage angehängt ist, ein benutzerdefiniertes Feld enthält, das auch in einem benutzerdefinierten Formular enthalten ist, das an das Problem angehängt ist, wird der Feldwert aus dem Problem für das neue Projekt verwendet. Wenn das benutzerdefinierte Feld bei dem Problem jedoch leer ist, wird der Wert aus der Vorlage verwendet.

1. (Optional) Legen Sie bei Bedarf weitere Projektdetails &#x200B; (Projekteigentümer, Projektzeitpunkt) und Aufgaben fest.

   1. Klicks [!UICONTROL **In Projekt konvertieren**].

      >[!TIP]
      >
      >Wenn Sie sich entschieden haben, das ursprüngliche Problem zu löschen, handelt es sich jetzt um ein Projekt.
      >   
      >Oder
      >  
      >Wenn Sie sich entschieden haben, das ursprüngliche Problem beizubehalten, ist das Problem jetzt mit dem neuen Projekt verknüpft und wird nach Abschluss des Projekts abgeschlossen.
      >
      >Einige Problemfelder werden an das Projekt übertragen. Die meisten in der Vorlage definierten Felder werden automatisch in das neu erstellte Projekt übertragen, wenn Sie sie in vorherigen Schritten nicht geändert haben. Weitere Informationen finden Sie unter [Übersicht über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

   Das Problem wird jetzt in ein Projekt umgewandelt. Die Projektseite wird angezeigt.