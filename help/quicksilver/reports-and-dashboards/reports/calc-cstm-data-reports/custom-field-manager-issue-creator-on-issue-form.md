---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Beispiel für ein berechnetes benutzerdefiniertes Feld: den Manager bzw. die Managerin des Erstellers bzw. der Erstellerin eines Problems im benutzerdefinierten Formular für Probleme anzeigen'
description: Mit einem berechneten benutzerdefinierten Feld können Sie den Namen des Managers des Erstellers eines Problems in einem benutzerdefinierten Formular anzeigen, das an das Problem angehängt ist. Mit derselben Anweisung können Sie ähnliche berechnete Felder für Projekte, Probleme und andere Objekte erstellen.
author: Courtney
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 23%

---

# Beispiel für ein berechnetes benutzerdefiniertes Feld: den Manager bzw. die Managerin des Erstellers bzw. der Erstellerin eines Problems im benutzerdefinierten Formular für Probleme anzeigen

Mit einem berechneten benutzerdefinierten Feld können Sie den Namen des Managers des Erstellers eines Problems in einem benutzerdefinierten Formular anzeigen, das an das Problem angehängt ist. Mit derselben Anweisung können Sie ähnliche berechnete Felder für Projekte, Probleme und andere Objekte erstellen.

<!--
outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-Paket</p> </td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-Lizenz</p> </td> 
   <td>
      <p>Standard</p>
      <p>Abo</p></td>
  </tr> 
  <tr> 
   <td><p>Konfigurationen der Zugriffsebene</p></td> 
   <td> <p>Administrativer Zugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objektberechtigungen</p> </td> 
   <td> <p>Gewähren von Zugriff auf das Objekt, an das das Formular angehängt ist, mit Zugriff zum Bearbeiten des benutzerdefinierten Formulars</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Manager des Erstellers eines Problems im benutzerdefinierten Formular für Probleme anzeigen

Die folgenden Schritte zeigen, wie Sie ein berechnetes Feld für ein benutzerdefiniertes Formular für ein Problem erstellen können, in dem Sie den Namen des Managers des Benutzers erfassen können, der das Problem erstellt hat. Der Prozess ist identisch, wenn Sie z. B. den Namen des Managers eines Benutzers erfassen möchten, der eine Aufgabe, ein Projekt oder ein Portfolio erstellt hat.

1. Erstellen Sie ein benutzerdefiniertes Anfrage-Formular und fügen Sie ihm ein berechnetes Feld hinzu.

   Informationen zum Erstellen eines benutzerdefinierten Formulars und Hinzufügen berechneter Felder dazu finden Sie in den folgenden Artikeln:

   * [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [Hinzufügen berechneter Felder zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. Kopieren Sie den folgenden Textmoduscode und fügen Sie ihn in das Feld **Berechnung** des benutzerdefinierten Formulars ein:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Bei benutzerdefinierten Feldberechnungen wird zwischen Groß- und Kleinschreibung unterschieden.

1. Klicken Sie **Fertig** und dann **Speichern + Schließen**.

   Der Manager des Benutzers, der das Problem erstellt hat, wird im berechneten Feld angezeigt, wenn das Formular, das das Feld enthält, an ein Problem angehängt ist.
