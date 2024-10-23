---
title: Übersicht über Connected Record Types
description: Eine Möglichkeit, anzugeben, wie sich einzelne Datensatztypen zueinander verhalten, besteht darin, sie miteinander zu verbinden. Außerdem können Sie Adobe Workfront Planning-Record-Typen mit Objekttypen aus anderen Anwendungen verbinden, um das Benutzererlebnis zu verbessern und den Fokus in einer Anwendung zu behalten.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1c04c68b-7a7f-46ae-b750-2b1f79855de4
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '1438'
ht-degree: 1%

---

# Übersicht über verbundene Datensatztypen

<!--see the commented out markers below for the Planning connection field, might not display in green; also add Preview tags for the article-->

Sie können angeben, dass einzelne Datensatztypen miteinander oder mit Objekten aus anderen Anwendungen in Beziehung stehen, indem Sie sie verbinden.

In diesem Artikel wird eine Übersicht über Verbindungen vom Typ Datensatz beschrieben und beschrieben, welche Verbindungstypen zwischen Datensätzen und Objekttypen hergestellt werden können.

Weitere Informationen zum Verbinden von Datensatztypen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

## Überlegungen zum Verbinden von Datensatztypen

Es gibt zwei Schritte für Verbindungen in der Workfront-Planung:

1. Zunächst müssen Sie eine Verbindung zwischen zwei Datensatztypen oder einem Datensatztyp und einem Objekttyp aus einer anderen Anwendung herstellen. Informationen dazu, wie Sie Datensatztypen verbinden können, finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
1. Zweitens können Sie einzelne Datensätze eines Typs mit Datensätzen eines anderen Typs verbinden, nachdem die beiden Datensatztypen miteinander verbunden sind. Informationen zum Verbinden von Datensätzen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

Beachten Sie Folgendes zum Verbinden von Datensatztypen:

* Sie können die folgenden Entitäten in der Adobe Workfront-Planung verbinden:

   * Zwei Datensatztypen.

     Standardmäßig können Sie zwei Datensatztypen aus demselben Arbeitsbereich verbinden. Sie können auch Datensatztypen einrichten, um über andere Arbeitsbereiche eine Verbindung mit Datensatztypen herzustellen. Weitere Informationen finden Sie unter [Bearbeiten von Datensatztypen](/help/quicksilver/planning/architecture/edit-record-types.md).
   * Ein Datensatztyp und ein Objekttyp aus einer anderen Anwendung.

