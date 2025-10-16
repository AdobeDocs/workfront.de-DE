---
product-area: workfront-integrations
keywords: Google,DOC,Dokument,Blatt,Folie
navigation-topic: workfront-for-g-suite
title: Zugreifen auf  [!DNL Adobe Workfront]  Inhalte von Google Workspace aus
description: Sie können auf Ihre  [!DNL Adobe Workfront]  zugreifen, einschließlich aller Ihnen zugewiesenen Aufgaben, Probleme, Genehmigungen und Zugriffsanfragen, ohne Google Workspace verlassen zu müssen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: da2ecaf1-5cfb-470e-90a1-fbb386db8670
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Zugreifen auf [!DNL Adobe Workfront] [!UICONTROL Home]-Inhalte über [!DNL Google Workspace]

>[!IMPORTANT]
>
>Um stabilere und skalierbarere Integrationen bereitzustellen, wechseln wir mithilfe von Workfront Automation and Integration (Fusion) zu einem modernen, flexiblen Integrationsansatz. Im Rahmen dieser Umstellung werden die folgenden Funktionen von Workfront für Google Workspace nach dem 28. **2026 nicht mehr verfügbar**:
>
>* Zugriff auf Google Workspace-Funktionen in Workfront
>
>* Anzeigen und Verwalten von Workfront-Aufgaben über Gmail oder das Site-Panel des Google-Kalenders
>
>Es wird empfohlen, Workfront-Automatisierung und -Integration für die Integrationsanforderungen Ihres Unternehmens mit Google Workspace zu verwenden.
>
>Einen Überblick über die Automatisierung und Integration von Workfront finden Sie unter [Übersicht über Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Informationen zu den spezifischen Funktionen der Workfront-Automatisierungs- und Integrationsmodule für Google Workspace finden Sie unter [Gmail-](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) und [Google-](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Sie können auf Ihre [!DNL Adobe Workfront] [!UICONTROL Startseite] Inhalte zugreifen, einschließlich aller Ihnen zugewiesenen Aufgaben, Probleme, Genehmigungen und Zugriffsanfragen, ohne Google Workspace verlassen zu müssen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p><p>Arbeit oder höher</p>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie über [!UICONTROL &#x200B; auf &#x200B;]Startseite[!DNL Google Workspace]-Inhalte zugreifen können, müssen Sie

* Installieren von [!DNL Workfront for Google Workspace]\
   Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Zugriff [!DNL Workfront] [!UICONTROL Startseite] von [!DNL Google Workspace]

1. Stellen Sie sicher, dass Sie bei [!DNL Workfront] angemeldet sind.
1. Wenn das Bedienfeld [!UICONTROL Workfront für Google Workspace] nicht angezeigt wird, klicken Sie auf das [!DNL Workfront]-Symbol ![Workfront](assets/wf-lion-icon.png) in der Seitenleiste [!DNL Google Workspace] Add-ons ganz rechts auf der Seite.
1. Wenn oben in [!DNL Workfront] ein Pfeil nach links für [!DNL Google Workspace] angezeigt wird, klicken Sie auf den Pfeil, um zum Bereich [!UICONTROL Startseite] zu wechseln.

1. Klicken Sie im Bereich **[!UICONTROL Sortieren nach]** auf den Erweiterungspfeil ![Erweiterungspfeil](assets/dropdown-arrow.png) und klicken Sie dann auf eine Option, um anzugeben, wie Sie Ihre Arbeitselemente gruppieren möchten, damit Sie die gewünschte finden können.

   Wenn Sie nach **[!UICONTROL Commit-Datum]** oder **[!UICONTROL Geplantes]**) sortieren, befinden sich die ältesten Arbeitselemente oben.

   Beim Sortieren nach **[!UICONTROL Projekt]** werden Arbeitselemente in der Reihenfolge ihrer übergeordneten Projekte angezeigt, alphabetisch von A bis Z aufgelistet. Arbeitselemente ohne übergeordnetes Projekt werden unter &quot;**[!UICONTROL Projekt“]**.

1. Klicken Sie auf den Erweiterungspfeil ![Erweiterungspfeil](assets/dropdown-arrow.png) für die Gruppierung, die Sie anzeigen möchten.

   Die Anzahl der in den einzelnen Gruppen enthaltenen Elemente wird in Klammern angezeigt. Wenn Sie auf den [!UICONTROL Erweitern]-Pfeil klicken, werden alle Arbeitselemente in der Gruppe angezeigt.

   Arbeitselemente werden wie folgt angezeigt:

   * ![Aufgabensymbol](assets/task-icon.png) **Aufgaben** zeigt den Namen des übergeordneten Projekts, den Aufgabennamen und das geplante Abschlussdatum an.

   * ![Problem-Symbol](assets/issue-icon.png) **Probleme** zeigen den Namen des übergeordneten Projekts, den Namen des Problems und das geplante Abschlussdatum an.

   * ![Dokumentsymbol](assets/document-icon.png) **Genehmigungen** zeigen den Namen des Anforderers, den Dokumentnamen und das Übermittlungsdatum an.
   * **Zugriffsanfragen** zeigen den Namen des Anforderers, den Objektnamen und das Übermittlungsdatum an. Links wird das Symbol für den Objekttyp angezeigt.

1. Klicken Sie auf eine beliebige Stelle in einem Arbeitselement, um dessen Details, Aktualisierungen und Dokumente anzuzeigen.
