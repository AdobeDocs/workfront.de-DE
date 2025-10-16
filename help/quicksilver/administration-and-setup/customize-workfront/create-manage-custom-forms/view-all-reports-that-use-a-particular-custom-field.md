---
title: Alle Berichte anzeigen, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden
description: Sie können im Bereich Benutzerdefinierte Forms eine benutzerdefinierte Ansicht hinzufügen, die anzeigt, welche Berichte ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden. Dies ist nützlich, wenn Sie das Feld oder Widget bearbeiten oder löschen müssen, da es möglicherweise bereits in einem oder mehreren Berichten implementiert ist. Es ist wichtig zu beurteilen, ob diese Berichte angepasst werden müssen, damit sie weiterhin ordnungsgemäß funktionieren.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 15ac51cc13eeb57d2de194a9a6ceec7683acfbe6
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Alle Berichte anzeigen, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden

Sie können im Bereich Benutzerdefinierte Forms eine benutzerdefinierte Ansicht hinzufügen, die anzeigt, welche Berichte ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden. Dies ist nützlich, wenn Sie das Feld oder Widget bearbeiten oder löschen müssen, da es möglicherweise bereits in einem oder mehreren Berichten implementiert ist. Es ist wichtig zu beurteilen, ob diese Berichte angepasst werden müssen, damit sie weiterhin ordnungsgemäß funktionieren.

Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Administrativer Zugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Auflisten der Berichte, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Benutzerdefinierte Forms**.
1. Klicken Sie **Felder**, um einen Bericht anzuzeigen, in dem alle benutzerdefinierten Felder und Widgets in Ihrer Workfront-Instanz aufgelistet sind.

1. Klicken Sie auf **Ansicht** und suchen Sie dann nach benutzerdefinierten Ansichten in der Liste, die die Spalte **Berichte** enthalten (die auf dieser Registerkarte keine Standardspalte ist).

   In der Spalte Berichte können Sie sehen, welche Berichte jedes benutzerdefinierte Feld und Widget verwenden, das zu einem benutzerdefinierten Formular in Ihrem System hinzugefügt wurde. Es ist möglich, dass bereits eine Ansicht erstellt wurde, die die Spalte **Berichte** enthält.

1. Wenn keine Ansicht angezeigt wird, die die Spalte **Berichte** enthält, erstellen Sie eine neue Ansicht, die diese enthält:

   1. Klicken Sie auf **Ansicht** Menü und dann auf **Neue Ansicht**.

   1. Ersetzen Sie auf der **Neue Ansicht** Seite, die im Feld links oben angezeigt wird, **Neue Parameteransicht** durch einen beschreibenden Namen für die Ansicht, z. B. &quot;*und Widgets*.

   1. Klicken Sie **Spalte hinzufügen** unten rechts.
   1. Beginnen Sie im Feld **In dieser Spalte anzeigen** das oben links angezeigt wird, mit der Eingabe von *Bericht* und wählen Sie dann **Berichte** aus, wenn es in der Liste unter dem Feld angezeigt wird.

   1. (Bedingt) Wenn Sie die soeben hinzugefügte Spalte **Berichte** in eine andere horizontale Position verschieben möchten, ziehen Sie ihre Kopfzeile in den Bereich **Spaltenvorschau** am unteren Seitenrand.

   1. Klicken Sie **Fertig** und dann auf **Ansicht speichern**.

1. Klicken Sie auf **Dropdown** Menü „Ansicht“ und wählen Sie dann den Namen der soeben erstellten benutzerdefinierten Ansicht aus.
1. Suchen Sie in **Spalte** Name“ das benutzerdefinierte Feld oder Widget, das Sie bearbeiten oder löschen möchten, und sehen Sie sich dann die Spalte **Berichte** in dieser Zeile an, um festzustellen, welche Berichte es verwenden.

   Um die Informationen für diese Spalte zu finden, sucht Workfront in allen Berichtsfiltern, Ansichten und Gruppierungen nach den benutzerdefinierten Feldern und Widgets.

   Wenn ein Pluszeichen angezeigt wird, können Sie auf diese Textzeile klicken, um ein Feld anzuzeigen, in dem alle zusätzlichen Berichte aufgelistet sind, die das Feld oder Widget verwenden.

   >[!NOTE]
   >
   >Die anfängliche Ladezeit für dieses Tool kann je nach Datenmenge in Ihrem System zwischen 10 Sekunden und 2,5 Minuten dauern.

   >[!TIP]
   >
   >Wenn Sie keine Zeit haben, die Berichte zu untersuchen, die das benutzerdefinierte Feld oder Widget verwenden, können Sie auf Exportieren klicken, um eine Datei zu erstellen, die sie auflistet. Sie können diese Datei für alle Personen freigeben, denen ein Bericht gehört, der das Feld oder Widget verwendet, und die erforderlichen Änderungen, die Auswirkungen, die sie auf den Bericht haben können, und die Maßnahmen besprechen, die erforderlich sind, um sicherzustellen, dass der Bericht weiterhin ordnungsgemäß funktioniert.
   >
   >Diese Ansicht ist auch in einem Parameterbericht verfügbar:
   >      
   > 1. Klicken Sie im Hauptmenü auf **Berichte**.
   > 1. Klicken Sie in der oberen linken Ecke auf **Neuer Bericht** und klicken Sie dann in der **angezeigten Liste auf** Parameter.
   > 1. Klicken Sie **Spalte hinzufügen** unten rechts.
   > 1. Beginnen Sie im Feld **In dieser Spalte anzeigen** das oben links angezeigt wird, mit der Eingabe von *Bericht* und wählen Sie dann **Berichte** aus, wenn es in der Liste unter dem Feld angezeigt wird.
   > 1. (Bedingt) Wenn Sie die soeben hinzugefügte Spalte **Berichte** in eine andere horizontale Position verschieben möchten, ziehen Sie ihre Kopfzeile in den Bereich **Spaltenvorschau** am unteren Seitenrand.
   > 1. Klicken Sie **Fertig** und dann auf **Speichern+Schließen**.
   > 1. Geben Sie einen beschreibenden Namen für den Bericht ein, z. B. *Felder und Widgets*.
