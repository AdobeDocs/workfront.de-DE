---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Grundlagen der Migration von Workfront zur Adobe Admin Console
description: In diesem Artikel wird der Prozess des Wechsels eines Unternehmens in die Adobe Admin Console allgemein beschrieben, sodass Sie als Workfront-Administrator wissen, was Sie erwarten können.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1114'
ht-degree: 0%

---

# Grundlagen der Migration von Workfront zur Adobe Admin Console

Adobe verändert die Art und Weise, wie Sie Ihre Adobe Workfront-Benutzenden verwalten, und steigert so Ihre Produktivität. Im Rahmen dieser Änderung migriert Adobe Ihre Workfront-Instanz und Ihre Benutzerinnen und Benutzer zum Adobe Admin Console. Dies ist eine erforderliche Migration und hat keine Auswirkungen auf Berichte, Genehmigungspfade, Inhalte oder Assets. Dies wirkt sich darauf aus, wie Sie den Benutzerzugriff verwalten und wie sich Ihre Benutzer anmelden.

In diesem Artikel wird der Prozess des Wechsels eines Unternehmens in die Adobe Admin Console allgemein beschrieben, sodass Sie als Workfront-Administrator wissen, was Sie erwarten können.

Informationen dazu, wie Sie mit der Adobe Admin Console Ihre Adobe-Berechtigungen im gesamten Unternehmen verwalten können, finden Sie unter [Verwalten von Benutzenden in der Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## Was ändert sich?

Im Rahmen der Migration wechselt Ihre Benutzerverwaltung von der Workfront-Anwendung zur Adobe Admin Console mit den folgenden Administratorrollen:

* **Systemadministratoren** sind Super-Benutzer mit den Berechtigungen aller Administratoren. Sie weisen alle administrativen Rollen zu und verwalten Benutzer für die gesamte Organisation für alle Produkte.

* **Produktprofil-Administratoren (Workfront-Systemadministratoren)** verwalten, welche Benutzer in der Organisation Zugriff auf Workfront erhalten.

* **Benutzer melden sich mit Adobe Identity an.** Nachdem Adobe bestehende Benutzende in die Adobe Admin Console migriert hat, melden sich diese mit ihrer neuen Adobe-Identität bei ihren Workfront-Instanzen an - entweder mit einer Adobe ID oder Adobe Federated ID (SSO).

* **Die Verwaltung aller anderen Funktionen, einschließlich der Verwaltung von Funktionen** Benutzerrollen, Arbeitsbereichen, Funktionen und Verhaltensweisen, innerhalb des Workfront-Programms selbst ändert sich nicht.

## Zeitleiste für die Migration von Journey

Adobe migriert zuerst Ihre Workfront-Instanz zur Adobe Admin Console und dann alle vorhandenen Benutzenden mit verifizierten E-Mail-Adressen. Wenn Sie System- oder Workfront-Produktprofil-Administrator (Workfront-Systemadministrator) sind, erhalten Sie E-Mails, die Sie durch die Migrations-Journey führen. Hier ist eine Zeitleiste dessen, was Sie erwarten können:

### Workfront-Migration zu Adobe Admin Console abgeschlossen

Systemadministratoren erhalten eine E-Mail, wenn die Migration von Workfront zu Adobe Admin Console abgeschlossen ist. Zu diesem Zeitpunkt müssen Systemadministratoren möglicherweise einige erforderliche Schritte ausführen **bevor die Benutzermigration gestartet wird** um die Auswirkungen auf Workfront-Benutzer zu minimieren.

* **Wenn sich Ihre Workfront-Benutzer derzeit mit SSO** anmelden, müssen Sie SSO auf der Adobe Admin Console einrichten, damit sich Ihre Benutzer weiterhin mit SSO anmelden können. Wenn Ihre Workfront-Benutzenden derzeit SSO nicht verwenden, es jedoch auf Adobe Admin Console einrichten möchten, können Sie dies an dieser Stelle auf der Migrations-Journey tun.
* **Wenn Sie bereits andere Adobe-Produkte in Ihrer Adobe Admin Console** verwalten, kann Adobe Ihre Zustimmung einholen, Benutzer automatisch in Ihre bestehende Konsole zu migrieren. Klicken Sie in **E-Mail auf** Erste Schritte“, um zur Einverständnisseite zu navigieren.
* **Wenn Sie den Anfordererlizenztyp bereits gelöscht haben** wird er Ihrem System hinzugefügt. Diesem Lizenztyp werden keine Benutzer zugewiesen. Er ist jedoch für die Synchronisierung zwischen Workfront und Adobe Admin Console erforderlich. Sie müssen keine Maßnahmen bezüglich des Lizenztyps des Antragstellers ergreifen.

An der Benutzerverwaltung ändert sich derzeit nichts. Workfront-Administratoren verwalten weiterhin Benutzende in Workfront und Benutzende melden sich weiterhin mit ihrer Workfront ID oder SSO an, bis die Benutzermigration abgeschlossen ist.

### Benutzermigration planen

Nachdem der Systemadministrator die im vorherigen Abschnitt beschriebenen Voraussetzungen erfüllt hat, plant Adobe Ihre Benutzermigration automatisch für 30 Tage, nachdem diese Voraussetzungen erfüllt sind, und kommuniziert mit Workfront-Produktprofiladministratoren (Workfront-Systemadministratoren), um die Benutzermigration zu verwalten.

Workfront-Produktprofil-Administratoren (Workfront-Systemadministratoren):

* Sie erhalten eine E-Mail mit dem geplanten Startdatum der Benutzermigration (etwa 30 Tage nach Abschluss dieser Voraussetzungen)
* Erhalten Sie Zugriff auf die vorgesehene Workfront-Administratorkonsole, über die sie das Migrationsdatum ändern können

  >[!NOTE]
  >
  >Aufgrund der Komplexität der Migration sind Datumsänderungen auf maximal 30 Tage nach dem geplanten Datum beschränkt. Wenden Sie sich an den Support, wenn Sie ein späteres Datum benötigen.

* Eine Erinnerungs-E-Mail 1 Tag vor dem Startdatum der Benutzermigration erhalten

### Vorbereitung der Benutzer auf den Migrationstag

Als Workfront-Produktprofil-Administrator (Workfront-Systemadministrator) sind Sie dafür verantwortlich, sicherzustellen, dass alle Benutzenden auf den Migrationstag vorbereitet sind.

* Bereiten Sie alle Benutzer auf die bevorstehende Migration zu Adobe Identity vor, indem Sie sie über Folgendes informieren:

   * Wenn Benutzer migrieren, erhalten sie eine E-Mail von Adobe, in der sie über die Änderung der Art und Weise ihrer Anmeldung bei Workfront informiert werden. Benutzer werden aufgefordert, eine Einladung zur erstmaligen Anmeldung mit Adobe Identity anzunehmen, entweder durch Anmeldung mit einer bestehenden Adobe ID oder durch Einrichtung einer neuen mit derselben E-Mail-Adresse.

### Was am Migrationstag zu erwarten ist

* **Die Benutzermigration beginnt um Mitternacht im Hosting-Rechenzentrum des Kunden in Workfront.**

* **Adobe migriert zuerst automatisch Workfront-Administratoren.** Wenn Workfront-Administratoren in die Adobe Identity migriert werden, wird ihnen die Rolle &quot;Adobe-Produktprofil-Administrator“ (Workfront-Systemadministrator) zugewiesen. Vorhandene Rollen, die ein Benutzer vor der Migration möglicherweise hat, sind davon nicht betroffen.

  >[!NOTE]
  >
  >Während der Benutzermigration erfolgt kein Verlust des Zugriffs auf das Produkt. Wenn Benutzende während der Migration ihrer Benutzenden angemeldet sind, hat dies keine Auswirkungen. Bei ihrer nächsten Anmeldung müssen sie jedoch ihre Adobe-Identität verwenden.



* **Wenn Benutzerinnen und Benutzer migriert werden, erhalten sie eine E-Mail von Adobe, in der sie über die Änderung der Art und Weise ihrer Anmeldung bei Workfront informiert werden.** Benutzer werden aufgefordert, eine Einladung zur erstmaligen Anmeldung mit Adobe Identity anzunehmen, entweder indem sie sich mit einer bestehenden Adobe ID anmelden oder indem sie eine neue Adobe ID mit derselben E-Mail-Adresse einrichten.

  Informationen zum Anmelden bei Workfront mit einer Adobe ID finden Sie unter [Bei Adobe Experience Cloud anmelden](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### Benutzermigration abgeschlossen

Adobe benachrichtigt alle System- und Produktprofiladministratoren (Workfront-Systemadministratoren) per E-Mail, nachdem alle Administratoren und Benutzer migriert wurden. Derzeit melden sich alle Workfront-Benutzer für diese Instanz mit Adobe Identity bei Workfront an. Workfront-System- und -Produktprofiladministratoren (Workfront-Systemadministratoren) können den Benutzerzugriff innerhalb von Adobe Admin Console verwalten. Wenn Kundinnen und Kunden keine Form der Ordnersynchronisierung in der Administratorkonsole verwenden, können sie den Zugriff auf Workfront weiterhin in der Workfront-Anwendung verwalten.

## Support erhalten

Bei Fragen oder Bedenken folgen Sie den Schritten, die im Artikel [Wenden Sie sich an den Support](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md) beschrieben sind.




