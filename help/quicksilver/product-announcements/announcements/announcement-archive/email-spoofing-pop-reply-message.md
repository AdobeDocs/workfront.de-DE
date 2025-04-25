---
content-type: reference
navigation-topic: announcements
title: Entfernung von E-Mail-Spoofing und POP-Antworten
description: Mit Version 20.3 (geplant für August 2020) ändern wir die Art und Weise, wie Adobe Workfront E-Mails sendet und empfängt.
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# E-Mail-Spoofing und POP-Antwort

Mit Version 20.3 (geplant für August 2020) ändern wir die Art und Weise, wie Adobe Workfront E-Mails sendet und empfängt.

## Ausgehende E-Mails von Workfront

Um den erfolgreichen Versand von E-Mails zu steigern, werden wir das Spoofing von E-Mails, das häufig als Spam getaggt wird, beseitigen (siehe E-Mail-Spoofing). Alle E-Mails von Workfront werden von `notifications@my.workfront.com` gesendet, einschließlich automatisierter Warnhinweise und der Kommunikation zwischen Benutzenden. Eine Beispiel-E-Mail von Joan Harris sieht im Bereich Absender Ihrer E-Mail wie folgt aus:

![Beispiel-E-Mail](assets/noreply.png)

*Wir empfehlen Ihnen dringend, sich an Ihr IT-Team zu wenden* um sicherzustellen, dass E-Mails von `notifications@my.workfront.com` nicht für eingehende E-Mails in Ihrem System blockiert werden. Sie können auch auf [Zulassungsliste Ihrer Firewall konfigurieren](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) verweisen, um zu erfahren, von welchen IP-Adressen unser Traffic und unsere E-Mail stammen.

## Eingehende E-Mail-Antworten auf Benachrichtigungen (POP-Antwort)

Bestimmte E-Mail-Benachrichtigungen ermöglichen es Benutzenden, per E-Mail zu antworten und die Antwort als Kommentarantwort im Workfront-System in Workfront zu kopieren. Systemadministratoren in Workfront konnten traditionell zwischen der Bereitstellung ihres eigenen POP-E-Mail-Servers zum Empfang dieser Antworten und der Verwendung des integrierten Workfront-Antwortsystems wählen. Die benutzerdefinierte POP-E-Mail-Server-Auswahl wird mit Version 20.3 entfernt. Alle Konten, die für die Verwendung eines benutzerdefinierten Servers konfiguriert wurden, werden automatisch auf das native E-Mail-Antwortsystem von Workfront umgestellt. Systemadministratoren oder andere Workfront-Benutzer müssen keine Maßnahmen ergreifen.

E-Mails, die direkt aus dem Workfront Proof-System stammen, werden nicht geändert. Sie werden weiterhin diese E-Mails erhalten, wie Sie es bereits getan haben.

Bei weiteren Fragen oder Anliegen wenden Sie sich bitte an das [Workfront-Supportteam](https://experienceleague.adobe.com/?support-tab=home#support).
