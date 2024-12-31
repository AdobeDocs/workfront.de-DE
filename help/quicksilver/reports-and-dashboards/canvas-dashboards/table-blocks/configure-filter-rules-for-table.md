---
title: Filtern einer Tabelle auf der Reporting-Arbeitsfläche
description: Filtern einer Tabelle auf der Reporting-Arbeitsfläche
hidefromtoc: true
hide: true
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 0%

---

# Filtern einer Tabelle auf der Reporting-Arbeitsfläche

Nachdem Sie einem Bericht einen Tabellenblock hinzugefügt haben, können Sie Filter einrichten, um die in der Tabelle angezeigten Informationen zu begrenzen.

Eine Filterregel besteht aus drei Komponenten:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Feld</td> 
   <td> <p>Das Feld, das die Informationen enthält, nach denen Sie Ihre Tabelle filtern möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Benutzerin oder Benutzer</td> 
   <td> <p>Die Art und Weise, wie der Filter bestimmt, welche Feldwerte in Ihrer Tabelle enthalten oder davon ausgeschlossen sind. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Wert</td> 
   <td> <p>Die Werte innerhalb Ihres ausgewählten Felds, die entsprechend dem Operator ausgewertet werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Beispiel:** Wenn Sie die Ergebnisse in Ihrem Bericht auf die Anzeige von Projekten beschränken möchten, die Jane Doe gehören, können Sie eine Filterregel mit dem Feld „Projekteigentümer“, dem Operator „Gleich“ und dem Wert „Jane Doe“ erstellen.

