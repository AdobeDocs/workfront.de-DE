---
title: Übersicht über die Verbindungstypen
description: Eine Möglichkeit, anzugeben, wie sich einzelne Datensatztypen zueinander verhalten, besteht darin, sie miteinander zu verbinden. Außerdem können Sie Adobe Workfront Planning-Record-Typen mit Objekttypen aus anderen Anwendungen verbinden, um das Benutzererlebnis zu verbessern und den Fokus in einer Anwendung zu behalten.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 0%

---


<!--update metadata at GA-->
<!--add to TOC and mini TOC when live-->

# Übersicht über die Verbindungstypen

Sie können angeben, dass einzelne Datensatztypen miteinander oder mit Objekten aus anderen Anwendungen in Beziehung stehen, indem Sie sie verbinden.

Dieser Artikel gibt einen Überblick darüber, wie sich Datensätze verbinden, und beschreibt die Verbindungstypen, die Sie zwischen Datensätzen und Objekttypen herstellen können.

Weitere Informationen zum Verbinden von Datensatztypen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

## Überlegungen zum Verbinden von Datensatztypen

* Sie können die folgenden Entitäten in der Adobe Workfront-Planung verbinden:

   * Zwei Datensatztypen

     Die Datensatztypen müssen zum selben Arbeitsbereich gehören.
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

* Nachdem Sie einzelne Datensätze für einen Datensatztyp erstellt haben, können Sie die Datensätze, zu denen Sie eine Verbindung herstellen, aus dem Feld des verknüpften Datensatztyps auswählen. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

