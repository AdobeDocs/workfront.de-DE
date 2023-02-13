---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Berechnetes benutzerdefiniertes Feldbeispiel: Anzeigen des Verantwortlichen des Erstellers eines Problems im benutzerdefinierten Formular zum Problem"
description: Mithilfe eines berechneten benutzerdefinierten Felds können Sie den Namen des Verantwortlichen des Erstellers eines Problems in einem benutzerdefinierten Formular anzeigen, das an das Problem angehängt ist. Mit derselben Anweisung können Sie ähnliche berechnete Felder für Projekte, Probleme und andere Objekte erstellen.
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Berechnetes benutzerdefiniertes Feldbeispiel: Anzeigen des Verantwortlichen des Erstellers eines Problems im benutzerdefinierten Formular zum Problem

Mithilfe eines berechneten benutzerdefinierten Felds können Sie den Namen des Verantwortlichen des Erstellers eines Problems in einem benutzerdefinierten Formular anzeigen, das an das Problem angehängt ist. Mit derselben Anweisung können Sie ähnliche berechnete Felder für Projekte, Probleme und andere Objekte erstellen.

>[!TIP]
>
>Weitere Informationen zu weiteren benutzerdefinierten Textmodusbeispielen von anderen Kunden finden Sie im Abschnitt [Textmodus-Berichterstellung](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) Thema auf unserer Community-Site.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-Lizenz*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare<br>Informationen zur Gewährung von Administratorzugriff über die Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektberechtigungen</p> </td> 
   <td> <p>Beitragen Sie den Zugriff auf das Objekt, an das das Formular angehängt ist, und erhalten Sie Zugriff auf die Option Benutzerdefiniertes Formular bearbeiten .</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Anzeigen des Verantwortlichen des Erstellers eines Problems im benutzerdefinierten Formular zum Problem

Die folgenden Schritte zeigen, wie Sie ein berechnetes Feld für ein Problem-benutzerdefiniertes Formular erstellen können, in dem Sie den Namen des Managers des Benutzers erfassen können, der das Problem erstellt hat. Der Prozess ist identisch, wenn Sie den Namen des Managers eines Benutzers erfassen möchten, der eine Aufgabe, ein Projekt oder ein Portfolio erstellt hat.

1. Erstellen Sie ein benutzerdefiniertes Problemformular und fügen Sie ihm ein berechnetes Feld hinzu.

   Informationen zum Erstellen eines benutzerdefinierten Formulars und zum Hinzufügen berechneter Felder finden Sie in den folgenden Artikeln:

   * [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. Kopieren Sie den folgenden Textmoduscode und fügen Sie ihn in den **Berechnung** Feld des benutzerdefinierten Formulars:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Bei benutzerdefinierten Feldberechnungen wird zwischen Groß- und Kleinschreibung unterschieden.

1. Klicken **Fertig**, dann **Speichern und schließen**.

   Der Manager des Benutzers, der das Problem erstellt hat, wird im berechneten Feld angezeigt, wenn das Formular, das das Feld enthält, an ein Problem angehängt ist.
