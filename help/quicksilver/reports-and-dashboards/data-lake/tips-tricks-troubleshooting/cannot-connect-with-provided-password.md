---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Power BI-Tool kann keine Verbindung mit dem angegebenen Passwort herstellen
description: Wenn Sie versuchen, sich von Ihrem Power BI-Tool aus bei Data Connect anzumelden, erhalten Sie einen Anmeldefehler.
author: Courtney
feature: Reports and Dashboards
exl-id: c3f2b4a9-0831-48f0-871b-486d09ae5ea4
TQID: https://experienceleague.adobe.com/Z4RrMAPGd3CCti-cQFiJ7hlf-h8-suXeuoYfzk-9aKo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 229
ht-degree: 6%

---

# Power BI-Tool kann mit dem angegebenen Kennwort keine Verbindung herstellen

## Problem

Wenn Sie versuchen, sich von Ihrem Power BI-Tool aus bei Data Connect anzumelden, wird der folgende Fehler angezeigt:

`Cannot connect from BI tool with provided password`

## Ursache

Beim Erstellen der JDBC-Verbindung stellt Workfront ein temporäres Kennwort für die Datenverbindung bereit.

Bevor Sie über Power BI auf Data Connect zugreifen können, müssen Sie sich zunächst mit den bereitgestellten Verbindungsdetails anmelden, das temporäre Kennwort aktualisieren und dann mit Ihrer Anmeldung fortfahren.


## Lösung

Setzen Sie das Verbindungskennwort in Workfront zurück und erstellen Sie dann ein neues Kennwort mit dem Link im Dialogfeld „Verbindung bearbeiten“.

### Zurücksetzen des Verbindungskennworts in Workfront

1. Wechseln Sie zu Workfront > Einrichtung > System > Datenverbindung.
1. Suchen Sie die Verbindung in der Liste und öffnen Sie sie.
1. Markieren **unter „Verbindungskennwort zurücksetzen** das Kontrollkästchen, um zu bestätigen, dass Sie das Kennwort zurücksetzen möchten.
1. Klicken Sie **Verbindungskennwort zurücksetzen**.
   ![Verbindungskennwort zurücksetzen](assets/reset-password.png)
1. Fahren Sie mit dem folgenden Abschnitt fort.

### Neues Kennwort für die Verbindung erstellen

1. Kopieren Sie die URL und fügen Sie sie in eine neue Browser-Registerkarte ein.
1. Kopieren Sie in Workfront den Benutzernamen für die Verbindung und fügen Sie das Standardkennwort in die neue Browser-Registerkarte ein.
   ![URL und Standardkennwort kopieren](assets/link-password.png)
1. Klicken Sie auf **Anmelden**.
1. Geben Sie ein neues Kennwort ein und klicken Sie dann auf **Senden**.
1. Wechseln Sie zu Ihrem Power BI-Tool und melden Sie sich mit dem neuen Kennwort an.
