---
title: Übersicht über verbundene Datensatztypen
description: Eine Möglichkeit, die Beziehung zwischen den einzelnen Datensatztypen anzugeben, besteht darin, sie miteinander zu verbinden. Außerdem können Sie Datensatztypen von Adobe Workfront Planning mit Objekttypen aus anderen Anwendungen verbinden, um das Benutzererlebnis zu verbessern und deren Fokus in einer Anwendung zu behalten.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1c04c68b-7a7f-46ae-b750-2b1f79855de4
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1528'
ht-degree: 1%

---

# Übersicht über verbundene Datensatztypen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>   -->

Sie können angeben, dass sich einzelne Datensatztypen gegenseitig oder auf Objekte aus anderen Anwendungen beziehen, indem Sie sie verbinden.

Dieser Artikel bietet eine Übersicht über Verbindungen vom Typ Datensätze und beschreibt die Arten von Verbindungen, die Sie zwischen Datensatz- und Objekttypen herstellen können.

Informationen zum Verbinden von Datensatztypen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

## Überlegungen zum Verbinden von Datensatztypen

Bei der Planung von Workfront gibt es zwei Schritte für Verbindungen:

1. Zunächst müssen Sie eine Verbindung zwischen zwei Datensatztypen oder einem Datensatztyp und einem Objekttyp aus einer anderen Anwendung herstellen. Informationen zum Verbinden von Datensatztypen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
1. Zweitens können Sie einzelne Datensätze eines Typs mit Datensätzen eines anderen Typs verbinden, nachdem die beiden Datensatztypen verbunden wurden. Informationen zum Verbinden von Datensätzen finden Sie unter [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md).

Beachten Sie Folgendes zum Verbinden von Datensatztypen:

* In Adobe Workfront Planning können Sie die folgenden Entitäten verbinden:

   * Zwei Datensatztypen.

     Standardmäßig können Sie zwei Datensatztypen aus demselben Arbeitsbereich verbinden. Sie können auch Datensatztypen einrichten, um eine Verbindung mit Datensatztypen aus anderen Arbeitsbereichen herzustellen. Weitere Informationen finden Sie [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md).
   * Einen Datensatztyp und einen Objekttyp aus einer anderen Anwendung.

