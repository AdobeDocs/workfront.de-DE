---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Berechnetes benutzerdefiniertes Feldbeispiel: Anzeigen des Managers des Erstellers eines Problems beim benutzerdefinierten Formular zum Problem"
description: Mithilfe eines berechneten benutzerdefinierten Felds können Sie den Namen des Verantwortlichen des Erstellers eines Problems in einem benutzerdefinierten Formular anzeigen, das an das Problem angehängt ist. Mit derselben Anweisung können Sie ähnliche berechnete Felder für Projekte, Probleme und andere Objekte erstellen.
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Beispiel für ein berechnetes benutzerdefiniertes Feld: Zeigen Sie den Manager des Erstellers eines Problems zum benutzerdefinierten Formular für das Problem an.

Mithilfe eines berechneten benutzerdefinierten Felds können Sie den Namen des Verantwortlichen des Erstellers eines Problems in einem benutzerdefinierten Formular anzeigen, das an das Problem angehängt ist. Mit derselben Anweisung können Sie ähnliche berechnete Felder für Projekte, Probleme und andere Objekte erstellen.

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-Lizenz*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare<br>Informationen zum Gewähren des Administratorzugriffs von der Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren des Administratorzugriffs für Benutzer auf bestimmte Bereiche</a>.</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektberechtigungen</p> </td> 
   <td> <p>Zugriff der Contribute auf das Objekt, an das das Formular angehängt ist, mit Zugriff auf "Benutzerdefiniertes Formular bearbeiten"</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Anzeigen des Verantwortlichen des Erstellers eines Problems im benutzerdefinierten Formular zum Problem

Die folgenden Schritte zeigen, wie Sie ein berechnetes Feld für ein Problem-benutzerdefiniertes Formular erstellen können, in dem Sie den Namen des Managers des Benutzers erfassen können, der das Problem erstellt hat. Der Prozess ist identisch, wenn Sie den Namen des Managers eines Benutzers erfassen möchten, der eine Aufgabe, ein Projekt oder ein Portfolio erstellt hat.

1. Erstellen Sie ein benutzerdefiniertes Problemformular und fügen Sie ihm ein berechnetes Feld hinzu.

   Informationen zum Erstellen eines benutzerdefinierten Formulars und zum Hinzufügen berechneter Felder finden Sie in den folgenden Artikeln:

   * [Benutzerdefiniertes Formular erstellen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [Berechnete Felder zu einem Formular hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. Kopieren Sie den folgenden Textmoduscode und fügen Sie ihn in das Feld **Berechnung** des benutzerdefinierten Formulars ein:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Bei benutzerdefinierten Feldberechnungen wird zwischen Groß- und Kleinschreibung unterschieden.

1. Klicken Sie auf **Fertig** und dann auf **Speichern + Schließen**.

   Der Manager des Benutzers, der das Problem erstellt hat, wird im berechneten Feld angezeigt, wenn das Formular, das das Feld enthält, an ein Problem angehängt ist.
