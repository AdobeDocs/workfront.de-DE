---
content-type: reference
navigation-topic: announcements
title: Entfernen von E-Mail-Spoofing und POP-Antworten
description: Mit Version 20.3 (geplant für August 2020) nehmen wir zwei Änderungen an der Art vor, wie Adobe Workfront E-Mails sendet und empfängt.
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# E-Mail-Spoofing- und POP-Antwort

Mit Version 20.3 (geplant für August 2020) nehmen wir zwei Änderungen an der Art vor, wie Adobe Workfront E-Mails sendet und empfängt.

## Ausgehende E-Mail aus Workfront

Um den erfolgreichen Versand von E-Mails zu verbessern, beseitigen wir den Spoofing von E-Mails, die häufig als Spam gekennzeichnet werden (siehe E-Mail-Spoofing). Alle E-Mails von Workfront werden von notifications@my.workfront.com gesendet, einschließlich automatisierter Warnhinweise und der Kommunikation zwischen Benutzern und Benutzern. Eine Beispiel-E-Mail von Joan Harris sieht in diesem Abschnitt Ihrer E-Mail aus:

![](assets/noreply.png)

*Wir empfehlen dringend, dass Sie sich an Ihr IT-Team wenden*, um sicherzustellen, dass E-Mails von notifications@my.workfront.com nicht für eingehende E-Mails an Ihr System blockiert werden. Unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) finden Sie auch Informationen dazu, von welchen IP-Adressen unser Traffic und unsere E-Mail stammen.

## Eingehende E-Mail-Antworten auf Benachrichtigungen (POP-Antwort)

Bestimmte E-Mail-Benachrichtigungen ermöglichen es Benutzern, per E-Mail zu antworten und die Antwort als Kommentar-Antwort in Workfront im Workfront-System zu kopieren. Systemadministratoren in Workfront haben bisher die Wahl zwischen der Bereitstellung ihres eigenen POP-E-Mail-Servers für den Empfang dieser Antworten oder der Verwendung des integrierten Workfront-Antwortsystems getroffen. Die benutzerdefinierte POP-E-Mail-Server-Auswahl wird mit Version 20.3 entfernt. Alle Konten, die für die Verwendung eines benutzerdefinierten Servers konfiguriert sind, werden automatisch auf das native E-Mail-Antwortsystem von Workfront umgestellt. Für Systemadministratoren und andere Benutzer von Workfront ist keine Aktion erforderlich.

An E-Mails, die direkt aus dem Workfront Proof-System kommen, wird nichts geändert. Sie werden diese E-Mails wie bisher erhalten.

Wenden Sie sich bei weiteren Fragen oder Bedenken an das [Workfront-Supportteam](https://one.workfront.com/s/support?language=en_US).
