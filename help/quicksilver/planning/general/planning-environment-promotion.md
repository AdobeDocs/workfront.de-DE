---
title: Verwenden der Umgebungsförderung für die Adobe Workfront-Planung
description: Sie können Workfront Planning-Arbeitsbereiche, Datensatztypen, Felder und Ansichten mithilfe von Umgebungsförderungsfunktionen von einer Workfront-Umgebung in eine andere kopieren. Anstatt alles manuell neu zu erstellen, stellen Sie die Konfiguration in einem Paket in der Quellumgebung zusammen und installieren Sie es in der Zielumgebung.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 00706e8c7ed590cf112f4817da9740a970a4a4b3
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 2%
---

# Verwenden der Umgebungsförderung für die Adobe Workfront-Planung

<!--add to TOC-->
<!--add to miniTOC-->

<!--
Not sure if this bit will ever be needed because this only exists when both Preview and Prod have the features in parity. Features released here always come to both environments at the same time: 

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

<!--if Lilit says this is not for STA, break the intro and specify that; she is checking on this-->

Sie können Workfront Planning-Arbeitsbereiche, Datensatztypen, Felder und Ansichten mithilfe von Umgebungsförderungsfunktionen von einer Workfront-Umgebung in eine andere kopieren.

Anstatt alles manuell neu zu erstellen, stellen Sie die Konfiguration in einem Paket in der Quellumgebung zusammen und installieren Sie es in der Zielumgebung.

Die Verwendung der Umgebungsförderung mit Planning ähnelt der Verwendung für Workfront. Weitere Informationen finden Sie im Abschnitt „Umgebungs-Promotion“ im Artikel [Adobe Workfront-Testumgebungen](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-testing-environments.md).

## Überlegungen zur Verwendung der Umgebungsförderung mit Planning

* Sie müssen ein Workfront-Administrator sein, um die Umgebung für die Promotion verwenden zu können.
* Die folgenden Daten werden über die Umgebungsförderung importiert:

  * Arbeitsbereiche
  * Workspace-Abschnitte
  * Eintragstypen
  * Felder
  * Ansichten
  * Hierarchien
  * Freigabeeinstellungen für alle Objekte
  * Automatisierungen <!--this might not be part of it; Lilit is checking-->
  * Antragsformulare
  * Geschäftsregeln
  * Verbundene Objekte
  * Objekte, von denen der Arbeitsbereich abhängig ist oder für die andere Objekte freigegeben sind, z. B. Gruppe, Teams, Aufgabengebiete. Die folgenden Szenarien sind vorhanden:

    * Wenn in der Zielumgebung bereits ein Objekt mit demselben Namen vorhanden ist, kennzeichnet Workfront einen Konflikt und Sie entscheiden, wie Sie ihn handhaben möchten.
    * Wenn ein Team oder eine Gruppe, für die ein Objekt freigegeben ist, nicht in der Zielumgebung vorhanden ist, wird es bei der Promotion erstellt.
* Für jedes Objekt haben Sie folgende Möglichkeiten:

  * Als neues Objekt erstellen
  * Vorhandenes Objekt verwenden, aber mit einem neuen Namen erstellen
  * Vorhandenes Objekt überschreiben. Das Überschreiben ersetzt die -Konfiguration im Ziel.

* Die Installation kann einige Minuten dauern. Sie können eine Installation bei Bedarf von der Ergebnisseite aus zurücksetzen.
* Es wird empfohlen, den Prozess vor dem Fortfahren zu testen, sofern dies möglich ist. Sie können eine Installation in einer Sandbox- oder Vorschau-Umgebung durchführen, bevor Sie sie zur Produktion weiterleiten.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Pakete</p></td> 
   <td> 
<p>Prime- oder Ultimate-Workflow-Paket mit einem Prime- oder Ultimate-Planungspaket</p>
<p>Prime- oder Ultimate-Planungspaket beim Kauf als eigenständiges Produkt</p>
   </td> 
   </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Workflow-Standard</p>    
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Planungsgenehmigung</p></td> 
   <td><p>Planungsstandard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Sie müssen der Zugriffsebene sowohl einen Workflow- als auch einen Planning-Lizenztyp hinzufügen, wenn Sie sowohl einen Workflow als auch ein Planning-Paket haben</p>  
   <p>Sie müssen Systemadministrator sein</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für Arbeitsbereiche</p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  
   </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Importieren der Planungskonfiguration mithilfe der Umgebungsförderung

