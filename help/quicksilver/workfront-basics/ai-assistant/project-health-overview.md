---
title: Projektstatus - Übersicht
content-type: reference
description: Die Funktion „Projektdiagnose“ nutzt die Leistungsfähigkeit des KI-Assistenten, um Ihnen sofort einen Überblick über die Leistung Ihrer Projekte zu geben.
author: Jenny
feature: Get Started with Workfront
exl-id: e4d200c6-7f35-4919-96d3-2880a655ed62
source-git-commit: 8ece3c614febb6f480b352323721bcc9dcc940b6
workflow-type: tm+mt
source-wordcount: '1969'
ht-degree: 1%

---

# Projektstatus - Übersicht

>[!IMPORTANT]
>
>Die Funktion Projektdiagnose ist derzeit nur für Benutzer verfügbar, die an der Beta-Phase teilnehmen.

Die Funktion „Projektdiagnose“ von Adobe Workfront nutzt die Leistungsfähigkeit des KI-Assistenten, um Ihnen sofort eine Bewertung zu geben, wie Ihre Projekte funktionieren, welche Bereiche Ihre Aufmerksamkeit erfordern und wie Probleme vermieden werden können, die Sie Zeit und Geld kosten können.

Der KI-Assistent kann eine Bewertung des Projektzustands für die folgenden Objekte erstellen:

* Ein einzelnes Projekt
* Ein einzelnes Programm
* Mehrere Projekte