* Nachdem Sie einen Datensatztyp mit einem anderen Datensatztyp oder einem Objekttyp aus einer anderen Anwendung verbunden haben, gibt es folgende Szenarien:

   * **Wenn Sie zwei Datensatztypen verbinden**: Ein verknüpftes Datensatzfeld wird für den Datensatztyp erstellt, von dem Sie eine Verbindung herstellen. Ein ähnliches verknüpftes Datensatzfeld wird für den Datensatztyp erstellt, mit dem Sie eine Verbindung herstellen.

     Wenn Sie beispielsweise den Datensatztyp &quot;Kampagne&quot;mit dem Datensatztyp &quot;Produkt&quot;verbinden, wird ein verknüpftes Datensatzfeld, das Sie &quot;Verknüpftes Produkt&quot;nennen, im Datensatztyp &quot;Kampagne&quot;erstellt. Ein verknüpfter Datensatztyp, der automatisch &quot;Kampagne&quot;heißt, wird für den Produktdatensatztyp erstellt.

   * **Wenn Sie einen Datensatztyp mit einem Objekttyp aus einer anderen Anwendung verbinden**:

      * Ein verknüpftes Datensatzfeld wird für den Datensatztyp erstellt, aus dem Sie eine Verbindung herstellen. Für den Objekttyp der anderen Anwendung wird kein verknüpftes Datensatzfeld erstellt.

      * Über Workfront-Objekte ist der Zugriff auf die Felder für die Planung von Datensätzen nicht möglich.
      * Die Planung von Datensatzfeldern ist über Experience Manager-Assets verfügbar, wenn der Workfront-Administrator die Metadaten-Zuordnung durch die Integration zwischen Workfront und Adobe Experience Manager Assets konfiguriert. Weitere Informationen finden Sie unter [Konfigurieren der Asset-Metadatenzuordnung zwischen Adobe Workfront und Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

   * **Wenn Sie verknüpfte (oder Nachschlagefelder) Felder aus dem Datensatz oder Objekt hinzufügen, mit dem Sie eine Verbindung herstellen, wird ein verknüpftes (oder Nachschlagefeld) mit Informationen aus dem Datensatz, mit dem Sie eine Verbindung herstellen, in dem Datensatz angezeigt, von dem Sie eine Verbindung herstellen.**

     Sie können Felder von anderen Datensatztypen oder von Objekten einer anderen Anwendung mit dem Datensatztyp für die Workfront-Planung verbinden.

     Verknüpfte Felder sind schreibgeschützt und zeigen automatisch Informationen aus verbundenen Datensätzen oder Objekten an, wenn Sie die Datensätze oder Objekte verbinden.

     Wenn Sie beispielsweise den Datensatztyp &quot;Kampagne&quot;mit einem Workfront-Projekt verbinden und das Feld &quot;Geplantes Abschlussdatum&quot;des Projekts in den Workfront-Planungsdatensatz übertragen möchten, wird automatisch ein verknüpftes Feld namens &quot;Geplantes Abschlussdatum&quot;(aus Projekt) für die Kampagne erstellt. Sie können dieses verknüpfte Feld nicht manuell bearbeiten. Im Feld Geplantes Abschlussdatum (aus Projekt) wird das geplante Abschlussdatum der verknüpften Projekte angezeigt.

     >[!IMPORTANT]
     >
     >Jeder Benutzer mit der Berechtigung Anzeigen oder höher für den Arbeitsbereich kann die Informationen in den verknüpften Feldern anzeigen, unabhängig von seinen Berechtigungen oder Zugriffsrechten in der Anwendung der verknüpften Objekttypen.

* Verknüpfte Datensatzfelder erhalten das Beziehungssymbol ![](assets/relationship-field-icon.png).

  Verknüpfte Felder erhalten ein Symbol, das den Feldtyp identifiziert. Verknüpfte (oder Lookup-) Felder weisen beispielsweise Symbole darauf hin, dass es sich bei einem Feld um eine Zahl, einen Absatz oder ein Datum handelt.

* Suchfelder wird ein Symbol vorangestellt, das den Typ der im Feld angezeigten Informationen angibt.

## Verbindungstypen

Nachdem Sie eine Verbindung zwischen zwei Datensatztypen oder zwischen einem Datensatz und einem Objekttyp aus einer anderen Anwendung hergestellt haben, können Sie in den verbundenen Datensatzfeldern Datensätze hinzufügen.

Je nachdem, wie viele Datensätze Sie einer Verbindung hinzufügen können, stehen Ihnen beim Verbinden von Datensatztypen folgende Verbindungstypen zur Verfügung:

* [Eins bis viele](#one-to-many-connection-type)
* [Eins bis eins](#many-to-one-connection-type)
* [Viele bis eins](#many-to-one-connection-type)
* [Viele bis viele](#many-to-many-connection-type)

<!-- add screen shots for each type of connection below-->

### Eins-zu-viele-Verbindungstyp

Wenn Sie den 1:n-Verbindungstyp zwischen Datensatztypen auswählen, können Sie später einen Datensatz mit mehreren Datensätzen verbinden, mit denen Sie eine Verbindung herstellen möchten.

Wenn Sie beispielsweise Kampagnen mit Projekten verbinden, können Sie eine Kampagne mit mehreren Projekten verbinden. Ein Projekt kann jedoch nur mit einer Kampagne verbunden werden.

Wenn Sie diesen Verbindungstyp auswählen, können Sie ihn später nur in einen Verbindungstyp vom Typ Viele-zu-viele ändern.

### Eins-zu-Eins-Verbindungstyp

Wenn Sie den Eins-zu-Eins-Verbindungstyp zwischen Datensätzen auswählen, können Sie später einen Datensatz mit einem anderen Datensatz verbinden, mit dem Sie eine Verbindung herstellen.

Wenn Sie beispielsweise Kampagnen mit Projekten verbinden, können Sie eine Kampagne mit einem Projekt verbinden. Ein Projekt kann nur mit einer Kampagne verbunden werden.

Wenn Sie diesen Verbindungstyp auswählen, können Sie ihn später in einen anderen Verbindungstyp ändern.

### Viele-zu-eins-Verbindungstyp

Wenn Sie zwischen den Datensatztypen den Verbindungstyp n:1 auswählen, können Sie später viele Datensätze mit nur einem Datensatz verbinden, mit dem Sie eine Verbindung herstellen.

Wenn Sie beispielsweise Kampagnen mit Projekten verbinden, können Sie mehrere Kampagnen mit einem Projekt verbinden. Ein Projekt kann mit mehreren Kampagnen verbunden werden.

Wenn Sie diesen Verbindungstyp auswählen, können Sie ihn später nur in einen Verbindungstyp vom Typ Viele-zu-viele ändern.

### Viele-zu-viele-Verbindungstyp

Wenn Sie den Verbindungstyp Viele-zu-viele zwischen Datensätzen auswählen, können Sie später viele Datensätze mit mehreren Datensätzen verbinden, mit denen Sie eine Verbindung herstellen möchten.

Wenn Sie beispielsweise Kampagnen mit Projekten verbinden, können Sie mehrere Kampagnen mit mehreren Projekten verbinden. Sie können auch mehrere Projekte mit mehreren Kampagnen verbinden.

Wenn Sie diesen Verbindungstyp auswählen, können Sie den Verbindungstyp nach dem Speichern nicht mehr ändern.