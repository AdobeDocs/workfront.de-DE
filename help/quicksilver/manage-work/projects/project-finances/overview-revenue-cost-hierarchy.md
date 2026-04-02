---
content-type: overview
product-area: projects
navigation-topic: financials
title: Übersicht über Umsatz und Kostenhierarchie
description: In diesem Artikel wird der Schritt-für-Schritt-Prozess zur Bestimmung der geeigneten Abrechnungs- und Kostensätze für Aufgabengebiete und Benutzer für die Umsatzart und den Kostentyp „Benutzer und Funktion pro Stunde“ beschrieben.
author: Lisa
feature: Work Management
source-git-commit: dfc6344303f33a9c3c89837b759235612e54904e
workflow-type: tm+mt
source-wordcount: '3519'
ht-degree: 0%

---

# Übersicht über Umsatz- und Kostenhierarchie

{{highlighted-preview-article-level}}

{{ultimate-package}}

Um präzise Finanzberechnungen zu ermöglichen, verwendet Workfront bei der Berechnung des Umsatzes einer Aufgabe oder eines Projekts die entsprechenden Abrechnungssätze. Aufgabengebiet und Benutzerraten müssen auf allen Ebenen klar definiert sein, um genaue finanzielle Berechnungen zu ermöglichen.

In den Abschnitten dieses Artikels wird der schrittweise Prozess zur Bestimmung der geeigneten Abrechnungs- und Kostensätze für Aufgabengebiete und Benutzer für die Umsatzart „Benutzer und Funktion pro Stunde“ und die Kostentypliste beschrieben.

