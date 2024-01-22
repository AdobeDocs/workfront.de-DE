---
product-area: programs
navigation-topic: create and manage programs
title: Programm erstellen
description: Ein Programm stellt eine Sammlung von Projekten dar, die eine gemeinsame Strategie, ein gemeinsames Ziel oder ein gemeinsames Ziel haben, die über Projektgrenzen hinausgehen. Programme können nicht außerhalb eines Portfolios existieren.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 6ec353c2-2241-47c2-8c59-1d8ddc43781e
source-git-commit: e4cd543aa9f47e6b93aa148ea3fb972fbd356c02
workflow-type: tm+mt
source-wordcount: '998'
ht-degree: 0%

---

# Programm erstellen

<!-- Audited: 1/2024 -->

Ein Programm stellt eine Sammlung von Projekten dar, die eine gemeinsame Strategie, ein gemeinsames Ziel oder ein gemeinsames Ziel haben, die über Projektgrenzen hinausgehen. Programme können nicht außerhalb eines Portfolios existieren.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Neu: Beliebig</p><p>Oder</p><p>Aktuell: [!UICONTROL Business] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>Neu: [!UICONTROL Standard] </p><p>Oder </p><p>Aktuell: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>[!UICONTROL Zugriff auf Portfolios und Programme bearbeiten </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL Verwalten] Berechtigungen für das Portfolio</p> <p>Nachdem Sie ein Programm erstellt haben, verfügen Sie standardmäßig über [!UICONTROL Manager] -Berechtigungen.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Programm erstellen

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke.

1. Führen Sie einen der folgenden Schritte aus.

   * Erstellen Sie ein Programm aus dem [!UICONTROL Programme] Bereich:

      1. Klicks **[!UICONTROL Programme]** im Hauptmenü.
      1. Klicks **[!UICONTROL Neues Programm]**.
      1. Geben Sie in das angezeigte Feld den Namen eines vorhandenen Portfolios in das Feld **[!UICONTROL Portfolio auswählen]** -Feld.
      1. Geben Sie den Namen des neuen Programms in die **[!UICONTROL Name]** -Feld.
      1. Klicken Sie auf **[!UICONTROL Speichern]**.
   * Erstellen Sie ein Programm aus dem [!UICONTROL Portfolios] Bereich:

      1. Klicks **[!UICONTROL Portfolios]** im [!UICONTROL Hauptmenü], und öffnen Sie dann ein Portfolio.
      1. Klicken Sie im linken Bereich auf **[!UICONTROL Programme]**.
      1. Klicken Sie auf **[!UICONTROL Neues Programm]** Dropdown-Menü und **[!UICONTROL Neues Programm]**.


1. (Bedingt) Wenn Sie das Programm aus einem Portfolio erstellt haben, geben Sie den Namen für das Programm im **[!UICONTROL Unbenanntes Programm]** -Feld.

   Der Name kann bis zu 255 Zeichen enthalten.

1. (Optional) Klicken Sie auf **[!UICONTROL Programm-Manager]** in der Kopfzeile des Programms, um es zu aktualisieren.

   >[!TIP]
   >
   >Als Ersteller des Programms werden Sie standardmäßig als Programmmanager festgelegt.

1. Klicks **[!UICONTROL Programmdetails]** im linken Bereich.
1. Doppelklicken Sie auf ein beliebiges Feld, um die Informationen im **[!UICONTROL Übersicht]** Bereich.

Sie können die folgenden Informationen angeben:

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Feld</th> 
      <th>Beschreibung</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td> <p>Geben Sie eine Beschreibung für das Programm an.</p> <p>Die Beschreibung wird auf der Landingpage des Programms angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Programm-Manager]</td> 
      <td> <p>Beginnen Sie mit der Eingabe des Namens des Benutzers, der als Programm-Manager fungieren soll, und klicken Sie dann auf den Namen des Benutzers, wenn er in der Dropdownliste angezeigt wird. Dies entspricht dem [!UICONTROL Programmeigentümer]. </p> <p>Tipp: Sie können auch den Programm-Manager im Programmheader aktualisieren. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Group] </td> 
      <td> <p>Fügen Sie den Namen einer einzelnen Gruppe hinzu, wenn die Gruppe Eigentümer des Programms ist oder für dessen Abschluss verantwortlich ist. </p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe auswählen, indem Sie den Mauszeiger darüber bewegen und auf das Symbol [!UICONTROL Information] klicken <img src="assets/info-icon.png"> , das daneben angezeigt wird. Dadurch wird eine QuickInfo mit Informationen zur Gruppe angezeigt, z. B. die Hierarchie der Gruppen darüber und deren Administratoren.</p> 
       <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
        <img src="assets/group-details-widget-programs-350x268.png" style="width: 350;height: 268;"> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional und bedingt) Klicken Sie in die **[!UICONTROL Benutzerdefiniertes Formular hinzufügen]** , um ein benutzerdefiniertes Formular für das Portfolio auszuwählen und die benutzerdefinierten Felder zu aktualisieren.

   >[!TIP]
   >
   >Sie müssen bereits benutzerdefinierte Programmformulare erstellt haben, bevor Sie sie an Programme anhängen können.