* Sie können die Workfront Planning-Datensatztypen mit den folgenden Objekttypen aus den folgenden Anwendungen verbinden:

   * Adobe Workfront:

      * Projekte
      * Portfolios
      * Programme
      * Firmen
      * Gruppen

   * Adobe Experience Manager Assets:

      * Bilder
      * Ordner

     >[!IMPORTANT]
     >
     >Sie müssen über eine Adobe Experience Manager Assets-Lizenz verfügen und die Workfront-Instanz Ihres Unternehmens muss mit der Adobe Business Platform oder der Adobe Admin Console integriert sein, um Workfront Planning-Datensätze mit Adobe Experience Manager Assets zu verbinden.
     >
     >Wenn Sie Fragen zum Einstieg in Adobe Admin Console haben, lesen Sie die [FAQ zum einheitlichen Erlebnis für Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Nachdem Sie Datensätze für die verbundenen Datensatztypen erstellt haben, können Sie diese über das Feld für den verbundenen Datensatz miteinander verknüpfen.  Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

* Nachdem Sie einen Datensatztyp mit einem anderen Datensatztyp oder einem Objekttyp aus einer anderen Anwendung verbunden haben, gibt es folgende Szenarien:

   * **Wenn Sie zwei Planungs-Datensatztypen verbinden**: Ein verknüpftes Datensatzfeld wird für den Datensatztyp erstellt, von dem Sie eine Verbindung herstellen. Ein ähnliches verknüpftes Datensatzfeld wird für den Datensatztyp erstellt, mit dem Sie eine Verbindung herstellen.

     Wenn Sie beispielsweise den Datensatztyp &quot;Kampagne&quot;mit dem Datensatztyp &quot;Produkt&quot;verbinden, wird ein verknüpftes Datensatzfeld (Verbindungsfeld) mit dem Namen &quot;Verknüpftes Produkt&quot;im Datensatztyp &quot;Kampagne&quot;erstellt. Ein verknüpfter Datensatztyp, der automatisch &quot;Kampagne&quot;heißt, wird für den Produktdatensatztyp erstellt.

   * **Wenn Sie einen Datensatztyp mit einem Objekttyp aus einer anderen Anwendung verbinden**:

      * Ein verknüpftes Datensatzfeld wird für den Datensatztyp erstellt, aus dem Sie eine Verbindung herstellen. Für den Objekttyp der anderen Anwendung wird kein verknüpftes Datensatzfeld erstellt.
      * Über Workfront-Objekte ist der Zugriff auf die Felder für die Planung von Datensätzen nicht möglich.
      * Auf der Registerkarte Planung des Workfront-Objekts werden Planungsdatensätze angezeigt. Weitere Informationen finden Sie unter [Verwalten von Datensätzen im Abschnitt &quot;Planung&quot;von Adobe Workfront-Objekten](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
     <!--* Planning records are visible from a Workfront object's custom form when you add the Planning connection field type to the form. For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). -->
      * Die Planung von Datensatzfeldern ist über Experience Manager-Assets verfügbar, wenn der Workfront-Administrator die Metadaten-Zuordnung durch die Integration zwischen Workfront und Adobe Experience Manager Assets konfiguriert. Weitere Informationen finden Sie unter [Konfigurieren der Asset-Metadatenzuordnung zwischen Adobe Workfront und Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).


   * **Wenn Sie Suchfelder aus dem Datensatz oder Objekt hinzufügen, mit dem Sie eine Verbindung herstellen,**: Zusätzlich zur Erstellung eines verknüpften Datensatzfelds können Sie auch eine Verbindung zu Feldern des verbundenen Datensatzes oder Objekttyps herstellen, die als Lookup-Felder bezeichnet werden. Ein verknüpftes (oder Lookup-Feld) mit Informationen aus dem Datensatz, mit dem Sie eine Verbindung herstellen, wird auf dem Datensatz angezeigt, von dem Sie eine Verbindung herstellen.

     Sie können Felder von anderen Datensatztypen oder von Objekten einer anderen Anwendung mit dem Datensatztyp für die Workfront-Planung verbinden.

     Verknüpfte Felder sind schreibgeschützt und zeigen automatisch Informationen aus verbundenen Datensätzen an.

     Sie können in Formeln, Filtern oder Gruppierungen auf Suchfelder aus anderen Datensätzen oder Objektarten verweisen.

     Wenn Sie beispielsweise den Datensatztyp &quot;Kampagne&quot;mit einem Workfront-Projekt verbinden und das Feld &quot;Geplantes Abschlussdatum&quot;des Projekts in den Workfront-Planungsdatensatz übertragen möchten, wird automatisch ein verknüpftes Feld namens &quot;Geplantes Abschlussdatum&quot;(aus Projekt) für die Kampagne erstellt. Sie können dieses verknüpfte Feld nicht manuell bearbeiten. Im Feld Geplantes Abschlussdatum (aus Projekt) wird das geplante Abschlussdatum der verknüpften Projekte angezeigt.

     >[!IMPORTANT]
     >
     >Jeder Benutzer mit der Berechtigung Anzeigen oder höher für den Arbeitsbereich kann die Informationen in den Suchfeldern anzeigen, unabhängig von seinen Berechtigungen oder Zugriffsniveaus in der Anwendung der verknüpften Objektarten oder den Berechtigungen in anderen Arbeitsbereichen.

     Verknüpfte Datensatzfelder erhalten das Beziehungssymbol ![](assets/relationship-field-icon.png).

     Verknüpfte Felder erhalten ein Symbol, das den Feldtyp identifiziert. Verknüpfte (oder Lookup-) Felder weisen beispielsweise Symbole darauf hin, dass es sich bei einem Feld um eine Zahl, einen Absatz oder ein Datum handelt.

## Verbindungstypen

Nachdem Sie eine Verbindung zwischen zwei Datensatztypen oder zwischen einem Datensatz und einem Objekttyp aus einer anderen Anwendung hergestellt haben, können Sie in den verbundenen Datensatzfeldern Datensätze hinzufügen.

Je nachdem, wie viele Datensätze Sie einem verbundenen Datensatzfeld hinzufügen können, stehen Ihnen beim Verbinden von Datensatztypen folgende Verbindungstypen zur Verfügung:

* [Viele-zu-viele](#many-to-many-connection-type)
* [Eins-zu-viele](#one-to-many-connection-type)
* [Viele-zu-eins](#many-to-one-connection-type)
* [Eins-zu-eins](#many-to-one-connection-type)

>[!WARNING]
>
>Diese Optionen sind beim Verbinden der folgenden Elemente nicht verfügbar:
>
>* Zwei Datensätze aus verschiedenen Arbeitsbereichen
>
>* Datensatz-Typ und Experience Manager-Assets

### Viele-zu-viele-Verbindungstyp

![](assets/many-to-many-connection-picker.png)

Wenn Sie eine n:n-Verbindung zwischen Datensatztypen erstellen, können Sie dann aus beiden Datensatztypen mehrere Datensätze im Verbindungsfeld auswählen.

Wenn Sie beispielsweise eine n:n-Verbindung zwischen Kampagnen und Projekten herstellen, können Sie für jede Kampagne mehrere Projekte und für jedes Projekt mehrere Kampagnen auswählen.

Ein reales Beispiel für eine Beziehung zwischen vielen und vielen ist die Beziehung zwischen Filmen und Schauspielern. Jeder Film kann mehrere Schauspieler haben, und jeder Schauspieler kann in mehreren Filmen spielen.

Wenn Sie diesen Verbindungstyp auswählen, können Sie den Verbindungstyp nach dem Speichern nicht mehr ändern.

### Eins-zu-viele-Verbindungstyp

![](assets/one-to-many-connection-picker.png)


Wenn Sie eine Eins-zu-viele-Verbindung zwischen Datensatztypen erstellen, können Sie dann im aktuellen Datensatztyp mehrere Datensätze im Verbindungsfeld auswählen. Das entsprechende Verbindungsfeld im Datensatztyp, zu dem Sie eine Verbindung herstellen, ermöglicht jedoch die Auswahl nur eines Datensatzes. Das Feld &quot;Verbundener Datensatz&quot;, das automatisch für den zweiten Datensatztyp erstellt wird, wird automatisch auf einen Beziehungstyp zwischen zwei Datensätzen eingestellt.

Wenn Sie beispielsweise eine Eins-zu-viele-Verbindung zwischen Kampagnen und Projekten herstellen, können Sie für jede Kampagne mehrere Projekte auswählen, aber jedes Projekt kann nur mit einer Kampagne verbunden sein.

Ein reales Beispiel für einen 1:n-Beziehungstyp ist die Beziehung zwischen Bibliotheken und Büchern: Eine Bibliothek hat viele Bücher im Inventar, aber ein bestimmtes Buch kann nur zu einem bestimmten Zeitpunkt in einer Bibliothek sein.

Wenn Sie diesen Verbindungstyp auswählen, können Sie ihn später nur in einen Verbindungstyp vom Typ Viele-zu-viele ändern.

### Viele-zu-eins-Verbindungstyp

![](assets/many-to-one-connection-picker.png)


Wenn Sie eine n:1-Verbindung zwischen Datensatztypen erstellen, können Sie dann jeden Datensatz im aktuellen Datensatztyp mit nur einem Datensatz des verbundenen Datensatztyps verbinden. Das Feld für den verknüpften Datensatz, das automatisch beim zweiten Datensatztyp erstellt wird, wird automatisch auf einen 1:n-Beziehungstyp eingestellt.

Wenn Sie beispielsweise Kampagnen mit Projekten verbinden und diese Art von Verbindung wählen, können Sie einer Kampagne nur ein Projekt hinzufügen. Sie können jedoch einem Projekt mehrere Kampagnen hinzufügen.

Ein reales Beispiel für einen Beziehungstyp zwischen einer und vielen Filmen ist die Beziehung zwischen vielen Filmen und einem Schauspieler: Ein Schauspieler kann in vielen Filmen sein, aber jeder Film kann nur einen bestimmten Schauspieler haben, der einmal in seiner Wiedergabe war.

Wenn Sie diesen Verbindungstyp auswählen, können Sie ihn später nur in einen Verbindungstyp vom Typ Viele-zu-viele ändern.

### Eins-zu-Eins-Verbindungstyp

![](assets/one-to-one-connection-picker.png)

Wenn Sie eine Eins-zu-Eins-Verbindung zwischen Datensatztypen herstellen, können Sie in beiden Datensatztypen jeden Datensatz nur mit einem Datensatz des anderen Datensatztyps verbinden.

Wenn Sie beispielsweise Kampagnen mit Projekten verbinden und diese Art der Verbindung auswählen, können Sie eine Kampagne mit einem Projekt verbinden. Ein Projekt kann nur mit einer Kampagne verbunden werden.

Ein echtes Beispiel für eine Eins-zu-Eins-Beziehung ist die Beziehung zwischen einer Person und der eindeutigen Kennung ihres Landes (z. B. Sozialversicherungsnummer, Pass-ID, lokale Identifikationsnummer): Jede Person hat nur eine eindeutige Kennung für ein Land und jede eindeutige Kennung kann nur mit einer Person verknüpft werden.

Wenn Sie diesen Verbindungstyp auswählen, können Sie ihn später in einen anderen Verbindungstyp ändern.