* Sie können Workfront Planning-Datensatztypen mit den folgenden Objekttypen aus den folgenden Programmen verbinden:

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
     >Sie müssen über eine Adobe Experience Manager Assets-Lizenz verfügen und die Workfront-Instanz Ihres Unternehmens muss in die Adobe Business Platform oder die Adobe Admin Console integriert sein, um Workfront-Planungsdatensätze mit Adobe Experience Manager Assets zu verbinden.
     >
     >Wenn Sie Fragen zum Onboarding in der Adobe Admin Console haben, lesen Sie die häufig gestellten Fragen zu [Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Nachdem Sie Datensätze für die verbundenen Datensatztypen erstellt haben, können Sie sie über das Feld Verbundener Datensatz miteinander verknüpfen.  Weitere Informationen finden Sie unter [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md).

* Nachdem Sie einen Datensatztyp mit einem anderen Datensatztyp oder mit einem Objekttyp aus einer anderen Anwendung verbunden haben, sind die folgenden Szenarien vorhanden:

   * **Wenn Sie zwei Planning-Datensatztypen verbinden**: Für den Datensatztyp, von dem aus Sie eine Verbindung herstellen, wird ein verknüpftes Datensatzfeld erstellt. Für den Datensatztyp, mit dem Sie eine Verbindung herstellen, wird ein ähnliches verknüpftes Datensatzfeld erstellt.

     Wenn Sie beispielsweise den Datensatztyp „Kampagne“ mit dem Datensatztyp „Produkt“ verbinden, wird ein verknüpftes Datensatzfeld (Verbindungsfeld), das Sie „Verknüpftes Produkt“ nennen, für den Datensatztyp der Kampagne erstellt. Ein verknüpfter Datensatztyp mit der automatischen Bezeichnung „Kampagne“ wird für den Produktdatensatztyp erstellt.

   * **Wenn Sie einen Datensatztyp mit einem Objekttyp aus einer anderen Anwendung verbinden**:

      * Für den Datensatztyp, von dem aus Sie eine Verbindung herstellen, wird ein verknüpftes Datensatzfeld erstellt. Für den Objekttyp des anderen Programms wird automatisch kein verknüpftes Datensatzfeld erstellt.
      * Auf Felder für Planungsdatensätze kann nicht über Workfront-Objekte zugegriffen werden.
      * Die Planungsdatensätze sind auf der Registerkarte Planung des Workfront-Objekts sichtbar. Weitere Informationen finden Sie unter [Verwalten von Datensatzverbindungen aus Workfront-Objekten](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
      * Sie können ein benutzerdefiniertes Feld für die Planning-Verbindung erstellen und es an das benutzerdefinierte Formular eines Workfront-Objekts anhängen. Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
      * Auf Planungs-Datensatzfelder kann über Experience Manager Assets zugegriffen werden, wenn der Workfront-Administrator die Metadatenzuordnung durch die Integration zwischen Workfront und Adobe Experience Manager Assets konfiguriert. Weitere Informationen finden Sie unter &quot;[ der Asset-Metadatenzuordnung zwischen Adobe Workfront und Experience Manager Assets ](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).


   * **Beim Hinzufügen von Suchfeldern aus dem Datensatz oder Objekt, mit dem Sie eine Verbindung herstellen**: Zusätzlich zum Erstellen eines verknüpften Datensatzfelds können Sie auch eine Verbindung zu Feldern aus dem verbundenen Datensatz oder Objekttyp herstellen, die als Suchfelder bezeichnet werden. Ein verknüpftes Feld (oder Suchfeld) mit Informationen aus dem Datensatz, mit dem Sie eine Verbindung herstellen, wird für den Datensatz angezeigt, von dem aus Sie eine Verbindung herstellen.

     Sie können Felder aus anderen Datensatztypen oder den Objekten einer anderen Anwendung mit dem Workfront Planning-Datensatztyp verbinden.

     Verknüpfte Felder sind schreibgeschützt und zeigen automatisch Informationen aus verbundenen Datensätzen an.

     Sie können in Formeln, Filtern oder Gruppierungen auf Suchfelder aus anderen Datensatz- oder Objekttypen verweisen.

     Wenn Sie beispielsweise den Datensatztyp „Kampagne“ mit einem Workfront-Projekt verbinden und auswählen, dass das Feld Geplantes Abschlussdatum des Projekts dem Workfront-Planungsdatensatz hinzugefügt werden soll, wird automatisch ein verknüpftes Feld namens Geplantes Abschlussdatum (aus Projekt) für die Kampagne erstellt. Dieses verknüpfte Feld kann nicht manuell bearbeitet werden. Das Feld Geplantes Abschlussdatum (aus Projekt) zeigt das geplante Abschlussdatum der verknüpften Projekte an.

     >[!IMPORTANT]
     >
     >Alle Personen mit Anzeigen- oder höheren Berechtigungen für den Arbeitsbereich können die Informationen in den Suchfeldern anzeigen, unabhängig von ihren Berechtigungen oder Zugriffsebenen bei der Anwendung der verknüpften Objekttypen oder ihren Berechtigungen in anderen Arbeitsbereichen.

     Verknüpfte Datensatzfelder werden durch ein Beziehungssymbol (Beziehungsfeldsymbol![ vorangestellt](assets/relationship-field-icon.png).

     Verknüpfte Felder werden durch ein Symbol vorangestellt, das den Feldtyp angibt. Beispielsweise werden verknüpften Feldern (oder Suchfeldern) Symbole vorangestellt, die angeben, dass ein Feld eine Zahl, ein Absatz oder ein Datum ist.

     >[!TIP]
     >
     >Die Datumsfeldinformationen der Workfront-Objekte werden in Workfront Planning im 24-Stunden-Format angezeigt, unabhängig davon, wie sie in Workfront angezeigt werden.
     >
     >Wenn beispielsweise das geplante Startdatum eines Projekts in Workfront um 15 :00 angezeigt wird, wird es in Workfront :00 in einem importierten Suchfeld als 15 angezeigt.


## Verbindungstypen

Nachdem Sie eine Verbindung zwischen zwei Datensatztypen oder zwischen einem Datensatz und einem Objekttyp aus einer anderen Anwendung hergestellt haben, können Sie Datensätze in die verbundenen Datensatzfelder einfügen.

Je nachdem, wie viele Datensätze Sie einem verbundenen Datensatzfeld hinzufügen können, können Sie im Folgenden die Verbindungstypen auswählen, aus denen Sie beim Verbinden von Datensatztypen auswählen können:

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
>* Datensatztyp und Experience Manager-Assets

### Viele-zu-viele-Verbindungstyp

![Viele zu viele Verbindungsauswahl](assets/many-to-many-connection-picker.png)

Wenn Sie eine n:n-Verbindung zwischen Datensatztypen erstellen, können Sie mehrere Datensätze im Verbindungsfeld aus beiden Datensatztypen auswählen.

Wenn Sie beispielsweise eine n:n-Verbindung zwischen Kampagnen und Projekten herstellen, können Sie für jede Kampagne mehrere Projekte und für jedes Projekt mehrere Kampagnen auswählen.

Ein reales Beispiel für einen Viele-zu-viele-Beziehungstyp ist die Beziehung zwischen Filmen und Schauspielern. Jeder Film kann mehrere Schauspieler haben, und jeder Schauspieler kann in mehreren Filmen spielen.

Wenn Sie diesen Verbindungstyp auswählen, können Sie den Verbindungstyp nach dem Speichern nicht mehr ändern.

### 1:n-Verbindungstyp

![1:n-Verbindungsauswahl](assets/one-to-many-connection-picker.png)


Wenn Sie eine Eins-zu-Viele-Verbindung zwischen Datensatztypen erstellen, können Sie dann im Verbindungsfeld des aktuellen Datensatztyps mehrere Datensätze auswählen. Das entsprechende Verbindungsfeld im Datensatztyp, mit dem Sie eine Verbindung herstellen, ermöglicht jedoch die Auswahl nur eines Datensatzes. Das verbundene Datensatzfeld, das automatisch für den zweiten Datensatztyp erstellt wird, wird automatisch auf einen Viele-zu-eins-Beziehungstyp eingestellt.

Wenn Sie beispielsweise eine Eins-zu-Viele-Verbindung zwischen Kampagnen und Projekten erstellen, können Sie für jede Kampagne mehrere Projekte auswählen, jedes Projekt kann jedoch nur mit einer Kampagne verbunden werden.

Ein reales Beispiel für eine Eins-zu-viele-Beziehung ist die Beziehung zwischen Bibliotheken und Büchern: Eine Bibliothek hat viele Bücher im Inventar, aber ein bestimmtes Buch kann zu einem bestimmten Zeitpunkt nur in einer Bibliothek sein.

Wenn Sie diesen Verbindungstyp auswählen, können Sie ihn später nur in einen n:n-Verbindungstyp ändern.

### Viele-zu-eins-Verbindung

![Viele zu einer Verbindungsauswahl](assets/many-to-one-connection-picker.png)


Wenn Sie eine n:1-Verbindung zwischen Datensatztypen erstellen, können Sie dann jeden Datensatz im aktuellen Datensatztyp mit nur einem Datensatz aus dem verbundenen Datensatztyp verbinden. Das verbundene Datensatzfeld, das automatisch für den zweiten Datensatztyp erstellt wird, wird automatisch auf einen Eins-zu-Viele-Beziehungstyp eingestellt.

Wenn Sie beispielsweise Kampagnen mit Projekten verbinden und diesen Verbindungstyp auswählen, können Sie einer Kampagne nur ein Projekt hinzufügen. Sie können jedoch mehrere Kampagnen zu einem Projekt hinzufügen.

Ein reales Beispiel für einen Viele-zu-eins-Beziehungstyp ist die Beziehung zwischen vielen Filmen und einem Schauspieler: Ein Schauspieler kann in vielen Filmen sein, aber jeder Film kann nur einen bestimmten Schauspieler einmal in seiner Besetzung haben.

Wenn Sie diesen Verbindungstyp auswählen, können Sie ihn später nur in einen n:n-Verbindungstyp ändern.

### 1:1-Verbindungstyp

![1:1-Verbindungsauswahl](assets/one-to-one-connection-picker.png)

Wenn Sie eine Eins-zu-eins-Verbindung zwischen Datensatztypen erstellen, können Sie in beiden Datensatztypen jeden Datensatz nur mit einem Datensatz aus dem anderen Datensatztyp verbinden.

Wenn Sie beispielsweise Kampagnen mit Projekten verbinden und diesen Verbindungstyp auswählen, können Sie eine Kampagne mit einem Projekt verbinden. Ein Projekt kann nur mit einer Kampagne verbunden werden.

Ein reales Beispiel für eine Eins-zu-eins-Beziehung ist die Beziehung zwischen einer Person und der eindeutigen Kennung ihres Landes (z. B. Sozialversicherungsnummer, Reisepass-ID, lokale Kennung): Jede Person hat nur eine eindeutige Kennung für ein Land und jede eindeutige Kennung kann mit nur einer Person verknüpft werden.

Wenn Sie diesen Verbindungstyp auswählen, können Sie ihn später in einen anderen Verbindungstyp ändern.
