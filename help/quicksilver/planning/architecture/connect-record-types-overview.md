---
title: Übersicht über Connected Record Types
description: Eine Möglichkeit, anzugeben, wie sich einzelne Datensatztypen zueinander verhalten, besteht darin, sie miteinander zu verbinden. Außerdem können Sie Adobe Workfront Planning-Record-Typen mit Objekttypen aus anderen Anwendungen verbinden, um das Benutzererlebnis zu verbessern und den Fokus in einer Anwendung zu behalten.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 0%

---


<!--update metadata at GA-->
<!--add mini TOC when live, already added to big TOC to get the link-->

# Übersicht über verbundene Datensatztypen

<!--REMOVE THE CONTENT BELOW FROM THE "CONNECT RECORD TYPES" ARTICLE WHEN YOU TURN THIS ARTICLE LIVE- THIS IS THE SAME CONTENT AS THERE, DUPLICATED-->

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
      * Die Planung von Datensatzfeldern ist über Experience Manager-Assets verfügbar, wenn der Workfront-Administrator die Metadaten-Zuordnung durch die Integration zwischen Workfront und Adobe Experience Manager Assets konfiguriert. Weitere Informationen finden Sie unter [Konfigurieren der Asset-Metadatenzuordnung zwischen Adobe Workfront und Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
      * Auf der Registerkarte Planung des Workfront-Objekts werden Planungsdatensätze angezeigt. Weitere Informationen finden Sie unter [Verwalten von Datensätzen im Abschnitt &quot;Planung&quot;von Adobe Workfront-Objekten](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

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

<!--## Connection types

After you establish a connection between two record types or between a record and an object type from another application, you can add records in the connected record fields. 

Depending on how many records you can add to a connected record field, the following are the connection types you can choose from when connecting record types: 

* [Many to many](#many-to-many-connection-type)
* [One to many](#one-to-many-connection-type)
* [Many to one](#many-to-one-connection-type)
* [One to one](#many-to-one-connection-type)

>[!WARNING]
>
>These options are not available when connecting the following: 
>* Two records from different workspaces
>
>* A record type and Experience Manager assets

### Many-to-many connection type

![](assets/many-to-many-connection-picker.png)

When you create a many-to-many connection between record types, you can then select multiple records in the connection field from both record types. 

For example, if you create a many-to-many connection between campaigns and projects, you can select multiple projects for each campaign, and multiple campaigns for each project. 

A real-life example of a many-to-many relationship type is the relationship between movies and actors. Each movie can have multiple actors, and each actor can play in multiple movies. 

When you select this connection type, you cannot change the connection type after you save it. 

### One-to-many connection type

![](assets/one-to-many-connection-picker.png)


When you create a one-to-many connection between record types, you can then select multiple records in the connection field in the current record type, but the corresponding connection field in the record type you connect to will allow selecting only one record. The connected record field that is automatically created on the second record type is automatically set to a many-to-one relationship type. 

For example, if you create a one-to-many connection between campaigns and projects, you can select multiple projects for each campaign, but each project can be connected to only one campaign.

A real-life example of a one-to-many relationship type is the relationship between libraries and books: a library has many books in its inventory; but one particular book can only be in one library at a given point in time. 

When you select this connection type, you can later change it only to a many-to-many connection type. 

### Many-to-one connection type

![](assets/many-to-one-connection-picker.png)


When you create a many-to-one connection between record types, you can then connect each record in the current record type with only one record from the connected record type. The connected record field that is automatically created on the second record type is automatically set to a one-to-many relationship type. 

For example, if you connect campaigns with projects and you choose this type of connection, you can add only one project to a campaign. But you can add multiple campaigns to one project. 

A real-life example of a many-to-one relationship type is the relationship between many movies and one actor: one actor can be in many movies, but each movie can only have a specific actor once in its cast. 

When you select this connection type, you can later change it only to a many-to-many connection type.

### One-to-one connection type

![](assets/one-to-one-connection-picker.png)

When you create a one-to-one connection between record types, in both record types you can connect each record only with one record from the other record type.

For example, if you connect campaigns with projects and you choose this type of connection, you can connect one campaign with one project. One project can be connected only to one campaign. 

A real-life example of a one-to-one relationship is the one existing between a person and their country's unique identifier (like a Social Security Number, Passport ID, local identification ID): each person has only one unique identifier for a country and each unique identifier can be linked to only one person. 

When you select this connection type, you can later change it to any other connection type. 

-->



