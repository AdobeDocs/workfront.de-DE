---
title: Alle Berichte anzeigen, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden
description: Sie können eine benutzerdefinierte Ansicht im Bereich "Benutzerdefinierter Forms"hinzufügen, die anzeigt, welche Berichte ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden. Dies ist nützlich, wenn Sie das Feld oder Widget bearbeiten oder löschen müssen, da es möglicherweise bereits in einem oder mehreren Berichten implementiert ist. Es ist wichtig zu beurteilen, ob diese Berichte angepasst werden müssen, damit sie weiterhin ordnungsgemäß funktionieren.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# Alle Berichte anzeigen, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden

Sie können eine benutzerdefinierte Ansicht im Bereich &quot;Benutzerdefinierter Forms&quot;hinzufügen, die anzeigt, welche Berichte ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden. Dies ist nützlich, wenn Sie das Feld oder Widget bearbeiten oder löschen müssen, da es möglicherweise bereits in einem oder mehreren Berichten implementiert ist. Es ist wichtig zu beurteilen, ob diese Berichte angepasst werden müssen, damit sie weiterhin ordnungsgemäß funktionieren.

Weitere Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Abo</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Berichte auflisten, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms**.
1. Klicken Sie auf **Felder** , um einen Bericht anzuzeigen, in dem alle benutzerdefinierten Felder und Widgets in Ihrer Workfront-Instanz aufgelistet sind.

1. Klicken Sie auf das Menü **Ansicht** und suchen Sie dann nach benutzerdefinierten Ansichten in der Liste, die die Spalte **Berichte** enthalten (dies ist keine Standardspalte auf dieser Registerkarte).

   In der Spalte Berichte können Sie sehen, welche Berichte die einzelnen benutzerdefinierten Felder und Widgets verwenden, die zu einem benutzerdefinierten Formular in Ihrem System hinzugefügt wurden. Es ist möglich, dass bereits eine Ansicht erstellt wurde, die die Spalte **Berichte** enthält.

1. Wenn keine Ansicht angezeigt wird, die die Spalte **Berichte** enthält, erstellen Sie eine neue Ansicht, die diese enthält:

   1. Klicken Sie auf das Menü **Ansicht** und dann auf **Neue Ansicht**.

   1. Ersetzen Sie auf der angezeigten Seite **Neue Ansicht** im Feld links oben die Option **Neue Parameteransicht** durch einen beschreibenden Namen für die Ansicht, z. B. *Felder und Widgets*.

   1. Klicken Sie unten rechts auf **Spalte hinzufügen**.
   1. Geben Sie in das Feld **In dieser Spalte anzeigen** oben links den Wert *report* ein und wählen Sie dann **Reports** aus, wenn es in der Liste unter dem Feld angezeigt wird.

   1. (Bedingt) Wenn Sie die gerade hinzugefügte Spalte **Berichte** an eine andere horizontale Position verschieben möchten, ziehen Sie die Kopfzeile in den Bereich **Spaltenvorschau** am unteren Rand der Seite.

   1. Klicken Sie auf **Fertig** und dann auf **Ansicht speichern**.

1. Klicken Sie auf das Dropdownmenü **Ansicht** und wählen Sie dann den Namen der soeben erstellten benutzerdefinierten Ansicht aus.
1. Suchen Sie in der Spalte **Name** das benutzerdefinierte Feld oder Widget, das Sie bearbeiten oder löschen möchten, und sehen Sie sich dann die Spalte **Berichte** in dieser Zeile an, um zu sehen, welche Berichte es verwenden (falls vorhanden).

   Um die Informationen für diese Spalte zu finden, sucht Workfront in allen Berichtsfiltern, Ansichten und Gruppierungen nach den benutzerdefinierten Feldern und Widgets.

   Wenn ein Pluszeichen angezeigt wird, können Sie auf diese Textzeile klicken, um ein Feld mit allen weiteren Berichten anzuzeigen, die das Feld oder Widget verwenden.

   >[!NOTE]
   >
   >Die anfängliche Ladezeit für dieses Tool kann je nach Datenmenge in Ihrem System zwischen 10 und 2,5 Minuten dauern.

   >[!TIP]
   >
   >Wenn Sie keine Zeit haben, die Berichte zu untersuchen, die das benutzerdefinierte Feld oder Widget verwenden, können Sie auf Exportieren klicken, um eine Datei zu erstellen, in der diese aufgelistet sind. Sie können diese Datei mit allen Personen teilen, die Eigentümer eines Berichts sind, der das Feld oder Widget verwendet, und die notwendigen Änderungen, die möglichen Auswirkungen auf den Bericht und die erforderlichen Maßnahmen besprechen, um sicherzustellen, dass der Bericht weiterhin ordnungsgemäß funktioniert.
   >
   >Diese Ansicht ist auch in einem Parameterbericht verfügbar:
   >      
   > 1. Klicken Sie im Hauptmenü auf **Berichte**.
   > 1. Klicken Sie in der linken oberen Ecke auf **Neuer Bericht** und klicken Sie dann in der angezeigten Liste auf **Parameter** .
   > 1. Klicken Sie unten rechts auf **Spalte hinzufügen**.
   > 1. Geben Sie in das Feld **In dieser Spalte anzeigen** oben links den Wert *report* ein und wählen Sie dann **Reports** aus, wenn es in der Liste unter dem Feld angezeigt wird.
   > 1. (Bedingt) Wenn Sie die gerade hinzugefügte Spalte **Berichte** an eine andere horizontale Position verschieben möchten, ziehen Sie die Kopfzeile in den Bereich **Spaltenvorschau** am unteren Rand der Seite.
   > 1. Klicken Sie auf **Fertig** und dann auf **Speichern+Schließen**.
   > 1. Geben Sie einen beschreibenden Namen für den Bericht ein, z. B. *Felder und Widgets*.
