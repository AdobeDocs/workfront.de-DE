---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: Vorschau der Sandbox-Testumgebung - [!DNL Workfront Proof]
description: Die Vorschau-Sandbox ist eine Testumgebung, die als Replikation Ihrer Live-Umgebung dient und an jedem Wochenende aktualisiert wird [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# Vorschau der Sandbox-Testumgebung - [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Die Vorschau-Sandbox ist eine Testumgebung, die als Replikation Ihrer Live-Umgebung dient und an jedem Wochenende aktualisiert wird [!DNL Workfront Proof].

## Grundlegendes zur Vorschau-Sandbox

Die Vorschau-Sandbox dient als Umgebung, in der Benutzer in Ihrer Organisation Daten aus der Produktionsumgebung sicher testen und verwenden können, ohne die Produktionsumgebung zu beeinträchtigen. Es eignet sich ideal zum Ausführen von Trainings-Sitzungen, zum Testen neuer Funktionen und zum Ermitteln der Einrichtungsfunktion.

Außerdem werden neue Produktfunktionen in die Vorschau-Sandbox-Umgebung hochgeladen, bevor sie in die Produktionsumgebung bereitgestellt werden. Ihre Benutzer können dort neue Funktionen ausprobieren, ohne den üblichen Workflow in der Produktionsumgebung zu beeinträchtigen.

Die Vorschau-Sandbox enthält Ihre tatsächlichen Produktionsdaten. Daten werden von der Produktion in die Vorschau übertragen und nicht umgekehrt. Er wird jedes Wochenende aktualisiert, sodass die Daten bis zu einer Woche hinter der Produktionsumgebung liegen können. Elemente, die seit der letzten Aktualisierungszeit erstellt wurden, befinden sich bis zur folgenden Aktualisierung in der Umgebung &quot;Sandbox-Vorschau&quot;.

## Zugriff auf die Vorschau-Sandbox

Als Systemadministrator haben Sie standardmäßig Zugriff auf die Umgebung &quot;Sandbox-Vorschau&quot;. Wenn Sie nicht auf die in diesem Abschnitt beschriebene Vorschau-Sandbox-Umgebung zugreifen können, wenden Sie sich an Ihren [!DNL Workfront] Administrator oder unserem Supportteam.

* [Zugriff auf die Vorschau-Sandbox als eigenständige Sandbox [!DNL Workfront Proof] Kunde](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [Zugriff auf die Vorschau-Sandbox als [!DNL Workfront]+[!DNL Workfront Proof] Kunde](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### Zugriff auf die Vorschau-Sandbox als eigenständige Sandbox [!DNL Workfront Proof] Kunde

1. Navigieren Sie zu dieser URL:  `https://preview.proofhq.com`.
1. Melden Sie sich mit Ihren Anmeldedaten für die Vorschau an.\
   Ihre Vorschauberechtigungen sollten mit Ihren Produktionsberechtigungen übereinstimmen, es sei denn, Sie haben sie in der Produktion geändert, nachdem die Vorschauaktualisierung stattgefunden hat. Die Anmeldungen werden nur synchronisiert, wenn eine Aktualisierung erfolgt, die an jedem Wochenende stattfindet. Sie werden nicht automatisch synchronisiert.

### Zugriff auf die Vorschau-Sandbox als [!DNL Workfront+Workfront] Testversand-Kunde

Als Systemadministrator können Sie auf die [!DNL Workfront Proof] Sandbox-Vorschau über [!DNL Workfront] -Schnittstelle.

So greifen Sie auf die [!DNL Workfront Proof] Vorschau-Sandbox:

1. Melden Sie sich bei Ihrer [!DNL Workfront] Umgebung.
1. Klicken **[!UICONTROL Einrichtung]** in der Symbolleiste für globale Navigation.
1. Klicken **[!UICONTROL System]** >**[!UICONTROL Voreinstellungen]**.

1. Im **[!UICONTROL Testumgebungen]** Abschnitt, klicken Sie auf **[!UICONTROL Sandbox-Vorschau]**.

1. Melden Sie sich mit Ihren Vorschauanmeldeinformationen an.\
   Ihre Vorschauanmeldeinformationen sollten mit Ihren Produktionsberechtigungen übereinstimmen, es sei denn, Sie haben sie in der Produktion geändert, nachdem die Vorschauaktualisierung stattgefunden hat. Die Anmeldungen werden nur bei einer Aktualisierung synchronisiert. Sie werden nicht automatisch synchronisiert.
1. Klicken Sie auf [!DNL Workfront Proof] in der Symbolleiste für globale Navigation.\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   Die [!DNL Workfront Proof] Die Vorschau der Umgebung wird angezeigt.

## Empfangen von E-Mails über die Vorschau-Sandbox

E-Mail-Benachrichtigungen werden nie von der [!DNL Workfront Proof] Vorschau der Umgebung