Sie können auch nur Projekte anzeigen, denen ein Projektbesitzer zugewiesen wurde. Dieses Feld würde das Feld „Projektbesitzer“ und den Operator „Ist nicht leer“ enthalten.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie sich für die Betaversion der Reporting-Arbeitsfläche registrieren. Weitere Informationen finden Sie unter [Reporting-Arbeitsfläche - Betaversion: Übersicht](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Konfigurieren von Filterregeln für Tabellen

1. Klicken Sie auf das **Hauptmenü**-Symbol ![](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront und dann auf **Reporting**.

1. Klicken Sie **Neuer Bericht**.

   Oder

   Um zu einem vorhandenen Bericht zu wechseln, klicken Sie auf das **Mehr Menü**-Symbol ![](assets/more-icon.png) in der Berichtskopfzeile und wählen Sie dann **Bearbeiten** aus.

1. Um Zeilen in einer neuen Tabelle zu gruppieren, ziehen oder doppelklicken Sie auf einen Tabellenblock auf der Arbeitsfläche.

   Oder

   Um Zeilen in einer vorhandenen Tabelle zu gruppieren, klicken Sie auf das **Bearbeiten**-Symbol ![](assets/edit-icon.png) in der Tabellenkopfzeile.

1. Suchen Sie im rechten Bedienfeld das Feld, nach dem Sie Ihre Tabelle filtern möchten, und ziehen Sie es dann in den Abschnitt Filter .

   Ein Filterregelsatz wird mit dem Namen des ausgewählten Felds angezeigt.

1. Wählen Sie den gewünschten Operator aus dem Dropdown-Menü aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Gleich</strong> </td> 
      <td> <p>Gibt nur eine exakte Übereinstimmung mit dem gesuchten Wert zurück.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ungleich</strong> </td> 
      <td> <p>Dadurch werden nur Ergebnisse zurückgegeben, die nicht exakt mit dem gesuchten Wert übereinstimmen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ist leer</strong> </td> 
      <td> <p>Das Feld ist für das Objekt vorhanden, dem Feld wurde jedoch noch kein Wert zugewiesen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ist nicht leer</strong> </td> 
      <td> <p>Das Feld, nach dem gefiltert werden soll, ist vorhanden und wurde mit einem Wert versehen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ist kleiner als</strong> </td> 
      <td> <p>Hierbei werden alle Ergebnisse mit einem Wert gesucht, der kleiner als der eingegebene ist, ohne den eingegebenen Wert zu berücksichtigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ist kleiner oder gleich</strong> </td> 
      <td> <p>Hierbei werden alle Ergebnisse mit einem Wert gesucht, der kleiner oder gleich dem eingegebenen Wert ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ist größer als</strong> </td> 
      <td> <p>Hierbei werden alle Ergebnisse mit einem Wert gesucht, der größer ist als der eingegebene Wert, ohne den eingegebenen Wert zu berücksichtigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ist größer oder gleich</strong> </td> 
      <td> <p>Hierbei werden alle Ergebnisse mit Werten gesucht, die größer oder gleich dem eingegebenen Wert sind.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Zwischen</strong> </td> 
      <td> <p>Stellt zwei erforderliche Feldwerte bereit und sucht nach allen Ergebnissen innerhalb des Bereichs beider Felder, einschließlich der eingegebenen Werte.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Enthält</strong> </td> 
      <td> <p>Dadurch wird über eine gesamte Textzeichenfolge nach dem angegebenen Text gesucht.</p> <p>Die Verwendung von „Enthält Inf“ erfasst beispielsweise alles, was „Inf“ oder „inf“ enthält, wie das Wort „Infinity“.</p> <p>Hinweis: Adobe Workfront sucht für jede Filterregel das gesamte Wort oder die Phrase, das bzw. die Sie eingeben. Wenn Sie beispielsweise nach Feldern mit der Phrase „Neues Projekt“ im Namen suchen, zeigt Workfront keine Projekte an, die nur „Neu“ oder „Projekt“ im Namen enthalten, oder Phrasen, die zusätzliche Wörter dazwischen enthalten, wie „Neues Hauptprojekt“. Der Filter findet nur Projekte mit der exakten Phrase „Neues Projekt“ im Namen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Enthält nicht</strong> </td> 
      <td> <p>Dadurch werden Elemente herausgefiltert, denen der angegebene Text fehlt.</p> <p>Beispielsweise gibt „enthält keine inf“ alle Felder zurück, deren Namen nicht „inf“ oder „inf“ enthalten.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Geben Sie den letzten Wert ein, um die Filterregel basierend auf dem ausgewählten Operator abzuschließen.

   >[!NOTE]
   >
   >Bei den hier eingegebenen Werten wird **Groß-** Kleinschreibung beachtet.

1. (Optional) Gehen Sie wie folgt vor, um Ihrem Regelsatz eine weitere Filterregel hinzuzufügen:

   1. Ziehen Sie ein weiteres Feld in den Bereich **Ablegen, um eine weitere Regel hinzuzufügen** im Abschnitt Filter unter Ihrer anderen Regel.
   1. Wiederholen Sie die Schritte 4 bis 6.
   1. Wählen Sie in der Dropdown-Liste Operator links neben der neuen Regel **AND** oder **OR**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>UND</p> </td> 
         <td> <p>Wenn Sie Filterregeln oder Regelsätze mit dem AND-Operator verbinden, geben Sie an, dass alle Regeln auf derselben Ebene erfüllt werden sollen.</p> <p>Standardmäßig werden die Anweisungen in einem Filter durch den AND-Operator verbunden.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>ODER</p> </td> 
         <td> <p>Wenn Sie Filterregeln oder Regelsätze mit dem OR-Operator verbinden, geben Sie an, dass <strong>mindestens</strong> eine Regel - oder Regelsatz - auf dieser Ebene erfüllt werden soll.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >AND- und OR-Operatoren auf derselben Ebene - die entweder mehrere Regeln innerhalb eines Regelsatzes oder ganze Regelsätze miteinander verbinden - stimmen immer überein. Wenn Sie beispielsweise den Operator zwischen zwei Regeln innerhalb eines Regelsatzes ändern, ändern sich alle anderen Operatoren in diesem Regelsatz automatisch, sodass sie mit ihm übereinstimmen.

1. (Bedingt) Gehen Sie wie folgt vor, um einen zusätzlichen Filterregelsatz hinzuzufügen:

   1. Ziehen Sie das Feld, das Sie hinzufügen möchten, in den Bereich **Regelsatz hinzufügen** unter Ihre anderen Filterregelsätze.
   1. Wiederholen Sie die Schritte 4 bis 7.
   1. Wählen Sie in der Dropdown-Liste Operator links neben dem neuen Regelsatz die Option **AND** oder **OR**. Diese Operatoren funktionieren wie die in Schritt 7 aufgeführten, gelten aber für alle Regelsätze im Gegensatz zu einzelnen Regeln innerhalb eines Satzes.****