Weitere Informationen zu Abrechnungssätzen, Umsatztypen und zur Berechnung des Umsatzes finden Sie unter [Übersicht über Abrechnung und Umsatz](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Übersicht über die Wirksamkeitsdaten

Workfront-Administratoren können optional Gültigkeitsdaten festlegen, die bestimmen, wann Abrechnungssätze, Kostensätze und andere Finanzattribute im System wirksam werden. Beispielsweise könnte ein Aufgabengebiet oder ein Benutzer einen standardmäßigen Abrechnungssatz von 50 $ haben. Bei Anwendung des effektiven Datums könnte dieser 50-Dollar-Satz am 31. März auslaufen, und ein neuer Satz von 55 US-Dollar würde automatisch am 1. April beginnen.

Bei Berechnungen des geplanten Umsatzes basieren die Abrechnungssätze auf dem Datum der geplanten Stunden. Die geplanten Stunden werden gleichmäßig über die Aufgabendauer verteilt. Im vorherigen Beispiel wird für Stunden, die für den 31. März oder früher geplant sind, der Tarif von 50 USD verwendet, und für Stunden, die für den 1. April oder später geplant sind, der Tarif von 55 USD.

Bei Berechnungen des tatsächlichen Umsatzes basieren die Abrechnungssätze auf dem Datum für die protokollierten Stunden. Im vorherigen Beispiel verwenden Stunden, die am 31. März oder früher erfasst wurden, den Tarif von 50 USD, und Stunden, die am 1. April oder später erfasst wurden, den Tarif von 55 USD.

>[!NOTE]
>
>Aufgabenzuweisungen werden nicht mit einem Gültigkeitsdatum definiert. Stattdessen werden die anwendbaren Tarife durch Arbeitsaufträge aus dem System abgerufen, unabhängig davon, ob es sich um eine Tarifkarte, ein Benutzerprofil oder eine Überschreibung auf Arbeitsauftragsebene handelt. Wirksamkeitsdaten stellen sicher, dass der richtige Satz basierend auf dem Zeitpunkt der Arbeit angewendet wird, aber sie definieren die Zuweisungen nicht direkt.

## Übersicht über das Aufgabengebiet für die Abrechnung

Ein **Aufgabengebiet für die Abrechnung** wird für einen Benutzer auf Zuordnungs- oder Projektebene festgelegt. Sie gilt nur für Benutzende und kann nicht für andere Aufgabengebiete verwendet werden. Das Aufgabengebiet eines/r Benutzenden ist beispielsweise in erster Linie Designer, fungiert jedoch bei einer Aufgabe oder einem Projekt als Senior Designer und die Quote sollte dies widerspiegeln.

Ein Aufgabengebiet auf Arbeitsauftragsebene für die Fakturierung ist nur für diese spezifische Zuweisung bestimmt und wird nicht automatisch auf die anderen Zuweisungen des Benutzers angewendet. Ein Aufgabengebiet auf Projektebene für die Fakturierung gilt für alle Zuweisungen des Benutzers zu diesem Projekt. Sie können sie bei Bedarf auf individueller Zuweisungsebene überschreiben.

Wenn ein Aufgabengebiet für die Fakturierung auf Benutzerzuweisung- oder Projektebene angewendet wird, kann in Umsatzberechnungen der mit dem Aufgabengebiet für die Fakturierung verknüpfte Satz anstelle der Sätze „Benutzer“ oder „Aufgabengebiet“ verwendet werden. Das Aufgabengebiet für die Fakturierung ist nur verfügbar, wenn der Umsatztyp Benutzer und Funktion Stündlich verwendet wird.

>[!NOTE]
>
>Während ein(e) Benutzende(r) für Abrechnungszwecke möglicherweise mit einer anderen Rolle agiert, verwenden Kostenberechnungen weiterhin sein/ihr primäres Aufgabengebiet. Das Aufgabengebiet für die Abrechnung wirkt sich nur auf Abrechnungsberechnungen aus.

Weitere Informationen finden Sie unter [Einrichten eines Aufgabengebiets für die Abrechnung](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md).

## Überblick über die konservierten Zinssätze

Die Markierung **Projekt-Abrechnungssatzinformationen beibehalten** für ein Projekt steuert, ob das System die Abrechnungsinformationen für Zuweisungen zum Zeitpunkt der Fertigstellung der Tarifkarte verwendet oder ob Änderungen aufgrund von Änderungen während des Projektverlaufs zulässig sind. Änderungen am Aufgabengebiet, Gehalt, Tarifkarte oder anderen abrechnungsbezogenen Informationen des Benutzers wirken sich nicht auf die Abrechnungssätze für Zuweisungen aus. Die Tarife werden gemäß der endgültigen Tarifkarte zum Zeitpunkt der Aktivierung der Projekt-Markierung beibehalten. Diese Zuweisungseigenschaften (z. B. Aufgabengebiet und Gehalt) werden weiterhin aktualisiert, um sicherzustellen, dass die tatsächlichen Kosten der Zuweisung korrekt sind.

Wenn die Markierung aktiviert ist, sperrt das System die datumswirksamen Abrechnungssätze (die auf der endgültigen Tarifkarte festgelegt sind, die dem Projekt beigefügt ist) für die Dauer des Projekts.

Die Markierung kann für ein Projekt aktiviert werden, wenn die Arbeit begonnen hat und Zuweisungen und Stunden bereits vorhanden sind. Zu diesem Zeitpunkt:

* Der endgültige Kartensatz „Genehmigt“ wird zur Quelle der Abrechnungssätze für alle Projektzuweisungen.
* Alle früheren, aktuellen und künftigen Zuweisungen werden anhand der endgültig genehmigten Sätze neu berechnet.
* Die tatsächlichen und geplanten Werte werden neu berechnet.

>[!NOTE]
>
>Sobald die Markierung aktiviert ist, um die Verrechnungssätze beizubehalten, kann sie nicht mehr deaktiviert werden, es sei denn, das Projekt verfügt über keine Zuweisungen und keine Stunden. Dadurch wird sichergestellt, dass alle Finanzberichte die tatsächlichen vertraglichen Kurse widerspiegeln.
>Wenn die Markierung deaktiviert ist, können die Abrechnungssätze vom System neu berechnet oder dynamisch angepasst werden. Jegliche Aktualisierungen der Rolle, des Gehalts oder des Abrechnungssatzes des Benutzers werden sofort im Abrechnungssatz für die Zuweisung angezeigt.

Weitere Informationen finden Sie unter [Projekte ](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) und [Tarifkarten verwalten](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Geplanter Umsatz - Benutzer und Funktion pro Stunde

Wenn für die Aufgabe der Umsatztyp „Benutzer und Funktion - Stündlich“ festgelegt ist, verwendet Workfront zum Bestimmen des Abrechnungssatzes für den geplanten Umsatz sowohl die Benutzer- als auch die Aufgabenrollensatzhierarchie.

Dieses Bild zeigt den Fluss der geplanten Umsatzhierarchie:

![Geplanter Umsatz für Benutzer und Funktion, Umsatztyp „Stündlich“](assets/planned-revenue-chart.png)

Wenn ein(e) Benutzende(r) der Aufgabe zugewiesen wird, sucht Workfront gemäß dieser Hierarchie:

1. Das System sucht zunächst nach einer Rate, die für den Benutzer bei der Zuweisung beibehalten wurde.

   Eine gespeicherte Rate folgt weiterhin der Hierarchie, die Rate wird jedoch eingefroren, wenn das Projekt beibehalten wird. Weitere Informationen finden Sie unter [Übersicht über die Einbehaltungssätze](#overview-of-preserved-rates).

1. Als Nächstes sucht das System auf einer Tarifkarte nach dem Abrechnungssatz für das primäre Aufgabengebiet oder das Aufgabengebiet für die Abrechnung des Benutzers, der der Aufgabe zugewiesen wurde. Wenn ein Satz existiert und gesperrt ist, wird dieser Satz in der Umsatzberechnung verwendet.

   Wenn ein Tarif auf der Tarifkarte vorhanden ist und diese entsperrt ist, verwendet das System diesen Tarif nicht und sucht nach dem nächsten Tarif in der Hierarchie.

1. Als Nächstes sucht das System nach der Überschreibungsrate auf Zuweisungsebene für den Benutzer. Dies ist ein manuell hinzugefügter Tarif, der an die spezifische Zuweisung gebunden ist, und überschreibt alle anderen Tarife für den Benutzer für diese Zuweisung (mit Ausnahme eines gesperrten Tarifs für Tarifkarten). Wenn ein Satz gefunden wird, wird dieser Satz in der Umsatzberechnung verwendet.
1. Anschließend sucht das System nach einem Aufgabengebiet für die Fakturierung auf Aufgabenzuweisungsebene.

   Das Aufgabengebiet für die Fakturierung gilt nur für eine bestimmte Zuweisung und für die Zuweisung anstelle des primären Aufgabengebiets des Benutzers. Das Aufgabengebiet einer Benutzerin oder eines Benutzers ist beispielsweise Designer, in einer Aufgabe agiert sie jedoch als Senior Designer mit einem höheren Abrechnungssatz.

   Workfront sucht nach dem Aufgabengebiet für Abrechnungssatz:

   * Das System sucht zunächst nach dem Abrechnungssatz des Aufgabengebiets für die Abrechnung aus der Zuweisung (im Beispiel Senior Designer) und berücksichtigt dabei die tatsächlichen Daten. Sie sehen dies im Bereich „Sätze“ > „Abrechnung“ des Projekts in einer **Source: Überschreibungen > Ressourcentyp: Aufgabengebiet** Gruppierung. Dies ist ein Überschreibungssatz für das Projekt.
   * Als Nächstes sucht das System über eine Tarifkarte nach dem Aufgabengebiet für den Abrechnungssatz und berücksichtigt dabei die Wirksamkeitsdaten. Sie sehen dies im Bereich „Sätze“ > „Abrechnung“ des Projekts in einer **Tarifkarte: Angehängte Tarifkarte > Ressourcentyp: Aufgabengebiet** Gruppierung.
   * Wenn der Satz für das Aufgabengebiet für die Fakturierung nicht im Projekt oder auf der Tarifkarte angegeben ist, sucht das System nach dem Satz für das Aufgabengebiet auf Systemebene (im Beispiel „Senior Designer„), wobei die Gültigkeitsdaten berücksichtigt werden.
   * Wenn ein Aufgabengebiet für die Abrechnung zugewiesen ist und keiner der Sätze aus den vorherigen Schritten gefunden wird, ist der Abrechnungssatz 0.

     >[!NOTE]
     >
     >Wenn ein Aufgabengebiet für die Abrechnung zugewiesen wird, der Abrechnungssatz jedoch 0 ist, ist dies ein Indikator, um die Tarifeinrichtung erneut aufzurufen. Eine Rate von 0 bedeutet, dass keine Raten für dieses Aufgabengebiet (im Beispiel Senior Designer) in Workfront eingerichtet wurden. Sie sollten entweder Tarife für das Aufgabengebiet hinzufügen oder das Aufgabengebiet für die Fakturierung aus der Zuweisung löschen.
     >
     >Da Aufgaben Aufgabenrollensätze vom Projekt erben, wenn diese Sätze auf Projektebene verfügbar sind, wurden alle Sätze bei der Suche nach dem Aufgabengebiet für die Fakturierung auf Projektebene bereits gefunden, als Workfront nach dem Aufgabengebiet für die Fakturierung auf Aufgabenzuordnungsebene gesucht hat. Die Suche auf Projektebene nach einem Aufgabengebiet für die Fakturierung verbleibt weiterhin in der Suchhierarchie.

1. Wenn ein Aufgabengebiet für die Fakturierung auf der Aufgabenzuordnungsebene nicht verfügbar war, sucht das System dann nach dem Abrechnungssatz für das Projekt für den spezifischen Benutzer, der der Aufgabe zugewiesen wurde, wobei Datumsangaben für das Wirksamwerden berücksichtigt werden. Dies wird im Bereich „Sätze“ > „Abrechnung“ des Projekts in einer Gruppierung &quot;**Source: Überschreibungen > Ressourcentyp: Benutzer** angezeigt. Dies ist ein Überschreibungssatz für das Projekt.
1. Als Nächstes sucht das System nach dem Abrechnungssatz auf Systemebene im Benutzerprofil, wobei die tatsächlichen Daten berücksichtigt werden.
1. Als Nächstes sucht das System nach dem Abrechnungssatz für das primäre Aufgabengebiet des Benutzers (im Beispiel Designer).

   * Das System sucht zunächst nach dem Abrechnungssatz für das Projekt für das primäre Aufgabengebiet des Benutzers und berücksichtigt dabei die tatsächlichen Daten. Sie sehen dies im Bereich „Sätze“ > „Abrechnung“ des Projekts in einer **Source: Überschreibungen > Ressourcentyp: Aufgabengebiet** Gruppierung. Dies ist ein Überschreibungssatz für das Projekt.
   * Als Nächstes sucht das System auf einer Tarifkarte nach dem Tarif für das Aufgabengebiet und berücksichtigt dabei das Datum des In-Kraft-Tretens. Sie sehen dies im Bereich „Sätze“ > „Abrechnung“ des Projekts in einer **Tarifkarte: Angehängte Tarifkarte > Ressourcentyp: Aufgabengebiet** Gruppierung.
   * Als Nächstes sucht das System nach der Aufgabengebiet-Quote auf Systemebene, wobei Datumsangaben für die Gültigkeit berücksichtigt werden.

1. Wenn keiner dieser Sätze gefunden wird, ist der Abrechnungssatz 0.

Wenn ein(e) Benutzende(r) der Aufgabe nicht zugewiesen ist, durchsucht Workfront die Vorgangsrollensätze gemäß dieser Hierarchie:

1. Das System sucht zunächst nach einer Rate mit Beibehaltung in der Zuweisung für das Aufgabengebiet.
1. Das System sucht auf einer Tarifkarte nach dem Abrechnungssatz für das der Aufgabe zugewiesene Aufgabengebiet. Wenn ein Satz existiert und gesperrt ist, wird dieser Satz in der Umsatzberechnung verwendet.

   Wenn ein Tarif auf der Tarifkarte vorhanden ist und diese entsperrt ist, verwendet das System diesen Tarif nicht und sucht nach dem nächsten Tarif in der Hierarchie.

1. Als Nächstes sucht das System nach der Überschreibungsrate für Zuweisungsaufgaben für das Aufgabengebiet. Dies ist ein manuell hinzugefügter Satz für das Aufgabengebiet für die spezifische Zuweisung und überschreibt alle anderen Sätze für das Aufgabengebiet für diese Aufgabe. Wenn ein Satz gefunden wird, wird dieser Satz in der Umsatzberechnung verwendet.
1. Als Nächstes sucht das System nach dem Abrechnungssatz für das Aufgabengebiet, das der Aufgabe zugewiesen wurde.

   * Das System sucht zunächst nach dem Abrechnungssatz für das Projekt für das Aufgabengebiet und berücksichtigt dabei die tatsächlichen Daten. Sie sehen dies im Bereich „Sätze“ > „Abrechnung“ des Projekts in einer **Source: Überschreibungen > Ressourcentyp: Aufgabengebiet** Gruppierung. Dies ist ein Überschreibungssatz für das Projekt.
   * Als Nächstes sucht das System auf einer Tarifkarte nach dem Tarif für das Aufgabengebiet und berücksichtigt dabei das Datum des In-Kraft-Tretens. Sie sehen dies im Bereich „Sätze“ > „Abrechnung“ des Projekts in einer **Tarifkarte: Angehängte Tarifkarte > Ressourcentyp: Aufgabengebiet** Gruppierung.
   * Als Nächstes sucht das System nach der Aufgabengebiet-Quote auf Systemebene, wobei Datumsangaben für die Gültigkeit berücksichtigt werden.

1. Wenn keiner dieser Sätze gefunden wird, ist der Abrechnungssatz 0.

## Tatsächlicher Umsatz - Benutzer und Funktion pro Stunde

Wenn für die Aufgabe der Umsatztyp „Benutzer und Funktion - Stündlich“ festgelegt ist, verwendet Workfront zwei Hierarchien, um den Abrechnungssatz für den tatsächlichen Umsatz zu bestimmen. Der Abrechnungssatz basiert auf den Stunden, die Benutzende für eine Aufgabe protokollieren.

Der „Benutzer“ in den Hierarchien ist die Person, die der Aufgabe zugewiesen wurde. Der „Besitzer“ ist die Person, deren Zeit für die Aufgabe protokolliert wird, auch wenn sie der Aufgabe nicht zugewiesen ist. Zum Beispiel wird Michael eine Aufgabe zugewiesen, aber Joanna schließt die Arbeit ab, weil Michael krank war. Der Manager kann die Zeit für die Aufgabe protokollieren und den Besitzer der protokollierten Stunden auf Joanna festlegen. Die Werte für den geplanten Umsatz basieren auf der Zuweisung und dem Satz von Michael in der Hierarchie, aber die tatsächlichen Umsatzwerte basieren auf dem Satz von Joanna.

Dieses Bild zeigt den Fluss der tatsächlichen Umsatzhierarchie:

![Tatsächlicher Umsatz für Kostentyp „Benutzer und Funktion pro Stunde“](assets/actual-revenue-chart.png)

### Wenn der Eigentümer der protokollierten Stunden und der der Aufgabe zugewiesene Benutzer identisch sind

Workfront sucht zunächst nach einem Abrechnungssatz anhand der Benutzerzuweisung. Wenn ein(e) Benutzende(r) der Aufgabe nicht zugewiesen ist, sucht er/sie anhand der Aufgabenrollenzuweisung nach einem Abrechnungssatz.

Die Hierarchie für dieses Szenario entspricht der geplanten Umsatzhierarchie. Siehe [Geplanter Umsatz - Benutzer und Funktion pro Stunde](#planned-revenue--user-and-role-hourly) für diesen Workflow.

### Wenn der Eigentümer der protokollierten Stunden nicht der zugewiesene Benutzer der Aufgabe ist

Workfront sucht in den Benutzereigenschaften des Eigentümers entsprechend dieser Hierarchie:

1. Das System sucht zunächst nach einem Erhaltungssatz für die Zuweisung für den Eigentümer.
1. Als Nächstes sucht das System auf einer Tarifkarte nach dem Abrechnungssatz für das primäre Aufgabengebiet des Eigentümers. Wenn ein Satz existiert und gesperrt ist, wird dieser Satz in der Umsatzberechnung verwendet.

   Wenn ein Tarif auf der Tarifkarte vorhanden ist und diese entsperrt ist, verwendet das System diesen Tarif nicht und sucht nach dem nächsten Tarif in der Hierarchie.

1. Als Nächstes sucht das System nach dem Abrechnungssatz für das Projekt für den Eigentümer, wobei die tatsächlichen Daten berücksichtigt werden. Sie sehen dies im Bereich „Sätze“ > „Abrechnung“ des Projekts in einer &quot;Source: Überschreibungen“ > „Ressourcentyp: Benutzergruppe“. Dies ist ein Überschreibungssatz für das Projekt.
1. Anschließend sucht das System nach einem Aufgabengebiet für die Fakturierung auf Projektebene.

   Das Aufgabengebiet für die Fakturierung ist nur für ein bestimmtes Projekt und gilt für das Projekt anstelle des primären Aufgabengebiets des Eigentümers. Das Aufgabengebiet des Eigentümers ist beispielsweise in erster Linie Designer, in einem Projekt fungieren sie jedoch als Senior Designer mit einem höheren Abrechnungssatz.

   Workfront sucht nach dem Aufgabengebiet für Abrechnungssatz:

   * Das System sucht zunächst auf einer Tarifkarte nach dem Aufgabengebiet für den Abrechnungssatz, wobei die tatsächlichen Daten berücksichtigt werden. Sie sehen dies im Bereich „Sätze“ > „Abrechnung“ des Projekts in einer **Tarifkarte: Angehängte Tarifkarte > Ressourcentyp: Aufgabengebiet** Gruppierung.
   * Wenn der Tarif für das Aufgabengebiet „Abrechnung“ nicht auf der Tarifkarte angegeben ist, sucht das System nach dem Tarif für das Aufgabengebiet auf Systemebene (im Beispiel „Senior Designer„), wobei die Gültigkeitsdaten berücksichtigt werden.
   * Wenn ein Aufgabengebiet für die Abrechnung zugewiesen ist und keiner der Sätze aus den vorherigen Schritten gefunden wird, ist der Abrechnungssatz 0.

     >[!NOTE]
     >
     >Wenn ein Aufgabengebiet für die Abrechnung zugewiesen wird, der Abrechnungssatz jedoch 0 ist, ist dies ein Indikator, um die Tarifeinrichtung erneut aufzurufen. Eine Rate von 0 bedeutet, dass keine Raten für dieses Aufgabengebiet (im Beispiel Senior Designer) in Workfront eingerichtet wurden. Sie sollten entweder Sätze für das Aufgabengebiet hinzufügen oder das Aufgabengebiet für die Fakturierung aus dem Projekt löschen.

1. Als Nächstes sucht das System nach dem Abrechnungssatz auf Systemebene im Benutzerprofil des Eigentümers, wobei die tatsächlichen Daten berücksichtigt werden.
1. Als Nächstes sucht das System nach dem Abrechnungssatz für das primäre Aufgabengebiet des Eigentümers (im Beispiel Designer).

   * Das System sucht zunächst nach dem Abrechnungssatz für das Projekt für das primäre Aufgabengebiet des Verantwortlichen, wobei Datumsangaben für das Wirksamwerden berücksichtigt werden. Sie sehen dies im Bereich „Sätze“ > „Abrechnung“ des Projekts in einer **Source: Überschreibungen > Ressourcentyp: Aufgabengebiet** Gruppierung. Dies ist ein Überschreibungssatz für das Projekt.
   * Als Nächstes sucht das System auf einer Tarifkarte nach dem Tarif für das Aufgabengebiet und berücksichtigt dabei das Datum des In-Kraft-Tretens. Sie sehen dies im Bereich „Sätze“ > „Abrechnung“ des Projekts in einer **Tarifkarte: Angehängte Tarifkarte > Ressourcentyp: Aufgabengebiet** Gruppierung.
   * Als Nächstes sucht das System nach der Aufgabengebiet-Quote auf Systemebene, wobei Datumsangaben für die Gültigkeit berücksichtigt werden.

1. Wenn keiner dieser Sätze gefunden wird, ist der Abrechnungssatz 0.

## Geplante Kosten - Benutzer und Funktion pro Stunde

Wenn für die Aufgabe der Kostentyp „Benutzer und Funktion pro Stunde“ festgelegt ist, verwendet Workfront zum Bestimmen des Satzes für geplante Kosten sowohl Benutzende als auch Aufgabengebiets-Hierarchien.

Dieses Bild zeigt den Ablauf der geplanten Kostenhierarchie:

![Geplante Kosten für Benutzer- und Funktionskostentyp pro Stunde](assets/planned-cost-chart.png)

Wenn ein(e) Benutzende(r) der Aufgabe zugewiesen wird, sucht Workfront gemäß dieser Hierarchie:

1. Das System sucht nach der Überschreibungsrate für die Zuweisungsaufgabe für den Benutzer. Dies ist ein manuell hinzugefügter Satz für den Benutzer für die spezifische Zuweisung und überschreibt alle anderen Sätze für den Benutzer für diese Aufgabe. Wenn ein Satz gefunden wird, wird dieser Satz in der Kostenberechnung verwendet.
1. Als Nächstes sucht das System nach dem Kostensatz für das Projekt für den spezifischen Benutzer, der der Aufgabe zugewiesen wurde, unter Berücksichtigung des effektiven Datums. Dies wird im Bereich „Sätze“ > „Kosten“ des Projekts in einer Gruppierung &quot;**: Überschreibungen“ > „Ressourcentyp: Benutzer** angezeigt. Dies ist ein Überschreibungssatz für das Projekt.
1. Als Nächstes sucht das System nach dem Kostensatz auf Systemebene für das Benutzerprofil und berücksichtigt dabei die tatsächlichen Daten.
1. Als Nächstes sucht das System basierend auf der Attributbewertung nach der Kostensatz für das primäre Aufgabengebiet des Benutzers mit der Kombination der zugewiesenen Attribute.
1. Wenn keiner dieser Sätze gefunden wird, ist der Kostensatz 0.

Wenn ein(e) Benutzende(r) der Aufgabe nicht zugewiesen ist, durchsucht Workfront die Kostensätze für Aufgabengebiete gemäß dieser Hierarchie:

1. Das System sucht nach der Überschreibungsrate für die Zuweisungsaufgabe für das Aufgabengebiet. Dies ist ein manuell hinzugefügter Satz für das Aufgabengebiet für die spezifische Zuweisung und überschreibt alle anderen Sätze für das Aufgabengebiet für diese Aufgabe. Wenn ein Satz gefunden wird, wird dieser Satz in der Kostenberechnung verwendet.
1. Als Nächstes sucht das System nach dem Kostensatz für Aufgabengebiete auf Systemebene mit der Kombination der zugewiesenen Attribute, basierend auf dem Attributwert und unter Berücksichtigung von effektiven Datumsangaben.
1. Wenn keiner dieser Sätze gefunden wird, ist der Kostensatz 0.

## Istkosten - Benutzer und Funktion pro Stunde

Wenn für die Aufgabe der Kostentyp „Benutzer und Funktion pro Stunde“ festgelegt ist, verwendet Workfront zwei Hierarchien, um den Abrechnungssatz für die Ist-Kosten zu bestimmen. Der Abrechnungssatz basiert auf den Stunden, die Benutzende für eine Aufgabe protokollieren.

Der „Benutzer“ in den Hierarchien ist die Person, die der Aufgabe zugewiesen wurde. Der „Besitzer“ ist die Person, deren Zeit für die Aufgabe protokolliert wird, auch wenn sie der Aufgabe nicht zugewiesen ist. Zum Beispiel wird Michael eine Aufgabe zugewiesen, aber Joanna schließt die Arbeit ab, weil Michael krank war. Der Manager kann die Zeit für die Aufgabe protokollieren und den Besitzer der protokollierten Stunden auf Joanna festlegen. Die Werte für den geplanten Umsatz basieren auf der Zuweisung und dem Satz von Michael in der Hierarchie, aber die tatsächlichen Umsatzwerte basieren auf dem Satz von Joanna.

Dieses Bild zeigt den Fluss der Ist-Kosten-Hierarchie:

![Istkosten für Benutzer- und Funktionskostentyp pro Stunde](assets/actual-cost-chart.png)

### Wenn der Eigentümer der protokollierten Stunden und der der Aufgabe zugewiesene Benutzer identisch sind

Workfront sucht zunächst nach einem Kostensatz anhand der Benutzerzuweisung. Wenn ein(e) Benutzende(r) der Aufgabe nicht zugewiesen ist, sucht er/sie anhand der Aufgabenrollenzuweisung nach einem Kostensatz.

Die Hierarchie für dieses Szenario entspricht der geplanten Kostenhierarchie. Siehe [Geplante Kosten - Benutzer und Funktion pro Stunde](#planned-cost--user-and-role-hourly) für diesen Workflow.

### Wenn der Eigentümer der protokollierten Stunden nicht der zugewiesene Benutzer der Aufgabe ist

Workfront sucht in den Benutzereigenschaften des Eigentümers entsprechend dieser Hierarchie:

1. Das System sucht nach dem Kostensatz für das Projekt für den Eigentümer und berücksichtigt die tatsächlichen Termine. Dies wird im Bereich „Sätze“ > „Kosten“ des Projekts in einer Gruppierung &quot;**: Überschreibungen“ > „Ressourcentyp: Benutzer** angezeigt. Dies ist ein Überschreibungssatz für das Projekt.
1. Als Nächstes sucht das System nach dem Kostensatz auf Systemebene im Benutzerprofil des Eigentümers und berücksichtigt dabei das Datum des Wirksamwerdens.
1. Als Nächstes sucht das System nach dem Kostensatz für das primäre Aufgabengebiet des Eigentümers (im Beispiel Designer).

   * Das System sucht zunächst nach dem Kostensatz für das Projekt für das primäre Aufgabengebiet des Eigentümers und berücksichtigt dabei effektive Termine. Dies wird im Bereich „Sätze“ > „Kosten“ des Projekts in einer Gruppierung &quot;**: Überschreibungen“ > „Ressourcentyp: Aufgabengebiet** angezeigt. Dies ist ein Überschreibungssatz für das Projekt.
   * Als Nächstes sucht das System auf einer Tarifkarte nach dem Tarif für das Aufgabengebiet und berücksichtigt dabei das Datum des In-Kraft-Tretens. Sie sehen dies im Bereich „Sätze“ > „Kosten“ des Projekts in einer **Tarifkarte: Angehängte Tarifkarte > Ressourcentyp: Aufgabengebiet** Gruppierung.
   * Als Nächstes sucht das System nach der Aufgabengebiet-Quote auf Systemebene, wobei Datumsangaben für die Gültigkeit berücksichtigt werden.

1. Wenn keiner dieser Sätze gefunden wird, ist der Abrechnungssatz 0.

