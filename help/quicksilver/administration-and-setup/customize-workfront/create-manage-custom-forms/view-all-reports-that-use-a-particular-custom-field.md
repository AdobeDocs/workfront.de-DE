---
title: Alle Berichte anzeigen, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden
description: Sie können eine benutzerdefinierte Ansicht im Bereich "Benutzerdefinierter Forms"hinzufügen, die anzeigt, welche Berichte ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden. Dies ist nützlich, wenn Sie das Feld oder Widget bearbeiten oder löschen müssen, da es möglicherweise bereits in einem oder mehreren Berichten implementiert ist. Es ist wichtig zu beurteilen, ob diese Berichte angepasst werden müssen, damit sie weiterhin ordnungsgemäß funktionieren.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Alle Berichte anzeigen, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden

Sie können eine benutzerdefinierte Ansicht im Bereich &quot;Benutzerdefinierter Forms&quot;hinzufügen, die anzeigt, welche Berichte ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden. Dies ist nützlich, wenn Sie das Feld oder Widget bearbeiten oder löschen müssen, da es möglicherweise bereits in einem oder mehreren Berichten implementiert ist. Es ist wichtig zu beurteilen, ob diese Berichte angepasst werden müssen, damit sie weiterhin ordnungsgemäß funktionieren.

Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) und [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> <p>Informationen dazu, wie Workfront-Administratoren diesen Zugriff gewähren, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welche Konfigurationen für Plan, Lizenztyp oder Zugriffsstufe Sie verwenden.

## Berichte auflisten, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Benutzerdefinierte Forms**.
1. Öffnen Sie die **Felder** um einen Bericht anzuzeigen, der alle benutzerdefinierten Felder und Widgets in Ihrer Workfront-Instanz auflistet.

   ![](assets/fields-tab.png)

1. Klicken Sie auf **Ansicht** Dropdown-Menü in der Kopfzeile am oberen Rand der Liste und suchen Sie dann nach benutzerdefinierten Ansichten in der Liste, die die **Berichte** -Spalte (keine Standardspalte auf dieser Registerkarte).

   In der Spalte Berichte können Sie sehen, welche Berichte die einzelnen benutzerdefinierten Felder und Widgets verwenden, die zu einem benutzerdefinierten Formular in Ihrem System hinzugefügt wurden. Es ist möglich, dass jemand bereits eine Ansicht erstellt hat, die Folgendes enthält: **Berichte** Spalte.

1. Wenn keine Ansicht angezeigt wird, die die **Berichte** erstellen Sie eine neue Ansicht, die Folgendes enthält:

   1. Klicken Sie auf **Ansicht** Dropdown-Menü, und klicken Sie auf **Neue Ansicht**.

   1. Im **Neue Ansicht** Seite, die angezeigt wird, ersetzen Sie im Feld links oben **Neue Parameteransicht** mit einem beschreibenden Namen für die Ansicht, z. B. *Felder und Widgets*.

   1. Klicks **Spalte hinzufügen** in der rechten unteren Ecke.
   1. Im **In dieser Spalte anzeigen** in der Nähe der oberen linken Ecke angezeigt wird, beginnen Sie mit der Eingabe. *Bericht*, wählen Sie **Berichte** , wenn sie in der Liste unter dem Feld angezeigt wird.

   1. (Bedingt) Wenn Sie die **Berichte** -Spalte, die Sie gerade zu einer anderen horizontalen Position hinzugefügt haben, ziehen Sie die Kopfzeile in **Spaltenvorschau** unten auf der Seite.

   1. Klicks **Fertig** Klicken Sie auf **Ansicht speichern**.

1. Klicken Sie auf **Ansicht** Dropdown-Menü und wählen Sie dann den Namen der soeben erstellten benutzerdefinierten Ansicht aus.
1. Im **Name** -Spalte, das benutzerdefinierte Feld oder Widget suchen, das Sie bearbeiten oder löschen möchten, und dann die **Berichte** in dieser Zeile, um zu sehen, welche Berichte sie verwenden (falls vorhanden).

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
   > 1. Klicken Sie links oben auf **Neuer Bericht** Klicken Sie auf **Parameter** in der Liste, die angezeigt wird.
   > 1. Klicks **Spalte hinzufügen** in der rechten unteren Ecke.
   > 1. Im **In dieser Spalte anzeigen** in der Nähe der oberen linken Ecke angezeigt wird, beginnen Sie mit der Eingabe. *Bericht*, wählen Sie **Berichte** , wenn sie in der Liste unter dem Feld angezeigt wird.
   > 1. (Bedingt) Wenn Sie die **Berichte** -Spalte, die Sie gerade zu einer anderen horizontalen Position hinzugefügt haben, ziehen Sie die Kopfzeile in **Spaltenvorschau** unten auf der Seite.
   > 1. Klicks **Fertig** Klicken Sie auf **Speichern+Schließen**.
   > 1. Geben Sie einen beschreibenden Namen für den Bericht ein, beispielsweise *Felder und Widgets*.
