---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Benutzer über Adobe Admin Console löschen
description: Sie können einen Benutzer nur aus Adobe Workfront Fusion entfernen und Zugriff auf andere Adobe-Produktprofile erhalten. Alternativ können Sie ihn vollständig aus der Adobe Admin Console entfernen.
author: Becky
feature: Workfront Fusion
exl-id: 0d989134-46c0-4637-b465-6fbe04258b8a
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Löschen von Benutzern über die [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>Die Funktion in diesem Artikel ist nur verfügbar, wenn die Instanz Ihres Unternehmens [!DNL Adobe Workfront Fusion] in den [!DNL Adobe Business Platform] integriert wurde.
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen in den [!DNL Adobe Business Platform] integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Verwaltungsunterschiede ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

Sie können einen Benutzer nur aus [!DNL Adobe Workfront Fusion] entfernen und Zugriff auf andere [!DNL Adobe] -Produktprofile gewähren. Alternativ können Sie den Benutzer vollständig aus dem [!DNL Adobe Admin Console] entfernen.

## Benutzer in [!DNL Adobe Workfront Fusion] löschen

Um einen Benutzer in [!DNL Adobe Workfront Fusion] zu löschen, müssen Sie den Benutzer über die [!DNL Adobe Admin Console] deaktivieren.

Ein Benutzer wird aus dem [!DNL Adobe Admin Console] deaktiviert, wenn einer der folgenden Punkte zutrifft:

* Der Benutzer wird aus einem Produkt- oder Produktprofil verschoben und keinem anderen Produkt- oder Produktprofil zugewiesen.
* Der Benutzer wird aus einer Gruppe entfernt, die mit einem Produktprofil verknüpft ist, und nicht aus einer anderen Gruppe, die mit einem Produktprofil verknüpft ist.
* Der Benutzer wird aus einem Produktprofil entfernt und keinem anderen Produktprofil zugewiesen.
* Der Benutzer wird in der Organisation, die Workfront Fusion enthält, gelöscht oder deaktiviert.

  Anweisungen finden Sie im Abschnitt &quot;Benutzer entfernen&quot;in [Benutzer einzeln verwalten](https://helpx.adobe.com/enterprise/using/manage-users-individually.html).

In [!DNL Workfront Fusion] wirkt sich die Deaktivierung auf eine der folgenden Arten auf den Benutzer aus:

* Wenn sich der Benutzer in nur einer Organisation befindet, wird der Benutzer deaktiviert.
* Wenn sich der Benutzer in mehr als einer Organisation befindet, wird der Benutzer aus der Organisation entfernt, in der der Benutzer mit dem [!DNL Adobe Admin Console] geändert wurde.
* Weitere Überlegungen zum Löschen eines Benutzers in [!DNL Workfront Fusion] finden Sie unter [Überlegungen beim Löschen eines Benutzers in  [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider)
