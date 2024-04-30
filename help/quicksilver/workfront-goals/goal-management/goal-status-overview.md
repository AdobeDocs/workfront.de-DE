---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Zielstatusübersicht in Adobe Workfront-Zielen
description: Der Zielstatus gibt an, ob ein Ziel aktiv ist und derzeit Fortschritte aufzeichnet oder ob es inaktiv, entworfen oder bereits erreicht ist.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 4%

---

# Zielstatusübersicht in Adobe Workfront-Zielen

Ihr Unternehmen muss über Folgendes verfügen, um die in diesem Artikel beschriebene Funktion verwenden zu können:

* Für den neuen Plan und die Lizenzstruktur:

   * Ein ultimativer Plan

     Oder

     Eine zusätzliche Lizenz für Adobe Workfront Goals für die Prime- oder Select Adobe Workfront-Pläne. Weitere Informationen finden Sie unter [Adobe Workfront-Abo](https://www.workfront.com/plans).

* Für den aktuellen Plan und die Lizenzstruktur:

   * A Pro oder höher
   * Eine Adobe Workfront Goals-Lizenz zusätzlich zu einer Workfront-Lizenz.

Wenden Sie sich an Ihren Workfront-Kundenbetreuer, um mehr über eine Workfront Goals-Lizenz zu erfahren.

Der Zielstatus gibt an, ob ein Ziel aktiv ist und derzeit Fortschritte aufzeichnet oder ob es inaktiv, entworfen oder bereits erreicht ist.

## Überlegungen beim Aktualisieren des Zielstatus in Workfront-Zielen

* Sie können den Status von Zielen, die Sie erstellt haben oder die für Sie freigegeben wurden, nicht manuell aktualisieren. Der Status der Ziele wird abhängig von den Aktionen, die Sie für das Ziel ausführen, aktualisiert. Wenn Sie beispielsweise ein Ziel aktivieren, ändert sich der Status Entwurf in Aktiv.
* Es gibt einige Einschränkungen, und manchmal können Sie den Status eines Ziels gemäß den folgenden Regeln nicht in einen anderen Status ändern:

  | Von/zu | Entwurf | Aktiv | Inaktiv | Geschlossen |
  |---|---|---|---|---|
  | Entwurf | - | Ja | Nein | Nein |
  | Aktiv | Nein | - | Ja | Ja |
  | Inaktiv | Nein | Ja | - | Nein |
  | Geschlossen | Nein | Ja | Nein | - |

* Das Öffnen eines geschlossenen Ziels aktualisiert auch den Fortschritt des Ziels.
* Bestimmte Aktionen, die Sie für ein Ziel ausführen, aktualisieren auch dessen Status. Informationen dazu, wie Sie Zielstatus aktualisieren können, finden Sie in den folgenden Artikeln:

   * [Ziele in Adobe Workfront erstellen](../../workfront-goals/goal-management/create-goals.md)
   * [Ziele in Adobe Workfront aktivieren](../../workfront-goals/goal-management/activate-goals.md)
   * [Löschen und Deaktivieren von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Ziele in Adobe Workfront schließen und erneut öffnen](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Übersicht über den Zielstatus in Workfront-Zielen

Informationen zum Erstellen von Workfront-Zielen finden Sie unter [Ziele in Adobe Workfront erstellen](../../workfront-goals/goal-management/create-goals.md).

Informationen zum Aktivieren von Zielen finden Sie unter [Ziele in Adobe Workfront aktivieren](../../workfront-goals/goal-management/activate-goals.md).

Ziele können in Workfront-Zielen einen der folgenden Status aufweisen:

* [Entwurf](#draft)
* [Aktiv](#active)
* [Inaaktiv](#inactive)
* [Geschlossen](#closed)

### Entwurf {#draft}

* Dies ist der Standardstatus für ein neu erstelltes Ziel. Informationen zum Erstellen von Zielen finden Sie unter [Ziele in Adobe Workfront erstellen](../../workfront-goals/goal-management/create-goals.md).
* Workfront-Ziele zeichnen keine Fortschritte bei der Erreichung eines entworfenen Ziels auf.
* Sie können den Fortschritt eines entworfenen Ziels nicht aktualisieren.
* Entwürfe von Zielen können nicht geschlossen oder deaktiviert werden, da sie keine Fortschrittsinformationen enthalten.
* Entworfene Ziele tragen nicht zur Berechnung anderer Ziele bei und werden in Grafiken nicht berücksichtigt.
* Die entworfenen Ziele werden in den folgenden Bereichen der Workfront-Ziele angezeigt:

   * Liste der Ziele
   * Zielausrichtung (nur als ausgerichtetes Ziel)


>[!IMPORTANT]
>
>Nachdem Sie den Status eines Ziels in einen anderen Status geändert haben, kann das Ziel nie wieder in den Status Entwurf versetzt werden.

### Aktiv {#active}

* Sie können ein entworfenes Ziel nur aktivieren, wenn Sie es mit einem Ergebnis, einer Aktivität oder einem anderen Ziel verknüpfen. Durch Aktivierung des Ziels ändert sich sein Status in &quot;Aktiv&quot;. Informationen zum Aktivieren von Zielen finden Sie unter [Ziele in Adobe Workfront aktivieren](../../workfront-goals/goal-management/activate-goals.md).
* Workfront Goals zeichnet Fortschritte bei aktiven Zielen auf.
* Aktive Ziele tragen zur Fortschrittsberechnung anderer Ziele bei und werden in Grafiken berücksichtigt.
* Aktive Ziele werden in den folgenden Bereichen der Workfront-Ziele angezeigt:

   * Liste der Ziele
   * Abschnitt &quot;Zielausrichtung&quot;
   * Der Fortschritt aktiver Ziele wird in Diagrammen angezeigt

* Sie können ein geschlossenes oder inaktives Ziel erneut aktivieren.

### Inaktiv {#inactive}

* Sie können ein aktives Ziel deaktivieren, wenn der Eigentümer die Bearbeitung vorübergehend oder dauerhaft beendet hat. Sie können sie für historische Informationen aufbewahren. Dadurch wird der Status des Ziels auf Inaktiv aktualisiert.

  Informationen zum Deaktivieren von Zielen finden Sie im Abschnitt &quot;Ziele deaktivieren&quot;im Artikel [Löschen und Deaktivieren von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* Sie können ein entworfenes oder geschlossenes Ziel nicht deaktivieren.
* Sie können ein inaktives Ziel reaktivieren und weiter daran arbeiten.
* Workfront-Ziele berechnen keinen Fortschritt bei inaktiven Zielen.
* Sie können den Fortschritt eines inaktiven Ziels nicht aktualisieren.
* Inaktive Ziele tragen nicht zur Fortschrittsberechnung anderer Ziele bei und werden in Grafiken nicht berücksichtigt.
* Inaktive Ziele haben einen Fortschrittsverlauf, weil sie einst aktiv waren, im Gegensatz zu entworfenen Zielen.
* Inaktive Ziele werden in den folgenden Bereichen der Workfront-Ziele angezeigt:

   * Liste der Ziele
   * Zielausrichtung (nur als ausgerichtete Ziele)

### Geschlossen {#closed}

* Sie können ein Ziel schließen, wenn Sie angeben möchten, dass Sie es erreicht haben oder dass Sie daran nicht mehr arbeiten, und dies auch in Zukunft nicht tun werden. Informationen zum Schließen von Zielen finden Sie unter [Ziele in Adobe Workfront schließen und erneut öffnen](../../workfront-goals/goal-management/close-and-reopen-goals.md).

  >[!TIP]
  >
  >Wenn Sie planen, später an einem Ziel zu arbeiten, das noch nicht erreicht wurde, empfehlen wir, den Status auf Inaktiv anstatt auf Geschlossen zu ändern.

* Ziele, die noch nie aktiviert wurden, können nicht geschlossen werden, wie beispielsweise entworfene Ziele.
* Sie können ein geschlossenes Ziel erneut öffnen und daran weiter arbeiten.
* Workfront-Ziele stoppen die Aufzeichnung des Fortschritts bei geschlossenen Zielen.
* Sie können den Fortschritt eines geschlossenen Ziels nicht aktualisieren.
* Geschlossene Ziele werden im folgenden Bereich von Workfront-Zielen angezeigt:

   * Liste der Ziele
   * Zielausrichtung (nur als ausgerichtete Ziele)
   * Informationen zu geschlossenen Zielen werden auch im Abschnitt Diagramme berücksichtigt.
