---
title: Tabelle in Berichtsarbeitsfläche filtern
description: Tabelle in Berichtsarbeitsfläche filtern
hidefromtoc: true
hide: true
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 0%

---

# Tabelle in Berichtsarbeitsfläche filtern

Nachdem Sie einen Tabellenblock zu einem Bericht hinzugefügt haben, können Sie Filter einrichten, um die in der Tabelle angezeigten Informationen zu beschränken.

Eine Filterregel enthält drei Komponenten:

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
   <td> <p>Die Art und Weise, wie der Filter bestimmt, welche Feldwerte in Ihre Tabelle aufgenommen oder daraus ausgeschlossen werden. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Wert</td> 
   <td> <p>Die Werte in Ihrem ausgewählten Feld, die entsprechend dem Operator ausgewertet werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Beispiel:** Wenn Sie die Ergebnisse in Ihrem Bericht darauf beschränken möchten, nur Projekte anzuzeigen, die im Besitz von Jane Doe sind, können Sie eine Filterregel mit dem Feld &quot;Projekteigentümer&quot;, dem Operator &quot;Gleich&quot;und dem Wert &quot;Jane Doe&quot;erstellen.

Oder Sie können nur Projekte anzeigen, denen ein Projekteigentümer zugewiesen ist, für die das Feld &quot;Projekteigentümer&quot;und der Operator &quot;Ist nicht leer&quot;vorhanden sind.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie sich in der Beta-Version der Reporting-Arbeitsfläche anmelden. Weitere Informationen finden Sie unter [Arbeitsfläche für die Berichterstellung Beta: Übersicht](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Konfigurieren von Filterregeln für eine Tabelle

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Berichterstellung**.![](assets/main-menu-icon.png)

1. Klicken Sie auf **Neuer Bericht**.

   Oder

   Wechseln Sie zu einem vorhandenen Bericht, klicken Sie auf das Symbol **Mehr Menü** ![](assets/more-icon.png) im Berichtkopf und wählen Sie dann **Bearbeiten** aus.

1. Um Zeilen auf einer neuen Tabelle zu gruppieren, ziehen Sie einen Tabellenblock auf die Arbeitsfläche oder doppelklicken Sie darauf.

   Oder

   Um Zeilen auf einer vorhandenen Tabelle zu gruppieren, klicken Sie auf das Symbol **Bearbeiten** ![](assets/edit-icon.png) in der Tabellenüberschrift.

1. Suchen Sie im rechten Bereich das Feld, nach dem Sie Ihre Tabelle filtern möchten, und ziehen Sie es in den Bereich Filter .

   Ein Filterregelsatz wird mit dem Namen des ausgewählten Felds angezeigt.

1. Wählen Sie im Dropdown-Menü den gewünschten Operator aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Entspricht</strong> </td> 
      <td> <p>Dadurch wird nur eine exakte Übereinstimmung mit dem gesuchten Wert zurückgegeben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Nicht gleich</strong> </td> 
      <td> <p>Dadurch werden nur Ergebnisse zurückgegeben, die nicht exakt mit dem gesuchten Wert übereinstimmen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ist leer</strong> </td> 
      <td> <p>Das Feld existiert für das Objekt, dem Feld wurde jedoch noch kein Wert zugewiesen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ist nicht leer</strong> </td> 
      <td> <p>Das Feld, nach dem Sie filtern, ist vorhanden und hat einen Wert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ist kleiner als</strong> </td> 
      <td> <p>Hierbei wird nach allen Ergebnissen gesucht, deren Wert kleiner ist als der eingegebene Wert, ohne den eingegebenen Wert einzuschließen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ist kleiner als oder gleich</strong> </td> 
      <td> <p>Hierbei werden alle Ergebnisse gesucht, deren Wert kleiner oder gleich dem eingegebenen Wert ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ist größer als</strong> </td> 
      <td> <p>Hierbei wird nach allen Ergebnissen gesucht, deren Wert größer als der eingegebene Wert ist, ohne den eingegebenen Wert einzuschließen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ist größer als oder gleich</strong> </td> 
      <td> <p>Hierdurch werden alle Ergebnisse gesucht, deren Werte größer oder gleich dem eingegebenen Wert sind.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Between</strong> </td> 
      <td> <p>Stellt zwei erforderliche Feldwerte bereit und sucht nach allen Ergebnissen innerhalb des Bereichs beider Felder, einschließlich der eingegebenen Werte.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Enthält</strong> </td> 
      <td> <p>Dadurch wird in einer gesamten Textzeichenfolge nach dem angegebenen Text gesucht.</p> <p>Beispielsweise erfasst die Verwendung von "Enthält Inf"alles mit "Inf"oder "inf", z. B. das Wort "Unendlichkeit".</p> <p>Hinweis: Adobe Workfront sucht nach dem gesamten Wort bzw. der gesamten Wortgruppe, die bzw. die Wortgruppe, die Sie für jede Filterregel eingeben. Wenn Sie beispielsweise nach Feldern suchen, deren Name die Wortgruppe "neues Projekt"enthält, zeigt Workfront keine Projekte an, deren Namen nur "neues Projekt"oder "Projekt"enthalten, oder Ausdrücke, die dazwischen zusätzliche Wörter enthalten, z. B. "neues Hauptprojekt". Der Filter findet nur Projekte mit dem genauen Wortlaut "neues Projekt"im Namen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>enthält nicht</strong> </td> 
      <td> <p>Dadurch werden Elemente herausgefiltert, die angegebenen Text fehlen.</p> <p>Beispielsweise gibt "enthält nicht inf"alle Felder zurück, deren Namen "Inf"oder "inf"enthalten.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Geben Sie je nach gewähltem Operator den letzten Wert ein, um die Filterregel abzuschließen.

   >[!NOTE]
   >
   >Bei den hier eingegebenen Werten wird zwischen **und nicht** zwischen Groß- und Kleinschreibung unterschieden.

1. (Optional) Gehen Sie wie folgt vor, um Ihrem Regelsatz eine weitere Filterregel hinzuzufügen:

   1. Ziehen Sie ein weiteres Feld in den Bereich **Ablegen , um im Abschnitt Filter unter Ihrer anderen Regel einen weiteren Regelbereich** hinzuzufügen.
   1. Wiederholen Sie die Schritte 4 bis 6.
   1. Wählen Sie links im Operator-Dropdown-Menü die Option **AND** oder **OR** aus.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>UND</p> </td> 
         <td> <p>Wenn Sie Filterregeln oder Regelsätze mit dem UND-Operator verbinden, geben Sie an, dass alle Regeln auf derselben Ebene erfüllt werden sollen.</p> <p>Standardmäßig werden die Anweisungen in einem Filter durch den UND -Operator verbunden.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>ODER</p> </td> 
         <td> <p>Wenn Sie Filterregeln oder Regelsätze mit dem ODER-Operator verbinden, geben Sie an, dass <strong>mindestens</strong> eine Regel - oder ein Regelsatz - auf dieser Ebene erfüllt werden soll.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >UND- und ODER-Operatoren auf derselben Ebene - die entweder mehrere Regeln innerhalb eines Regelsatzes oder ganze Regelsätze miteinander verbinden - stimmen immer überein. Wenn Sie beispielsweise den Operator zwischen zwei Regeln in einem Regelsatz ändern, ändern sich alle anderen Operatoren in diesem Regelsatz automatisch entsprechend.

1. (Bedingt) Gehen Sie wie folgt vor, um einen zusätzlichen Filterregelsatz hinzuzufügen:

   1. Ziehen Sie das Feld, das Sie hinzufügen möchten, in den Bereich **Regelsatz hinzufügen** unter Ihre anderen Filterregelsätze.
   1. Wiederholen Sie die Schritte 4 bis 7.
   1. Wählen Sie links im Operator-Dropdown-Menü des neuen Regelsatzes **AND** oder **OR** aus. Diese Operatoren funktionieren genauso wie die in Schritt 7 aufgeführten, gelten jedoch für ganze Regelsätze im Gegensatz zu einzelnen Regeln innerhalb eines Satzes.****
