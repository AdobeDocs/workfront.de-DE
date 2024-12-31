---
title: Einschränkungen bei der Proofing-Zusammenarbeit mit Personen außerhalb Ihrer Organisation
description: Einschränkungen bei der Proofing-Zusammenarbeit mit Personen außerhalb Ihrer Organisation
author: Courtney
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Einschränkungen bei der Proofing-Zusammenarbeit mit Personen außerhalb Ihrer Organisation

Es gibt einige Einschränkungen, die bei der Kommunikation mit Personen außerhalb Ihrer Organisation zu beachten sind, wenn sie zu einem Korrekturabzug hinzugefügt werden. Dies gilt insbesondere, wenn die Person außerhalb Ihrer Organisation über Proofing-Zugriff in einer separaten Umgebung verfügt.

## Kontakte mit der Auszeichnung eines Mitglieds

In einer Proofing-Umgebung gibt es drei Arten von Kontakten:

* **Benutzer**: Benutzer verfügen über eine Workfront Proof-Anmeldung in der Umgebung Ihres Unternehmens.
* **Mitglieder**: Mitglieder verfügen über eine eigene Workfront Proof-Anmeldung in der Umgebung eines anderen Unternehmens (nicht in Ihrer eigenen). Mitglieder können in Ihrer Umgebung nicht in Benutzer konvertiert werden.
* **Gäste**: Gäste verfügen nicht über eine eigene Workfront Proof-Anmeldung in der Umgebung Ihres Unternehmens, Sie haben jedoch deren Details zu Ihrem Konto hinzugefügt (z. B. Gastbewertungen für Korrekturabzüge). Sie können Gäste in Benutzer konvertieren.

Da Mitglieder nicht in Benutzer konvertiert werden können, ist ihre Möglichkeit, Personen in Korrekturabzugskommentaren zu taggen, auf Benutzer aus *ihrer ursprünglichen Organisation* beschränkt.

**Beispiel:** Unternehmen A lädt einen externen Benutzer ein, einen Korrekturabzug zu überprüfen. Dieser Benutzer existiert bereits in einer separaten Testumgebung, Firma B.

 

Wenn Firma A den externen Benutzer zum Korrekturabzug einlädt, wird der externe Benutzer der Kontaktliste von Firma A als Mitglied hinzugefügt. Reviewer im Korrekturabzugs-Workflow von Unternehmen A können externe Benutzer in Korrekturabzugskommentaren taggen, da sie sich jetzt im Kontaktverzeichnis von Unternehmen A befinden.

 

Der externe Benutzer kann keine Benutzer von Unternehmen A taggen, obwohl sie sich im selben Korrekturabzugs-Workflow befinden, da die Benutzer von Unternehmen A nicht als Kontakte zu Unternehmen B hinzugefügt wurden.

 

Der externe Benutzer von Unternehmen B kann andere Benutzer von Unternehmen B taggen, wenn sie sich im Korrekturabzugs-Workflow befinden oder wenn er berechtigt ist, den Korrekturabzug für neue Benutzer freizugeben, da diese Benutzer als Kontakte in Unternehmen B vorhanden sind.
