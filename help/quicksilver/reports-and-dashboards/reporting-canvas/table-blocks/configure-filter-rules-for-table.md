---
title: Tabelle in Berichtsarbeitsfläche filtern
description: Tabelle in Berichtsarbeitsfläche filtern
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 1%

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
   <td role="rowheader">Operator</td> 
   <td> <p>Die Art und Weise, wie der Filter bestimmt, welche Feldwerte in Ihre Tabelle aufgenommen oder daraus ausgeschlossen werden. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Wert</td> 
   <td> <p>Die Werte in Ihrem ausgewählten Feld, die entsprechend dem Operator ausgewertet werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Beispiel:** Wenn Sie die Ergebnisse in Ihrem Bericht so einschränken möchten, dass nur Projekte angezeigt werden, die Jane Doe gehören, können Sie eine Filterregel mit dem Feld &quot;Projekteigentümer&quot;, dem Operator &quot;Gleich&quot;und dem Wert &quot;Jane Doe&quot;erstellen.

Oder Sie können nur Projekte anzeigen, denen ein Projekteigentümer zugewiesen ist, für die das Feld &quot;Projekteigentümer&quot;und der Operator &quot;Ist nicht leer&quot;vorhanden sind.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie sich in der Beta-Version der Reporting-Arbeitsfläche anmelden. Weitere Informationen finden Sie unter [Reporting-Arbeitsfläche - Beta: Übersicht](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## Konfigurieren von Filterregeln für eine Tabelle

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Berichterstellung**.

1. Klicken **Neuer Bericht**.

   Oder

   Gehen Sie zu einem vorhandenen Bericht und klicken Sie auf die Schaltfläche **Mehr Menü** icon ![](assets/more-icon.png) im Berichtkopf und wählen Sie dann **Bearbeiten**.

1. Um Zeilen auf einer neuen Tabelle zu gruppieren, ziehen Sie einen Tabellenblock auf die Arbeitsfläche oder doppelklicken Sie darauf.

   Oder

   Um Zeilen in einer vorhandenen Tabelle zu gruppieren, klicken Sie auf die **Bearbeiten** icon ![](assets/edit-icon.png) in der Tabellenüberschrift.

1. Suchen Sie im rechten Bereich das Feld, nach dem Sie Ihre Tabelle filtern möchten, und ziehen Sie es in den Bereich Filter .

   Ein Filterregelsatz wird mit dem Namen des ausgewählten Felds angezeigt.

1. Wählen Sie im Dropdown-Menü den gewünschten Operator aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Gleich</strong> </td> 
      <td> <p>Dadurch wird nur eine exakte Übereinstimmung mit dem gesuchten Wert zurückgegeben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ungleich</strong> </td> 
      <td> <p>Dadurch werden nur Ergebnisse zurückgegeben, die nicht exakt mit dem gesuchten Wert übereinstimmen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Leer</strong> </td> 
      <td> <p>Das Feld existiert für das Objekt, dem Feld wurde jedoch noch kein Wert zugewiesen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Nicht leer</strong> </td> 
      <td> <p>Das Feld, nach dem Sie filtern, ist vorhanden und hat einen Wert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Less Than</strong> </td> 
      <td> <p>Hierbei wird nach allen Ergebnissen gesucht, deren Wert kleiner ist als der eingegebene Wert, ohne den eingegebenen Wert einzuschließen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Less Than Or Equal To</strong> </td> 
      <td> <p>Hierbei werden alle Ergebnisse gesucht, deren Wert kleiner oder gleich dem eingegebenen Wert ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Greater Than</strong> </td> 
      <td> <p>Hierbei wird nach allen Ergebnissen gesucht, deren Wert größer als der eingegebene Wert ist, ohne den eingegebenen Wert einzuschließen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Greater Than Or Equal To</strong> </td> 
      <td> <p>Hierdurch werden alle Ergebnisse gesucht, deren Werte größer oder gleich dem eingegebenen Wert sind.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Zwischen</strong> </td> 
      <td> <p>Stellt zwei erforderliche Feldwerte bereit und sucht nach allen Ergebnissen innerhalb des Bereichs beider Felder, einschließlich der eingegebenen Werte.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Enthält</strong> </td> 
      <td> <p>Dadurch wird in einer gesamten Textzeichenfolge nach dem angegebenen Text gesucht.</p> <p>Beispielsweise erfasst die Verwendung von "Enthält Inf"alles mit "Inf"oder "inf", z. B. das Wort "Unendlichkeit".</p> <p>Hinweis: Adobe Workfront sucht nach dem gesamten Wort bzw. der gesamten Wortgruppe, die Sie für jede Filterregel eingeben. Wenn Sie beispielsweise nach Feldern suchen, deren Name die Wortgruppe "neues Projekt"enthält, zeigt Workfront keine Projekte an, deren Namen nur "neues Projekt"oder "Projekt"enthalten, oder Ausdrücke, die dazwischen zusätzliche Wörter enthalten, z. B. "neues Hauptprojekt". Der Filter findet nur Projekte mit dem genauen Wortlaut "neues Projekt"im Namen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beinhaltet nicht</strong> </td> 
      <td> <p>Dadurch werden Elemente herausgefiltert, die angegebenen Text fehlen.</p> <p>Beispielsweise gibt "enthält nicht inf"alle Felder zurück, deren Namen "Inf"oder "inf"enthalten.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Geben Sie je nach gewähltem Operator den letzten Wert ein, um die Filterregel abzuschließen.

   >[!NOTE]
   >
   >Die hier eingegebenen Werte sind **not** Groß-/Kleinschreibung beachten.

1. (Optional) Gehen Sie wie folgt vor, um Ihrem Regelsatz eine weitere Filterregel hinzuzufügen:

   1. Ziehen Sie ein weiteres Feld in den **Ablegen , um eine weitere Regel hinzuzufügen** im Abschnitt Filter unter Ihrer anderen Regel.
   1. Wiederholen Sie die Schritte 4 bis 6.
   1. Wählen Sie links im Dropdown-Menü Operator die Option **UND** oder **ODER**.

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
         <td> <p>Wenn Sie Filterregeln oder Regelsätze mit dem ODER-Operator verknüpfen, geben Sie an, dass Sie <strong>mindestens</strong> eine Regel - oder einen Regelsatz - auf dieser Ebene zu erfüllen.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >UND- und ODER-Operatoren auf derselben Ebene - die entweder mehrere Regeln innerhalb eines Regelsatzes oder ganze Regelsätze miteinander verbinden - stimmen immer überein. Wenn Sie beispielsweise den Operator zwischen zwei Regeln in einem Regelsatz ändern, ändern sich alle anderen Operatoren in diesem Regelsatz automatisch entsprechend.

1. (Bedingt) Gehen Sie wie folgt vor, um einen zusätzlichen Filterregelsatz hinzuzufügen:

   1. Ziehen Sie das Feld, das Sie hinzufügen möchten, zum **Regelsatz hinzufügen** Bereich unterhalb Ihrer anderen Filterregelsätze.
   1. Wiederholen Sie die Schritte 4 bis 7.
   1. Wählen Sie im Dropdown-Menü Operator links im neuen Regelsatz die Option **UND** oder **ODER**. Diese Operatoren funktionieren genauso wie die in Schritt 7 aufgeführten, gelten jedoch für ganze Regelsätze im Gegensatz zu einzelnen Regeln innerhalb eines Satzes.****
