---
title: Prüfen von Einschränkungen bei der Zusammenarbeit mit Personen außerhalb Ihres Unternehmens
description: Prüfen von Einschränkungen bei der Zusammenarbeit mit Personen außerhalb Ihres Unternehmens
author: Courtney
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Prüfen von Einschränkungen bei der Zusammenarbeit mit Personen außerhalb Ihres Unternehmens

Bei der Kommunikation mit Personen außerhalb Ihres Unternehmens, die zu einem Testversand hinzugefügt werden, müssen einige Einschränkungen beachtet werden. Dies gilt insbesondere dann, wenn die Person außerhalb Ihres Unternehmens in einer separaten Umgebung über einen Testversandzugriff verfügt.

## Kontakte nach Mitgliedstaaten

In einer Testumgebung gibt es drei Kontakttypen:

* **Benutzer**: Benutzer haben eine Workfront Proof-Anmeldung in der Umgebung Ihres Unternehmens.
* **Mitglieder**: Mitglieder haben ihre eigene Workfront Proof-Anmeldung in der Umgebung eines anderen Unternehmens (nicht in Ihrer eigenen). Mitglieder können nicht in Benutzer in Ihrer Umgebung konvertiert werden.
* **Gäste**: Gäste haben keine eigene Workfront Proof-Anmeldung in der Umgebung Ihres Unternehmens, aber Sie haben ihre Details zu Ihrem Konto hinzugefügt (z. B. Gastreviewer bei Testsendungen). Sie können Gäste in Benutzer umwandeln.

Da Mitglieder nicht in Benutzer konvertiert werden können, ist ihre Fähigkeit, Personen in Testkommentaren mit Tags zu versehen, auf Benutzer aus *ihrer ursprünglichen Organisation* beschränkt.

**Beispiel:** Firma A lädt einen externen Benutzer ein, einen Testversand zu prüfen. Dieser Benutzer ist bereits in einer separaten Testumgebung, Firma B, vorhanden.

 

Wenn Unternehmen A den externen Benutzer zum Testversand einlädt, wird der externe Benutzer als Mitglied der Kontaktliste von Firma A hinzugefügt. Überprüfer im Testversand-Workflow von Unternehmen A können den externen Benutzer in Testversandkommentaren taggen, da sie sich jetzt im Kontaktverzeichnis von Firma A befinden.

 

Der externe Benutzer kann Benutzer von Firma A nicht mit Tags versehen, obwohl sie denselben Testversand-Workflow verwenden, da die Benutzer von Firma A nicht als Kontakte zu Firma B hinzugefügt wurden.

 

Der externe Benutzer von Firma B kann andere Benutzer von Firma B mit Tags versehen, wenn sie sich im Testversand-Workflow befinden oder die Berechtigung haben, den Testversand für neue Benutzer freizugeben, da diese Benutzer als Kontakte in Firma B vorhanden sind.
