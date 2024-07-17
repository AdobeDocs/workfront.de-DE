---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Informationen zur Migration von Workfront zu Adobe Admin Console
description: In diesem Artikel wird im Allgemeinen der Prozess der Umstellung eines Unternehmens auf die Adobe Admin Console beschrieben, sodass Sie als Workfront-Administrator wissen, was zu erwarten ist.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: 633c41eeb570402254125f92f3624cad7befd609
workflow-type: tm+mt
source-wordcount: '1114'
ht-degree: 0%

---

# Informationen zur Migration von Workfront zu Adobe Admin Console

Adobe verändert die Verwaltung Ihrer Adobe Workfront-Benutzer und bringt Ihnen und Ihrem Unternehmen eine höhere Produktivität. Im Rahmen dieser Änderung migriert Adobe Ihre Workfront-Instanz und Ihre Benutzer in die Adobe Admin Console. Dies ist eine erforderliche Migration und hat keine Auswirkungen auf Berichte, Genehmigungspfade, Inhalte oder Assets. Dies wirkt sich auf die Verwaltung des Benutzerzugriffs und die Anmeldung Ihrer Benutzer aus.

In diesem Artikel wird im Allgemeinen der Prozess der Umstellung eines Unternehmens auf die Adobe Admin Console beschrieben, sodass Sie als Workfront-Administrator wissen, was zu erwarten ist.

