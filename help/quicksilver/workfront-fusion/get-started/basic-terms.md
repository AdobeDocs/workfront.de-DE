---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Grundlegende Begriffe in Adobe Workfront Fusion
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 2169dc2e-2135-47e0-a615-3de12cd120a9
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 0%

---

# Grundlegende Begriffe in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Adobe Workfront Fusion-Glossar](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/fusion-glossary.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] erfordert eine [!DNL Adobe Workfront Fusion] zusätzlich zu einer [!UICONTROL Adobe Workfront]-Lizenz.


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Aktion</p> </td> 
   <td>Ein Modul, mit dem Sie Bundles aus oder in eine ausgewählte Anwendung oder einen ausgewählten Service lesen oder schreiben können.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Aggregator]</p> </td> 
   <td> <p>Ein Modultyp, der mehrere Bundles (mehrere Datenarrays) zu einem einzigen Bundle zusammenführt. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/aggregator-module.md" class="MCXref xref">[!UICONTROL Aggregator]-Modul in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Schlüssel</td> 
   <td>Ein eindeutiger Code, der den Benutzer, Entwickler oder das Programm identifiziert, das die API einer Software aufruft und für die Authentifizierung verwendet wird. Da [!DNL Adobe Workfront Fusion] Module durch Verbinden von APIs funktionieren, sind manchmal API-Schlüssel erforderlich. API-Schlüssel werden von der App verteilt, die sie benötigt. Wenn Sie beispielsweise einen API-Schlüssel für [!DNL ActiveCampaign] benötigen, fordern Sie ihn über Ihr [!DNL ActiveCampaign] an.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Programm oder Service</td> 
   <td> <p>Eine Software-Anwendung, am häufigsten.</p> <p>Eine App kann auch eine spezielle Funktion sein, die Daten bearbeitet, z. B. ein Iterator oder ein Aggregator. </p> <p>Ein Service ist eine Quelle von Bundles, die eine Web-API, eine Webseite, verschiedene Arten von Servern (FTP, SMTP, IMAP usw.) umfassen können. </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">App-Connector</td> 
   <td>Eine App, die eine Verbindung zu einem anderen System herstellt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Bündel</p> </td> 
   <td> <p>Ein Bundle ist eine Basiseinheit, die von Modulen zurückgegeben oder empfangen wird. Ein Bundle besteht aus Elementen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Wenn Sie eine App oder einen Service zu einem Szenario hinzufügen, müssen Sie höchstwahrscheinlich zunächst eine Verbindung zwischen [!DNL Workfront Fusion] und der App oder dem Service herstellen, um die ausgewählten Daten abzurufen oder zu senden. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">Verbindungen - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Zyklus</p> </td> 
   <td> <p>Ein Zyklus bezieht sich auf zwei Phasen des Szenario-Durchgangs: Operation und Commit. Das Szenario kann aus einem oder mehreren Zyklen bestehen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Szenarioausführung, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Datenspeicher</p> </td> 
   <td> <p>Ein Tool, das Daten aus Szenarien speichert oder es Ihnen ermöglicht, Daten zwischen einzelnen Szenarien oder Szenario-Ausführungen zu übertragen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/data-stores.md" class="MCXref xref">Datenspeicher in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Datenübertragung</p> </td> 
   <td> <p>Die Datenmenge, die über Ihr Szenario übertragen wird. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Szenariodetails in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Filter</p> </td> 
   <td> <p>Zusätzliche Funktionen, die zwischen zwei Modulen angewendet werden können. Mit einem Filter können Sie dann nur mit Bundles arbeiten, die bestimmten Kriterien entsprechen. Es gibt eine Reihe verschiedener Filter, die Sie anwenden können. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Hinzufügen eines Filters zu einem Szenario in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID</p> </td> 
   <td> <p>Ein Name, der zur eindeutigen Identifizierung eines Bundles verwendet wird. Eine ID wird normalerweise verwendet, um ein Bundle zu unterscheiden, das von einem bestimmten Service aktualisiert oder gelöscht werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Elemente</p> </td> 
   <td> <p>Ein Teil eines Bundles. Bundles können aus mehreren Elementen bestehen. Es gibt verschiedene Arten von Elementen: Text, Zahl, Boolescher Wert (ja/nein), Datum, Uhrzeit, Puffer (Binärdaten), Sammlungen, Menü auswählen, Array und Validierung.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Iterator]</p> </td> 
   <td> <p>Ein Modultyp, mit dem Sie ein Datenbündel (ein Datenarray) verwenden und in separate Pakete unterteilen können. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!UICONTROL Iterator]-Modul in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Modul</p> </td> 
   <td> <p>Ein einzelner Schritt innerhalb eines Szenarios, das eine Funktion ausführt, z. B. das Erstellen eines Datensatzes, innerhalb der zugehörigen App oder des zugehörigen Services.</p> <p>Jede Anwendung oder jeder Service verfügt über verschiedene Module, die definieren, wie sie bzw. er auf eine Anfrage reagiert.</p> <p>Es gibt 4 Modultypen: Aktionen, Trigger, Iteratoren und Aggregatoren.</p> <p> <img src="assets/module.jpg"> </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Modultypen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Vorgang</p> </td> 
   <td> <p>Eine von einem Modul ausgeführte Aufgabe.</p><p>Weitere Informationen finden Sie unter <a href="../../workfront-fusion/get-started/operations-in-workfront-fusion.md" class="MCXref xref">Vorgänge in [!DNL Adobe Workfront Fusion]</a>.</p>
  </tr> 
  <tr> 
   <td role="rowheader">Öffentliche/private Schlüssel</td> 
   <td>Öffentliche und private Schlüssel werden zum Ver- und Entschlüsseln von Daten verwendet. Der öffentliche Schlüssel kann verteilt werden, und jeder mit dem öffentlichen Schlüssel kann Daten verschlüsseln, aber nur der private Schlüssel kann sie entschlüsseln. Ebenso kann ein Benutzer mit einem privaten Schlüssel Daten verschlüsseln, die jeder mit dem öffentlichen Schlüssel entschlüsseln kann. Die Verschlüsselung des privaten Schlüssels stellt sicher, dass die Daten vom Eigentümer des privaten Schlüssels stammen und als Validierung der Datenquelle dienen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Router]</p> </td> 
   <td>Ermöglicht das Duplizieren von Daten oder das Hinzufügen neuer Routen zu einem Szenario, sodass Daten neu routen und verschiedene Datengruppen separat verarbeitet werden können. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/router-module.md" class="MCXref xref">[!UICONTROL Router]-Modul in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Szenario</p> </td> 
   <td> <p>Eine vom Benutzer erstellte Reihe automatisierter Schritte, die jeweils von einem Modul repräsentiert und ausgeführt werden. Der Zweck eines Szenarios besteht darin, Daten zu verschieben und zu bearbeiten.</p> <p> <img src="assets/scenario-350x178.jpg" style="width: 350;height: 178;"> </p> <p> Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in[!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Szenario-Segment</p> </td> 
   <td> <p> Ein Abschnitt eines Szenarios, das aus einer Reihe von Modulen besteht, die alle mit derselben Anwendung verbunden sind. Szenario-Segmente stellen oft einen kurzen Workflow im Programm dar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Transaktionen</p> </td> 
   <td> <p>[!DNL Workfront Fusion] Verwendet Transaktionsverarbeitung zur Erfassung des Szenario-Lebenszyklus. Eine Transaktion besteht aus mehreren Phasen, in denen Daten von einem konsistenten Zustand in einen anderen konsistenten Zustand transformiert werden. Es gibt 4 Phasen: Initialisierung, Vorgang (Lesen oder Schreiben), Commit/Rollback und Finalisierung.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Trigger</p> </td> 
   <td> <p>Ein Modul, mit dem Sie Pakete erfassen können, die seit der letzten Ausführung eines Szenarios hinzugefügt oder aktualisiert wurden. Es gibt zwei Typen von Triggern: Abfrage und Instant (Webhooks). Weitere Informationen finden Sie unter <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Instant Trigger (Webhooks) in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Webhook</p> </td> 
   <td> <p>Ein spezieller Trigger-Typ, mit dem Sie ein Szenario sofort ausführen können, nachdem ein neues Bundle verfügbar ist. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Instant Trigger (Webhooks) in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