Weitere Informationen zum KI-Assistenten finden Sie unter [KI-Assistent - Übersicht](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Auswählen oder höher </p> 
<p>Workflow auswählen oder höher</p>
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td> 
<p>Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationen der Zugriffsebene</p></td> 
   <td><p>Sie müssen Systemadministrator sein, um Projektzustandskonfigurationen verwalten zu können </p>
   <p>Zugriff auf Projekte bearbeiten, um Projektzustandskonfigurationen anzuwenden </p>
     <p>Anzeigen des Zugriffs auf Projekte zum Anzeigen von Projektzustandskonfigurationen </p>
  </td> 
  </tr>  
    </tr>  
</tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Für die Betaversion zur Projektdiagnose registrieren

Um die Projektdiagnose nutzen zu können, muss in Ihrer Organisation der KI-Assistent aktiviert sein.

Um den KI-Assistenten und die Projektdiagnose für Ihre Organisation zu aktivieren, müssen alle folgenden Bedingungen erfüllt sein:

* Ihr Unternehmen muss zu Adobe IMS (Identity Management System) migriert sein.
* Ihr Unternehmen muss über einen Select-, Prime- oder Ultimate Workfront-Plan verfügen
* Das einheitliche Adobe-Erlebnis muss aktiviert sein.
* Adobe muss eine unterzeichnete Adobe Gen AI-Vereinbarung in der Datei haben.
* Der Workfront-Administrator muss den KI-Assistenten für Benutzende in Ihrer Organisation aktivieren. Der KI-Assistent wird über Zugriffsebenen aktiviert.
* Sowohl die Option KI aktivieren als auch die Option Projektdiagnose müssen im Abschnitt KI-Voreinstellungen unter Setup > System > Voreinstellungen ausgewählt werden.

  ![Abschnitt KI-Voreinstellungen](assets/ai-preferences.png)

Weitere Informationen finden Sie unter [Übersicht über den KI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)Assistenten und [Systemeinstellungen konfigurieren](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Berechnen der Projektintegrität

Der KI-Assistent bietet Ihnen eine schnelle Bewertung der Gesamtbedingung eines Projekts, indem Sie ihm einen der verfügbaren Projektzustandsstatus zuweisen:

* Im Zielbereich
* Gefährdet
* In Schwierigkeiten

Dieser Status wird mithilfe der Projekt- und Programmkomponenten berechnet, z. B. Projektfortschritt, unterschätzte Arbeit und mehr. Eine vollständige Liste der Komponenten, die zur Messung des Projektzustands verwendet werden, finden Sie im Abschnitt [Liste der Projekt- und ](#project-and-program-states-list)).

Jeder Projektkomponente wird eine numerische Risikobewertung zugewiesen, die von (0-100) ausgeht und dann gemittelt wird, um den Gesamtzustand des Projekts zu erstellen:

* Am Ziel (75 oder höher): Die Projektleistung liegt innerhalb der erwarteten Schwellenwerte.
* Gefährdet (50-74): Es werden neue Probleme erkannt, die sich auf die Projektleistung auswirken können.
* In Schwierigkeiten (49 oder weniger): Die Projektleistung liegt unter den akzeptablen Schwellenwerten und erfordert sofortiges Eingreifen.

>[!NOTE]
>
>* Der KI-Assistent bewertet derzeit nur die Daten des ausgewählten Projekts.
>* Die projektübergreifende oder historische Analyse ist noch nicht in der Berechnung der Projektkonsistenz enthalten.

### Beispiele für die Berechnung des Projektzustands für ein Projekt

Im ersten Beispiel werden vier Projektkomponenten ausgewertet und ihre individuellen Risikobewertungen wie folgt berechnet:

* 2 On Target (90-Risiko-Score)
* 1 Risiko (45 Risikobewertung)
* 1 in Schwierigkeiten (20 Risikobewertung)

Wenn Sie diese Werte im Durchschnitt berechnen, ist das Ergebnis 61. Mithilfe der oben aufgeführten Kriterien für den Projektzustand versetzt dies dieses Projekt in den Zustand „Gefährdet“.

Im nächsten Beispiel ist zu einem frühen Zeitpunkt in der Timeline des Projekts eine Zeitplanänderung von einem Tag erfolgt. In diesem Szenario bewertet der KI-Assistent sowohl den Zeitpunkt als auch die Auswirkungen der Änderung im Verhältnis zur Gesamtdauer des Projekts:

* Eine Verschiebung um einen Tag zu Beginn eines 60-tägigen Projektzeitplans ist geringfügig und wird in der Regel als „Am Ziel“ bewertet.
* Eine Verschiebung um einen Tag in der Nähe des Abschlussdatums eines Projekts wirkt sich stärker auf die Unterbrechungen aus und kann als Gefährdet oder In Schwierigkeiten bewertet werden.

Da es sich um eine geringfügige Änderung handelt, die zu einem frühen Zeitpunkt in der Projektzeitleiste stattfand, versetzt dies das Projekt in den Status „On Target“.

Wenn in der Zeitleiste eines Projekts mehrere Zeitplanänderungen auftreten, werden diese Änderungen bewertet und dann gemittelt, bevor sie auf die Projektkonsistenzberechnung angewendet werden.

## Unterschiede zwischen Projektbedingungen und Projektstatus

Projektbedingungen und Projektzustand sind in Workfront ähnliche Konzepte und haben dieselben Standardnamen zur Beschreibung der Projektbedingung oder des Projektzustands (On Target, At Risk und In Trouble), dienen jedoch unterschiedlichen Zwecken.

Die Projektbedingungen bieten eine grundlegende Momentaufnahme der aktuellen Leistung eines Projekts, die nur auf den geplanten, projizierten und geschätzten Terminen basiert. Sie kann manuell vom Projektbesitzer oder automatisch von Workfront auf Grundlage der Projektaufgaben festgelegt werden. Alternativ dazu ist Project Health umfassender und bewertet zusätzliche Faktoren, sodass Sie ein besseres Verständnis davon erhalten, wie es funktioniert.

Weitere Informationen zu Projektbedingungen finden Sie unter [Benutzerdefinierte Bedingungen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

## Liste der Projekt- und Programmstatus

Die nachstehende Tabelle enthält eine Aufschlüsselung der verfügbaren Status, die der KI-Assistent Ihrem Projekt oder Programm beim Generieren einer Projektzustandsbewertung zuweist.

<table>
    <tr>
        <td><b>Projektstatus</b></td>
        <td><b>Definition</b></td>
        <td><b>Faktoren</b></td>
    </tr>
    <tr>
        <td>Im Zielbereich</td>
        <td>Dies wird zugewiesen, wenn das durchschnittliche Risikoniveau für die folgenden Faktoren unter den gesunden Schwellenwert fällt.
        </td>
        <td> 
        <ul><li>Umfangsausweitung</li>
        <li>Fehlende Felder</li>
        <li>Planänderungen</li>
        <li>Unterschätzte Arbeit</li>
        <li>Projektfortschritt</li>
        <li>Überfällige Aufgaben</li>
        <li>Budget</li>
        </ul></td>
    </tr>
    <tr>
        <td>Gefährdet</td>
        <td>Dies wird zugewiesen, wenn das durchschnittliche Risikoniveau für die folgenden Faktoren knapp unter den gesunden Schwellenwert fällt.</td>
        <td>
        <ul><li>Umfangsausweitung</li>
        <li>Fehlende Felder</li>
        <li>Planänderungen</li>
        <li>Unterschätzte Arbeit</li>
        <li>Projektfortschritt</li>
        <li>Überfällige Aufgaben</li>
        <li>Budget</li>
        </ul></td>
    </tr>
    <tr>
        <td>In Schwierigkeiten</td>
        <td>Dies wird zugewiesen, wenn das durchschnittliche Risikoniveau für die folgenden Faktoren unter den gesunden Schwellenwert fällt.</td>
        <td>
        <ul><li>Umfangsausweitung</li>
        <li>Fehlende Felder</li>
        <li>Planänderungen</li>
        <li>Unterschätzte Arbeit</li>
        <li>Projektfortschritt</li>
        <li>Überfällige Aufgaben</li>
        <li>Budget</li>
        </ul></td>
    </tr>
    </tr>
   </table>

## Liste mit Eingabeaufforderungen des KI-Assistenten

Nachstehend finden Sie eine Liste von Eingabeaufforderungen, mit denen Sie die KI-Bewertung anfordern können, um eine Bewertung des Projektzustands für ein Projekt, ein Programm oder alle Projekte in Ihrem Konto zu generieren.

<table>
    <tr>
        <td><b>Standort</b></td>
        <td><b>Eingabeaufforderung</b></td>
    </tr>
    <tr>
        <td>Eine bestimmte Seite mit Projektdetails</td>
        <td><em>Wie gesund ist dieses Projekt?</em></td>
    </tr>
    <tr>
        <td>Beliebige Seite in Workfront </td>
        <td><em>Wie ist der Zustand von Projekt [PROJEKTNAME]?</em></td>
    </tr>
    <tr>
        <td>Beliebige Seite in Workfront </td>
        <td><em>Wie gesund sind meine Projekte?</em></td>
    </tr>
       <tr>
        <td>Eine spezifische Seite mit Programmdetails</td>
        <td><em>Was ist der Gesundheitszustand dieses Programms?</em></td>
    </tr>
       <tr>
        <td>Beliebige Seite in Workfront </td>
        <td><em>Wie sieht der Zustand des Programms [PROGRAMMNAME] aus?</em></td>
    </tr>
   </table>

## Projektzustandskonfigurationen verwalten

Eine Konfiguration für den Projektzustand enthält spezifische Kriterien, die bestimmen, wie der Projektzustand berechnet wird. Nachdem eine Konfiguration erstellt wurde, können Sie sie auf ein Projekt anwenden.

>[!NOTE]
>
>Sie müssen Systemadministrator sein, um Projektzustandskonfigurationen verwalten zu können.

{{step-1-to-setup}}

1. Klicken Sie **linken Bereich auf** Projektvoreinstellungen“ und wählen Sie dann in **angezeigten Dropdown-Liste** Projektstatus“ aus.

1. Klicken Sie oben rechts auf der Seite auf **Neue Konfiguration**.

1. (Optional) Ersetzen Sie auf der Seite mit den Konfigurationsdetails *Nicht benannte Konfiguration* durch eine neue Konfiguration **Name**.

1. Deaktivieren Sie im **Welche Faktoren möchten Sie in den Projektzustand aufnehmen** die Auswahl aller Faktoren, die Sie bei der Bestimmung der Projektzustandskriterien nicht berücksichtigen möchten:
   * **Scope creep**: Wie sehr sich der Projektumfang seit dem Start erweitert hat.

   * **Erforderliche Felder**: Wenn erforderliche Felder fehlen (z. B. Projektbeschreibung). Diese Pflichtfelder bestimmen die Vollständigkeit des Projekts und werden im Abschnitt **Welche Felder möchten Sie auf Vollständigkeit überprüfen?** folgenden Konfigurationsabschnitt.


   * **Zeitplanänderungen**: Wie viele Zeitplanänderungen sind seit dem Start des Projekts aufgetreten.

   * **Aufgabenschätzung**: Wie genau die Aufgabenarbeit geschätzt wurde (z. B. keine überfälligen Aufgaben derzeit im Projekt).

   * **Aufgaben-Burndown**: Wie die Projektarbeit im Vergleich zur Projektzeitleiste voranschreitet.

   * **Überfällige Aufgaben**: Wie viele Aufgaben liegen derzeit nach ihrem Fälligkeitsdatum?

   * **Kosten**: Wenn das Projekt derzeit das Budget überschreitet.

1. In der **Wann beginnt Ihr Projekt offiziell?Wählen Sie** Abschnitt aus der Dropdown-Liste das Ereignis aus, das den Beginn Ihres Projekts signalisiert.

1. In der **Wie schätzen Sie den Arbeitsaufwand für ein Projekt ein?Wählen Sie** Abschnitt aus, welcher Projektfaktor mit zunehmendem Projektumfang größer wird.

1. In den **Welche Felder möchten Sie auf Vollständigkeit überprüfen?Wählen Sie** Abschnitt ein oder mehrere Felder aus, die auf ihre Vollständigkeit überprüft werden sollen.

   ![Felder zur Projektvollständigkeit](assets/project-completeness-fields.png)


1. Klicken **oben** auf „Speichern“.

## Anwenden von Projektzustandskonfigurationen

Nachdem ein Admin eine Projektzustandskonfiguration erstellt hat, können Benutzende mit Bearbeitungszugriff diese auf ein Projekt anwenden.


{{step1-to-projects}}

1. Wählen Sie auf **Seite** ein Projekt aus.

1. Klicken Sie auf das **Mehr**-Symbol ![Mehr](assets/more-icon.png) rechts neben dem Projektnamen und wählen Sie dann **Bearbeiten**. Das **Seitenbedienfeld** Projekt bearbeiten“ wird geöffnet.

1. Wählen Sie im linken Bedienfeld die Option **Projekteinstellungen**.

1. Wählen Sie **Feld** Projektzustandskonfiguration“ die Konfiguration aus, die Sie auf dieses Projekt anwenden möchten.

   ![Feld für die Konfiguration des Projektzustands](assets/project-health-configurations.png)

1. Klicken **unten links** Bedienfeld auf „Speichern“.

## Erstellen einer Projektzustandsbewertung für ein Projekt oder Programm

Wenn Sie Ansichtszugriff für ein Projekt oder Programm haben, können Sie mit dem KI-Assistenten die zugehörige Projektzustandsbewertung erstellen.

Wenn Sie eine Bewertung für ein Projekt generieren, kann dies entweder auf der Projektseite oder durch Verweis auf den Projektnamen erfolgen, wenn Sie den Assistenten nach der Leistung des Projekts fragen.

Wenn Sie eine Bewertung für ein Programm generieren, können Sie dies über die Seite mit den Programmdetails tun.

>[!NOTE]
>
>Eine Bewertung des Projektzustands kann erst für ein Projekt generiert werden, nachdem das Projekt gestartet wurde. Sie können konfigurieren, welche Ereignis-Trigger ein Projekt in den Projekteinstellungen starten sollen.

Weitere Informationen finden Sie im folgenden Abschnitt in diesem Artikel: [Verwalten von Projektzustandskonfigurationen](#manage-project-health-configurations).

1. Navigieren Sie zu dem Projekt oder Programm, für das Sie eine Bewertung des Projektzustands generieren möchten.

1. Klicken Sie auf der Seite mit den Projekt-/Programmdetails **das Symbol** KI![Assistent-Symbol](assets/ai-assistant-icon.png) in der oberen rechten Ecke des Bildschirms. KI-Assistent wird geöffnet.

1. Geben Sie im Feld **Fragen zu Workfront** Folgendes ein: *Wie sieht der Zustand dieses Projekts aus?*

   Oder

   Geben Sie im Feld **Fragen zu Workfront** Folgendes ein: *Wie sieht der Zustand dieses Programms aus?*

   >[!NOTE]
   >
   >Wenn Sie über eine andere Seite in Workfront auf den KI-Assistenten zugreifen, können Sie Folgendes eingeben *Was ist der Zustand des Projekts [PROJEKTNAME]?* oder *Was ist der Zustand des Programms [PROGRAMMNAME]?* <br>
   >Eine vollständige Liste der aktuellen Eingabeaufforderungen finden Sie im folgenden Abschnitt in diesem Artikel: [Liste der Eingabeaufforderungen des KI-Assistenten](#ai-assistant-prompts-list).

1. Klicken Sie auf das **Senden**-Symbol ![Senden-Symbol](assets/send-icon.png). Die Bewertung des Projektstatus wird generiert und im Bedienfeld angezeigt. Oben bei jeder Bewertung des Projektzustands wird ein Badge angezeigt, das den aktuellen Zustand des Projekts wiedergibt.

   ![Bewertung des Projektzustands](assets/health-assessment.png)

   Wenn Sie eine Bewertung für ein Portfolio generieren, werden mehrere Abzeichen aufgelistet, die die Bedingung jedes Projekts im Programm anzeigen. Weitere Informationen zu den Badge-Kennzeichnungen finden Sie im folgenden Abschnitt in diesem Artikel: [Projekt- und Programmstatusliste](#project-and-program-states-list).

1. (Optional) Klicken Sie auf einen der Bewertungspunkte, um dessen Details zu erweitern.

1. (Optional) Klicken Sie im Modus Erweiterte Details auf den Link Aufgabe , um die Aufgabendetails zu öffnen.

   ![Erweiterte Details](assets/expanded-details.png)

1. Klicken Sie nach Überprüfung der Projektzustandsdetails auf das **Schließen**-Symbol ![Schließen-](assets/close-icon.png)) in der oberen rechten Ecke des KI-Assistenten.

## Erstellen einer Projektdiagnose für mehrere Projekte

Sie können eine kombinierte Bewertung des Projektzustands für alle Projekte generieren, für die Sie derzeit Ansichtszugriff (oder höher) haben.

Ein Projekt wird nur dann in die kombinierte Bewertung des Projektzustands einbezogen, wenn es gestartet wurde. Sie können konfigurieren, welche Ereignis-Trigger ein Projekt in den Projekteinstellungen starten sollen. Weitere Informationen finden Sie im folgenden Abschnitt in diesem Artikel: [Verwalten von Projektzustandskonfigurationen](#manage-project-health-configurations).

1. Klicken Sie auf **KI** Assistent![ Symbol KI-Assistent](assets/ai-assistant-icon.png) in der rechten oberen Ecke des Bildschirms. KI-Assistent wird geöffnet.

1. Geben Sie Folgendes in das Feld **Fragen zu Workfront** ein: *Wie sieht der Zustand meiner Projekte aus?*

   Eine vollständige Liste der aktuellen Eingabeaufforderungen finden Sie im folgenden Abschnitt in diesem Artikel: [Liste der Eingabeaufforderungen des KI-Assistenten](#ai-assistant-prompts-list).

1. Klicken Sie auf das **Senden**-Symbol ![Senden-Symbol](assets/send-icon.png). Die Bewertung des Projektstatus wird generiert und im Bedienfeld angezeigt.

   ![Bewertung mehrerer Projekte](assets/multiple-projects-assessment.png)

   Beim Generieren einer Bewertung für mehrere Projekte gruppiert der KI-Assistent die Ergebnisse basierend auf der aktuellen Leistung der Projekte.

1. (Optional) Klicken Sie auf eines der Projektzustandsbedingungs-Badges, um die Projektliste zu erweitern, und wählen Sie dann einen Link für ein bestimmtes Projekt aus, um zur Detailseite dieses Projekts zu gehen.

1. Klicken Sie nach Überprüfung der Projektzustandsdetails auf das **Schließen**-Symbol ![Schließen-Symbol](assets/close-icon.png) in der oberen rechten Ecke des KI-Assistenten, um es zu schließen.

<!--

## Build a Project Health table report in a Canvas Dashboard

>[!IMPORTANT]
>
>The Canvas Dashboards feature is currently only available for users participating in the beta stage. For more information, see [Canvas Dashboards beta information](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md). 

You can add a table report to a Canvas Dashboard in order to easily visualize your Project Health data in a table format.  

### Prerequisites 

You must create a dashboard before you can build a table report. 

For more, see [Create a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

### Build a Project Health table report 

There are many configuration options available for building a Project Health table report. In this section, we'll walk you through the process of creating one that displays the following columns: 

* **Name**: Contains the project name. 
* **Project Health Analysis**: Contains a summary of the Project Health assessment. 
* **Project Health Created At**: Contains the date/time when the Project Health assessment was last generated. 
* **Project Health Label**: Contains the project's label (e.g. On Target, At Risk, or In Trouble).

{{step1-to-dashboards}}

1. In the left panel, click **Canvas Dashboards**. 
1. In the upper-right corner, click **New Dashboard**. 
1. In the **Create dashboard** box, enter the dashboard's **Name** and **Description**. 
1. Click **Create**. 
1. In the **Add report** box, select **Create report**. 
1. On the left side, select **Table**. 
1. In the upper-right corner, click **Create report**. 
1. (Optional) Follow the steps below to configure the **Details** ![Details icon](assets/details-icon.png) section: 
    1. Enter a report **Name**. 
    1. Enter a report **Description**. 
1. Follow the steps below to configure the **Build table** ![Build table icon](assets/drilldown-column.png) section: 
    1. In the left panel, click the **Table columns** icon. 
    1. Click **Add column**, then select **Project** > **Name**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Health Analysis**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Created At**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Health Label**. 

1. Follow the steps below to configure the **Filter** ![Filter icon](assets/filter-icon.png) section: 
    1. In the left panel, click the **Filter** icon. 
    1. Select **Edit filter**. 
    1. Click **Add condition** and then specify the field you want to filter by and the modifier that defines what kind of condition the field must meet. The column appears in the preview section on the right.
    1. (Optional) Click **Add filter group** to add another set of filtering criteria. The default operator between the sets is AND. Click the operator to change it to OR. 

1. Follow the steps below to configure the **Drilldown Group Settings** ![Group settings](assets/drilldown-group-icon.png) section: 
    1. In the left panel, click the **Group Settings** icon. 
    1. Click the **Add grouping** button and then select the field you want to create as a grouping. The grouping column appears in the preview section on the right. 

1. Click **Save** to create the report.

-->
