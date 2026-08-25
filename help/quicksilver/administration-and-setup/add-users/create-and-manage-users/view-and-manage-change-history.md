---
user-type: administrator
product-area: system-administration;setup
title: Anzeigen und Verwalten des Änderungsverlaufs
description: Mit dem Änderungsverlauf können Sie ein Änderungsprotokoll für Workfront-Objekte und -Felder anzeigen.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 1e06115eb5688271e2a6f4c8a41647eb644d8292
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 5%

---

# Änderungsverlauf anzeigen und verwalten

{{preview-fast-release-general}}

Mit dem Änderungsverlauf kann der Systemadministrator Änderungen an Objekten und bestimmten Feldern in Adobe Workfront konfigurieren und verfolgen. Mit der flexiblen Konfiguration kann der Administrator festlegen, welche Objekte und Felder genau verfolgt werden.

Der Änderungsverlauf kann die folgenden Typen definierter Daten verfolgen:

* Aktivität im Bereich „Setup“, z. B. Erstellen oder Löschen einer Zugriffsebene oder eines Aufgabengebiets
* Aktualisierungen auf Feldebene, z. B. Bearbeiten einer Projektbeschreibung oder Ändern der Layout-Vorlage eines Benutzers
* Objektaktualisierungen, z. B. Aktualisieren eines Projektstatus oder Anhängen eines benutzerdefinierten Formulars an eine Aufgabe
* <span class="preview">Einheitliche Workflow-Aktivität für Überprüfung und Genehmigung, einschließlich Teilnehmern und Entscheidungen</span>

Informationen zum Definieren der verfolgten Objekte und Felder finden Sie unter [Konfigurieren der nachzuverfolgenden Felder im Änderungsverlauf](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md).

In der Liste „Änderungsverlauf“ können Sie das Änderungsprotokoll für Workfront-Objekte anzeigen, einschließlich solcher Attribute:

* Objektname
* Objekttyp
* Art der Änderung (Vorgang)
* Datum und Uhrzeit der Änderung
* Source der Änderung, z. B. bestimmte Benutzende, APIs, Workfront Fusion, KI-LLMs oder das Workfront-System

>[!NOTE]
>
>Wenn Sie auf den Änderungsverlauf zugreifen, werden die verfolgten Änderungen nur für Felder angezeigt, für die Sie über die Berechtigung zum Anzeigen verfügen.
>Wenn beispielsweise Finanzdaten in Projekten verfolgt werden und Sie keinen Zugriff auf Finanzdaten haben, werden die Finanzfelder in der Liste „Änderungsverlauf“ nicht angezeigt.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td><span class="preview">Administrativer Zugriff auf den Änderungsverlauf</span></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Anzeigen des Änderungsverlaufs

Sie können die Änderungsprotokolle im Bereich „Setup“ einsehen.

Die Liste „Änderungsverlauf“ ist eine erweiterte Liste und enthält Filter, Spalten, Zeilenhöhe, eine Datumsauswahl und eine Suchleiste.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Tracking ändern > Verlaufsliste**.

   Die Liste „Änderungsverlauf“ wird geöffnet.

1. Um die Datumsangaben anzupassen, für die Änderungen angezeigt werden, klicken Sie auf die Datumsauswahl und wählen Sie die neuen Datumsangaben aus.

   Änderungen sind für die letzten 90 Tage verfügbar.

1. Um nach einem bestimmten Begriff zu suchen, klicken Sie in das Suchfeld und geben Sie den Begriff ein. Die Ergebnisse werden bei der Eingabe in der Liste hervorgehoben.
1. (Optional) Informationen zum Filtern nach einer Spalte finden Sie unter [Filtern von Elementen in einer erweiterten Liste](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list) im Artikel [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Optional) Informationen zum Ausblenden, Anzeigen oder Neuanordnen von Spalten finden Sie unter [Spalten anpassen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns) im Artikel [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Optional) Informationen zum Hinzufügen oder Entfernen von Spalten finden Sie unter [Hinzufügen und Entfernen von Spalten mit &#x200B;](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) Spaltenmanager“ im Artikel [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Optional) Informationen zum Anpassen der Zeilenhöhe finden Sie unter [Ändern der Zeilenhöhe in einer Ansicht](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view) im Artikel [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Änderungsverlauf exportieren

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Tracking ändern > Verlaufsliste**.
1. Filtern Sie die Liste, um die zu exportierenden Elemente anzuzeigen.
1. Klicken Sie auf **Export**-Symbol ![Export-Symbol](assets/export-icon.png) und wählen Sie aus, ob Sie im XLSX- oder CSV-Format speichern möchten.

   Das Feld Datei speichern wird geöffnet, und Sie können die exportierte Datei auf Ihrem Computer speichern.
   Speichern der exportierten Datei beenden Sie können ihn jetzt auf Ihrem Computer finden und für andere freigeben.