1. (Optional und bedingt) Wenn Sie ein benutzerdefiniertes Formular hinzufügen, klicken Sie auf ein beliebiges Feld im benutzerdefinierten Formular, um die Informationen in diesem Feld zu aktualisieren.
1. Klicks **[!UICONTROL Änderungen speichern]**.
1. Klicks **[!UICONTROL Projekte]** im linken Bereich, dann **[!UICONTROL Projekte hinzufügen]** , um dem Programm Projekte hinzuzufügen.

   Weitere Informationen zum Hinzufügen von Projekten zu Programmen finden Sie unter [Hinzufügen eines Projekts zu einem Programm](../../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

1. Klicks **[!UICONTROL Änderungen speichern]**.
1. (Optional) Klicken Sie auf die **[!UICONTROL Mehr Menü]** ![](assets/more-icon.png) neben dem Programmnamen und klicken Sie auf **[!UICONTROL Programm deaktivieren]**.

   Wenn Sie ein Programm deaktivieren, wird das Programm nicht mehr in einer Programmliste angezeigt, wenn Benutzer versuchen, es einem Projekt hinzuzufügen. Der Zugriff auf das Programm erfolgt weiterhin über die [!UICONTROL Programme] Bereich.

## Übersicht über Programm-Header

Sie finden einige Informationen über das Programm in seiner Kopfzeile.

Die folgenden Informationen werden in der Kopfzeile eines Programms angezeigt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Kopfzeileninformationen</td> 
   <td> <strong>Hinweise</strong> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Breadcrumb mit dem Namen des Portfolios</td> 
   <td>Sie können über die Kopfzeile des Programms auf das Portfolio zugreifen, zu dem das Programm gehört. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Name des Programms</td> 
   <td>Sie können den Programmnamen in der Kopfzeile bearbeiten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Name des Objekttyps und Aktivierungsstatus</td> 
   <td>Das Wort "Programm"wird bei der Anzeige eines Programms mit einem orangefarbenen Symbol angezeigt. Das Wort "[!UICONTROL Deaktiviert]" wird daneben angezeigt und der Entwurf ist grau, wenn das Programm nicht als [!UICONTROL aktiv] markiert ist. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aktionsbereich des Programms </td> 
   <td> <p>Klicken Sie auf eine der folgenden Optionen, um weitere Informationen oder Bearbeitungsoptionen für das Programm aufzurufen:</p> 
    <ul> 
     <li>Das Sternsymbol, um das Programm Ihrer Favoritenliste hinzuzufügen</li> 
     <li> <p>Das Menü [!UICONTROL Mehr] <img src="assets/qs-more-menu.png"> um einen der folgenden Schritte auszuführen: </p> 
      <ul> 
       <li>Programm bearbeiten</li> 
       <li>Deaktivieren Sie sie. Wenn ein Programm deaktiviert ist, können Sie es nicht mehr mit Projekten auf Projektebene verknüpfen. </li> 
       <li> <p>Löschen Sie es. Durch das Löschen des Programms werden die im Programm enthaltenen Projekte nicht gelöscht. Dadurch wird die Verknüpfung der Projekte mit dem Programm aufgehoben. </p> </li> 
       <li>Freigeben für andere</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prozentsatz abgeschlossen]</td> 
   <td> <p>Sie können den [!UICONTROL Prozentwert (Complete) des Programms nicht in der Kopfzeile bearbeiten. Diese Informationen werden aus den Projekten des Programms aktualisiert. Standardmäßig entspricht der prozentuale Abschluss des Programms dem Durchschnitt der vollständigen Prozentwerte der Projekte in einem [!UICONTROL Aktuellen] oder [!UICONTROL Genehmigten] Status, die zum Programm gehören.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Programm-Manager]</td> 
   <td> <p>Sie können den Programm-Manager in der Kopfzeile bearbeiten. Dies entspricht dem [!UICONTROL Programmeigentümer]. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Geplantes Abschlussdatum]</td> 
   <td>Das geplante Abschlussdatum des Programms kann nicht in der Kopfzeile bearbeitet werden.  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bedingung für aktive Projekte]</td> 
   <td>Dies ist eine Berechnung des Prozentsatzes der Projekte im Programm, für die die [!UICONTROL Bedingung] als [!UICONTROL On Target], [!UICONTROL At Risk] oder [!UICONTROL In Trouble] festgelegt ist. Die hier vertretenen Projekte sind Projekte mit dem Status [!UICONTROL Aktuell] und [!UICONTROL Genehmigt]. </td> 
  </tr> 
 </tbody> 
</table>

## Verschieben eines Programms

Sie können einem Portfolio vorhandene Programme hinzufügen. Da Programme nicht in zwei verschiedenen Portfolios existieren können, werden sie durch das Hinzufügen eines vorhandenen Programms dauerhaft von einem Portfolio in ein anderes verschoben.

Weitere Informationen finden Sie unter [Hinzufügen eines vorhandenen Programms zu einem Portfolio](../../../manage-work/portfolios/create-and-manage-programs/move-program.md).