Informationen dazu, wie Sie mit der Adobe Admin Console Ihre Adobe-Berechtigungen in Ihrer gesamten Organisation verwalten können, finden Sie unter [Verwalten von Benutzern in der Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## Was ändert sich?

Im Rahmen der Migration wechselt Ihre Benutzerverwaltung von der Workfront-Anwendung zur Adobe Admin Console mit den folgenden Administratorrollen:

* **Systemadministratoren** sind Superbenutzer mit Berechtigungen aller Administratoren. Sie weisen alle Administratorrollen zu und verwalten Benutzer für die gesamte Organisation für alle Produkte.

* **Produktprofiladministratoren (Workfront-Systemadministratoren)** verwalten, welche Benutzer in der Organisation Zugriff auf Workfront erhalten.

* **Benutzer melden sich mit Adobe Identity an.** Nachdem Adobe bestehende Benutzer in die Adobe Admin Console migriert wurde, melden sich die Benutzer mit ihrer neuen Adobe-Identität - entweder mit einer Adobe ID- oder Adobe-Federated ID (SSO) - bei ihren Workfront-Instanzen an.

* **Die Verwaltung aller anderen Funktionen** innerhalb der Workfront-Anwendung selbst, einschließlich der Verwaltung von Funktionen, Benutzerrollen, Arbeitsbereichen, Funktionen und Verhaltensweisen, ändert sich nicht.

## Timeline zur Migration Journey

Adobe migriert zuerst Ihre Workfront-Instanz in die Adobe Admin Console und migriert dann alle vorhandenen Benutzer mit verifizierten E-Mail-Adressen. Wenn Sie Systemadministrator oder Workfront Product Profile-Administrator (Workfront-Systemadministrator) sind, erhalten Sie E-Mails, die Sie durch die Migration-Journey führen. Im Folgenden finden Sie eine Timeline zu den erwarteten Funktionen:

### Workfront Migration zu Adobe Admin Console Complete

Systemadministratoren erhalten eine E-Mail, wenn die Migration von Workfront zu Adobe Admin Console abgeschlossen ist. Zu diesem Zeitpunkt müssen Systemadministratoren möglicherweise einige erforderliche Schritte **vor Beginn der Benutzermigration durchführen**, um die Auswirkungen auf Workfront-Benutzer zu minimieren.

* **Wenn sich Ihre Workfront-Benutzer derzeit mit SSO** anmelden, müssen Sie SSO in der Adobe Admin Console einrichten, damit sich Ihre Benutzer weiterhin mit SSO anmelden können. Wenn Ihre Workfront-Benutzer derzeit keine SSO verwenden, Sie sie jedoch in Adobe Admin Console einrichten möchten, können Sie dies an dieser Stelle auf der Journey tun.
* **Wenn Sie bereits andere Adobe-Produkte in Ihrer Adobe Admin Console** verwalten, kann Adobe Ihre Zustimmung einholen, um Benutzer automatisch in Ihre bestehende Konsole zu migrieren. Klicken Sie in der E-Mail auf die Schaltfläche **Erste Schritte** , um zur Einverständnisseite zu navigieren.
* **Wenn Sie den Lizenztyp &quot;Anforderer&quot;** bereits gelöscht haben, wird er Ihrem System hinzugefügt. Diesem Lizenztyp werden keine Benutzer zugewiesen, er ist jedoch für die Synchronisation zwischen Workfront und Adobe Admin Console erforderlich. In Bezug auf den Lizenztyp &quot;Anforderer&quot;ist keine Aktion von Ihnen erforderlich.

Die Benutzerverwaltung ändert sich derzeit nicht. Workfront-Administratoren verwalten Benutzer weiterhin in Workfront und Benutzer melden sich weiterhin mit ihrer Workfront ID oder SSO an, bis die Benutzermigration abgeschlossen ist.

### Benutzermigration planen

Nachdem der Systemadministrator die im vorherigen Abschnitt beschriebenen Voraussetzungen erfüllt hat, plant Adobe automatisch die Benutzermigration für 30 Tage, nachdem diese Voraussetzungen erfüllt sind, und kommuniziert mit Workfront-Produktprofiladministratoren (Workfront-Systemadministratoren), um die Benutzermigration zu verwalten.

Administratoren des Workfront-Produktprofils (Workfront-Systemadministratoren):

* Erhalten Sie eine E-Mail mit dem geplanten Startdatum für die Benutzermigration (ca. 30 Tage nach Abschluss dieser Voraussetzungen)
* Rufen Sie die vorgesehene Workfront-Administrator-Konsole auf, in der der Benutzer sein Migrationsdatum ändern kann.

  >[!NOTE]
  >
  >Aufgrund der Komplexität der Migration sind Datumsänderungen auf maximal 30 Tage nach dem geplanten Datum beschränkt. Wenden Sie sich an den Support , wenn Sie ein späteres Datum benötigen.

* Erhalten einer Erinnerungsmail 1 Tag vor dem Startdatum der Benutzermigration

### Benutzer für den Migrationstag vorbereiten

Als Workfront-Produktprofiladministrator (Workfront-Systemadministrator) ist dafür verantwortlich, sicherzustellen, dass alle Benutzer auf den Migrationstag vorbereitet sind.

* Bereiten Sie alle Benutzer auf die bevorstehende Migration auf Adobe Identity vor, indem Sie sie über Folgendes informieren:

   * Wenn Benutzer migrieren, erhalten sie eine E-Mail von der Adobe, in der sie über die Änderung der Anmeldung bei Workfront informiert werden. Die Benutzer werden eingeladen, erstmals eine Einladung zur Anmeldung mit Adobe Identity anzunehmen, indem sie sich entweder mit einer bestehenden Adobe ID anmelden oder eine neue mit derselben E-Mail-Adresse einrichten.

### Was erwartet man am Migrationstag?

* **Die Benutzermigration beginnt um Mitternacht des Workfront-Rechenzentrums des Kunden, in dem das Hosting erfolgt.**

* **Adobe migriert zuerst automatisch Workfront-Administratoren.** Wenn Workfront-Administratoren zu Adobe Identity migriert werden, wird ihnen die Administratorrolle für das Adobe-Produktprofil (Workfront-Systemadministrator) zugewiesen. Vorhandene Rollen, die ein Benutzer vor der Migration hat, sind nicht betroffen.

  >[!NOTE]
  >
  >Während der Benutzermigration geht der Zugriff auf das Produkt nicht verloren. Wenn ein Benutzer während der Migration seines Benutzers angemeldet ist, hat dies keine Auswirkungen. Nach der nächsten Anmeldung müssen sie jedoch ihre Adobe Identity verwenden.



* **Wenn Benutzer migriert werden, erhalten sie eine E-Mail von der Adobe, in der sie über die Änderung der Anmeldung bei Workfront informiert werden.** Benutzer werden aufgefordert, erstmals eine Einladung zur Anmeldung mit Adobe Identity anzunehmen, indem sie sich entweder mit einer bestehenden Adobe ID anmelden oder eine neue Adobe ID mit derselben E-Mail-Adresse einrichten.

  Informationen zum Anmelden bei Workfront mit einer Adobe ID finden Sie unter [Bei Adobe Experience Cloud anmelden](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### Benutzermigration abgeschlossen

Adobe benachrichtigt alle Systemadministratoren und Produktprofiladministratoren (Workfront-Systemadministratoren) per E-Mail, nachdem alle Administratoren und Benutzer migriert wurden. Derzeit melden sich alle Workfront-Benutzer für diese Instanz mit Adobe Identity bei Workfront an. Workfront-Systemadministratoren und Produktprofiladministratoren (Workfront-Systemadministratoren) können den Benutzerzugriff innerhalb der Adobe Admin Console verwalten. Wenn Kunden keine Form der Ordnersynchronisierung innerhalb der Admin Console verwenden, können sie den Zugriff auf Workfront innerhalb der Workfront-Anwendung weiterhin verwalten.

## Support erhalten

Bei Fragen oder Anliegen folgen Sie den Schritten, die im Artikel [Support kontaktieren](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md) beschrieben sind.