Im Folgenden finden Sie die wichtigsten Schritte zur Förderung der Planungskonfiguration in einer anderen Umgebung:

* [Erstellen Sie ein Paket in der Quellumgebung](#create-a-package-in-the-source-environment)
* [Package zur Installation vorbereiten](#make-the-package-ready-to-install)
* [Installieren des Pakets in der Zielumgebung](#install-the-package-in-the-target-environment)
* [Überprüfen der Ergebnisse](#verify-the-results)

Befolgen Sie die Anweisungen in den folgenden Abschnitten, um eine Planning-Konfiguration zwischen zwei Workfront-Umgebungen zu kopieren.

### Erstellen eines Pakets in der Quellumgebung

1. Verwenden Sie eine Quellumgebung, in der Ihre gewünschte Konfiguration vorhanden ist.
1. Klicken Sie in der Quellumgebung auf das **Hauptmenü** ![Hauptmenü](assets/main-menu-shell.png) und gehen Sie dann zu **Setup** > **System** > **Umgebungsförderung**.
Die Liste **Konfigurationspakete** zeigt vorhandene Pakete mit ihrem Status, ihrer Quellumgebung und dem Ort ihrer Bereitstellung an.
1. Klicken Sie **Paket erstellen**.

   >[!TIP]
   >
   >Ein Paket benötigt mindestens ein Objekt, bevor es zusammengestellt und installiert werden kann.
1. Geben Sie auf der Registerkarte **Paketdetails** einen **Namen** und eine **Beschreibung** für das Paket ein. Die Quellumgebung ist bereits mit der aktuellen Umgebung (Quelle) ausgefüllt.
1. Wählen Sie in der Liste der Objekttypen auf der linken Seite **Planning Workspace** aus.
1. Suchen Sie nach dem Arbeitsbereich, den Sie weiterleiten möchten, aktivieren Sie das entsprechende Kontrollkästchen und klicken Sie auf **Arbeitsbereich hinzufügen**. Der Arbeitsbereich wird unter **Paketinhalt** angezeigt.

   ![Workspace für die Umgebungsförderung ausgewählt](assets/workspace-selected-for-environment-promotion.png)
1. Klicken Sie **Speichern und zusammenführen**.

   Workfront stellt das Paket zusammen und fügt einen Eintrag auf der Registerkarte **Updates** des Pakets hinzu. Was das Paket enthält, können Sie auf der Registerkarte Inhalt überprüfen.
1. (Bedingt und optional) Klicken Sie stattdessen auf **Speichern und schließen**, wenn Sie den Vorgang später abschließen möchten.
1. (Optional) Klicken Sie auf **Inhalte**, um den Inhalt des Pakets zu überprüfen, oder klicken Sie auf **Bereitstellungen**, um festzustellen, ob dieses Paket mehrmals bereitgestellt wurde.

   Fahren Sie mit der Installation fort.

### Package zur Installation vorbereiten

Vor der Installation des Pakets in der Zielumgebung wird empfohlen, es in einer Testumgebung zu testen.

1. Nachdem das Paket wie im vorherigen Abschnitt beschrieben erstellt wurde, klicken Sie auf **Paketdetails** und klicken Sie auf **Bearbeiten**, setzen Sie **Status** auf **Testing** und klicken Sie dann auf **Speichern und schließen**.

   >[!TIP]
   >
   >Nach der Erstellung des Pakets wird sein Status auf &quot;**&quot;**. Der **Aktiv**-Status ist erst verfügbar, nachdem Sie das Paket zuvor getestet haben.
1. (Empfohlen) Klicken Sie auf **Installieren** und wählen Sie eine der verfügbaren Testumgebungen aus, um sie dort bereitzustellen und die Konfiguration zu testen.

   >[!TIP]
   >
   >Die Produktionsumgebung ist nicht als eine der Optionen verfügbar, wenn der Status auf „Testen **festgelegt**.

1. Klicken Sie nach der Installation in einer Testumgebung erneut auf **Bearbeiten** und legen Sie **Status** auf **Aktiv** fest. Klicken Sie dann auf **Speichern und schließen**.

   >[!TIP]
   >
   >Die Installation des Pakets in einer Testumgebung ähnelt der Installation in der Produktionsumgebung, wie im folgenden Abschnitt beschrieben.

   Fahren Sie mit dem folgenden Abschnitt fort, um das Paket in Ihrer Zielumgebung zu installieren.


### Installieren des Pakets in der Zielumgebung

1. Klicken Sie auf der Paketseite nach der Überprüfung auf **Installieren**.
1. Wählen Sie in **Liste** Zielumgebung“ die Umgebung aus, für die die Bereitstellung erfolgen soll (z. B. Ihre Produktionsumgebung), und klicken Sie auf **Weiter**. Das Standardziel ist die aktuelle Umgebung.
1. Bestätigen Sie auf der **Paketinformationen** die Quellumgebung und die Umgebung, in der Sie bereitstellen.
1. Erweitern Sie im Abschnitt **Objektzuordnung** jede Objektgruppierung, z. B. **Gruppe** und **Planning Workspace**, um die Objekte zu überprüfen.
1. Überprüfen Sie für jedes Objekt die Spalten **Kollision** und **Status** und wählen Sie dann eine **Bereitstellungsaktion** aus der Liste aus. Wählen Sie aus den folgenden Optionen:

   * **Neu erstellen**: Fügt das Objekt zum Ziel hinzu. Verwenden Sie diese Option, wenn keine Kollision erkannt wird.
   * **Use existing**: Ordnet das Objekt einem Objekt zu, das bereits im Ziel vorhanden ist, z. B. einer Gruppe mit demselben Namen.
   * **Mit neuem Namen erstellen**: Fügt das Objekt unter einem von Ihnen angegebenen Namen hinzu.
   * **Überschreiben**: Ersetzt das vorhandene Objekt im Ziel durch das Objekt aus dem Paket.
1. (Optional) Um mehrere Objekte gleichzeitig zu ändern, aktivieren Sie die entsprechenden Kontrollkästchen, wählen Sie eine Aktion in der Liste Bereitstellungsaktion oben in der Gruppe aus und klicken Sie auf Auf ausgewählte anwenden. Verwenden Sie die Filter oberhalb der Liste, z. B. Nur Fehler anzeigen , um den Fokus auf bestimmte Objekte zu legen.
1. Beheben Sie alle Fehlerindikatoren. Wenn Sie für **Objekt „Vorhandenes verwenden** auswählen, müssen Sie auch das Objekt auswählen, dem es zugeordnet ist.  Andernfalls wird im Status ein Fehler angezeigt und **Bereitstellen** bleibt nicht verfügbar.
1. Klicken Sie **Bereitstellen** und dann **Bereitstellen** zur Bestätigung.

   Workfront zeigt eine Installationsseite mit der Meldung **Dieses Paket wird installiert** an. Dies kann einige Minuten dauern.

   Nach Abschluss der Installation zeigt die Seite eine Erfolgsmeldung, die Umgebung, in der das Paket installiert wurde, und eine Liste der installierten Objekte mit jeweils einem Status wie **Verwendet vorhanden** oder **Installiert (Neu erstellen)**.
1. (Optional) Klicken Sie auf **Installation zurücksetzen**, falls erforderlich, um die Installation rückgängig zu machen und die Konfiguration aus der Zielumgebung zu entfernen.

   Überprüfen Sie die Installationsergebnisse.

### Überprüfen der Ergebnisse

1. Gehen Sie zur Zielumgebung > **Hauptmenü** > **Planung** und suchen Sie den importierten Arbeitsbereich.
1. Öffnen Sie die Datensatztypen und -ansichten, um zu bestätigen, dass die Felder und das Layout mit der Quelle übereinstimmen. Die Datensätze sind nicht enthalten, sodass die Tabellen leer sind.


