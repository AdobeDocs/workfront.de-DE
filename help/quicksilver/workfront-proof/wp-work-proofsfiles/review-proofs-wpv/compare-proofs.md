---
product-previous: workfront-proof
product-area: documents
navigation-topic: review-proofs-workfront-proofing-viewer
title: Vergleichen von Testsendungen im Testversand-Viewer
description: Sie können einen Vergleich zweier Testsendungen nebeneinander anzeigen. Dabei kann es sich um zwei Versionen desselben Testversands oder zwei vollständig separate Testsendungen handeln.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d4ec0c53-1451-4475-aa38-2319c6432936
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# Vergleichen von Testsendungen im Testversand-Viewer

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Sie können einen Vergleich zweier Testsendungen nebeneinander anzeigen. Dabei kann es sich um zwei Versionen desselben Testversands oder zwei vollständig separate Testsendungen handeln.

## Vergleichen von Testversionen {#compare-proof-versions}

1. Öffnen Sie den Testversand, der mehrere Versionen enthält, die Sie vergleichen möchten.
1. Klicken Sie in der linken oberen Ecke des angezeigten Testversand-Viewers auf den Namen des Testversands. Klicken Sie dann in der angezeigten Liste der Versionen auf das Symbol **Vergleichen** neben der Version, die Sie öffnen und vergleichen möchten.

   ![](assets/compare-proofs-choose-version-350x115.jpg)

   Die Testsendungen werden nebeneinander angezeigt, die neuere Version auf der linken Seite.

   <!--
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">Separate breadcrumbs above each proof allow you to view and go to the work item associated with the proof:</p>
   -->

   <!--
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/compare-proofs-breadcrumbs-350x148.jpg" style="width: 350;height: 148;"> </p>
   -->

1. Fahren Sie mit [Verwenden Sie die Vergleichswerkzeuge](#use-the-compare-tools) fort.

## Separate Testsendungen vergleichen {#compare-separate-proofs}

Sie können zwei verschiedene Testsendungen vergleichen.

* [Separate Testsendungen in  [!DNL Workfront] vergleichen](#compare-separate-proofs-in-workfront)
* [Separate Testsendungen in  [!DNL Workfront Proof] vergleichen](#compare-separate-proofs-in-workfront-proof)

### Separate Testsendungen in [!DNL Workfront] vergleichen {#compare-separate-proofs-in-workfront}

Informationen zum Vergleich separater Testsendungen mit der Dokumentliste innerhalb von [!DNL Workfront] finden Sie im Abschnitt [Vergleichen von zwei verschiedenen Testsendungen](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md#comparing-two-proofs-from-a-document-list) im Artikel [Testsendungen vergleichen](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md) .

### Separate Testsendungen in [!DNL Workfront Proof] vergleichen {#compare-separate-proofs-in-workfront-proof}

>[!NOTE]
>
>Die von Ihnen verglichenen Testsendungen müssen sich im selben Ordner und auf derselben Hierarchieebene innerhalb der Ordnerstruktur befinden. Weitere Informationen zum Verwenden von Ordnern zum Gruppieren von Testsendungen, die Sie vergleichen möchten, finden Sie unter [Arbeiten mit mehreren Testsendungen im Testversand-Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/work-with-multiple-proofs.md)

1. Öffnen Sie eine der Testsendungen, die Sie vergleichen möchten, im Testversand-Viewer.
1. Klicken Sie auf das Symbol **[!UICONTROL Modus vergleichen]** .

   ![proof_compare_icon.png](assets/proof-compare-icon.png)\
   Der Anzeigebereich wird halbiert und der Testversand wird links und rechts im Testversand-Viewer angezeigt.

   ![Vergleich_proofs-versions.png](assets/compare-proofs-versions-350x180.png)

1. Klicken Sie auf das Symbol [!UICONTROL Ordner] oberhalb des Testversands auf der linken oder rechten Seite, um die anderen Testsendungen im selben Ordner aufzulisten.

   ![Folder_icons_when_compare_in_proofing_viewer.png](assets/folder-icons-when-comparing-in-proofing-viewer-350x121.png)

1. Klicken Sie in der Liste auf den Namen des Testversands, den Sie mit dem Testversand vergleichen möchten, der derzeit im Testversand-Viewer geöffnet ist.

   ![Comparing_proofs-list_of_proofs_in_folder.png](assets/comparing-proofs-list-of-proofs-in-folder-350x89.png)

   Beide Testsendungen werden angezeigt.

1. Fahren Sie mit [Verwenden Sie die Vergleichswerkzeuge](#use-the-compare-tools) fort.

## Verwenden der Vergleichstools {#use-the-compare-tools}

Der Testversand-Viewer bietet verschiedene Tools zum effektiven und effizienten Vergleich von Testsendungen.

* [Testsendungen automatisch vergleichen](#auto-compare-proofs)
* [Testsendungen in einer Überlagerung vergleichen](#compare-proofs-in-an-overlay)
* [Vergleich der gleichzeitigen Navigation](#simultaneous-navigation-comparison)

### Testsendungen automatisch vergleichen {#auto-compare-proofs}

Der automatische Vergleich führt einen Pixelvergleich zwischen zwei statischen oder Videotests durch. Alle erkannten Unterschiede werden im Testversand links rot hervorgehoben.

Der automatische Vergleich ist beim Vergleich interaktiver Testsendungen nicht verfügbar.

So vergleichen Sie zwei Testsendungen automatisch:

1. Vergleichen Sie Testsendungen auf eine der folgenden Arten:

   * Vergleichen Sie zwei Versionen desselben Testversands (siehe [Testversand-Versionen vergleichen](#compare-proof-versions) in diesem Artikel).
   * Vergleichen Sie zwei separate Testsendungen (siehe [Separate Testsendungen vergleichen](#compare-separate-proofs) in diesem Artikel).

1. Klicken Sie auf das Symbol **[!UICONTROL Autovergleich]** .

   ![proof_autocompare_icon.png](assets/proof-autocompare-icon-31x32.png)

   Die Unterschiede zwischen den beiden Testsendungen werden im Testversand links rot hervorgehoben.

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Switch]** , um die aktive Seite so zu ändern, dass auf dem Testversand auf der rechten Seite Unterschiede angezeigt werden. Standardmäßig werden beim Testversand auf der linken Seite Unterschiede angezeigt.

   ![proof_autocompare_changactive.png](assets/proof-autocompare-changeactive.png)

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Farbe]** , um die Farbe und Deckkraft zu ändern, die zum Hervorheben von Unterschieden verwendet wird.

   ![proof_compare_color.png](assets/proof-compare-color.png)

### Testsendungen in einer Überlagerung vergleichen {#compare-proofs-in-an-overlay}

Der Überlagerungsvergleich ermöglicht es Ihnen, Unterschiede zwischen zwei statischen Testsendungen anzuzeigen, indem Sie die beiden Testsendungen als einen einzigen Testversand betrachten und gleichzeitig eine vertikale Trennlinie zwischen der Testmitte schaffen. Wenn Sie den Testversand über den vertikalen Divider schwenken, werden die Unterschiede angezeigt.

>[!NOTE]
>
>Der Vergleich von Überlagerungen ist beim Vergleich von Videos oder interaktiven Testsendungen nicht verfügbar.

So aktivieren Sie den Überlagerungsvergleich:

1. Vergleichen Sie Testsendungen auf eine der folgenden Arten:

   * Vergleichen Sie zwei Versionen desselben Testversands (siehe [Testversand-Versionen vergleichen](#compare-proof-versions) in diesem Artikel).
   * Vergleichen Sie zwei separate Testsendungen (siehe [Separate Testsendungen vergleichen](#compare-separate-proofs) in diesem Artikel).

1. Klicken Sie auf das Symbol **[!UICONTROL Überlagerung]** .

   ![proof_compare_overlay_icon.png](assets/proof-compare-overlay-icon.png)

   Die beiden Testsendungen werden als ein Testversand angezeigt, wobei der Abstand zwischen der Mitte des Testversands durch einen senkrechten Strich verläuft.

1. Führen Sie einen der folgenden Schritte aus:

   * Schwenken Sie den Testversand über die vertikale Trennlinie. Während Sie schwenken, sehen Sie den Testversand auf der linken Seite des vertikalen Teilers, während der Testversand auf der rechten Seite angezeigt wird.
   * Verschieben Sie den vertikalen Trennbereich nach links und rechts. Während Sie die Trennlinie verschieben, sehen Sie den Testversand auf der linken Seite des vertikalen Teilers, während der Testversand auf der rechten Seite angezeigt wird.

### Vergleich der gleichzeitigen Navigation {#simultaneous-navigation-comparison}

Die gleichzeitige Navigation ist beim Vergleich von Testsendungen standardmäßig aktiviert. Es ist verfügbar beim Vergleich eines statischen Testversands mit einem statischen Testversand oder beim Vergleich eines Videodrucks und eines Videodrucks. Es ist nicht verfügbar, wenn ein statischer Testversand und ein Videotest verglichen werden.

**Statische Testsendungen:** Bei Aktivierung für statische Testsendungen sperrt die gleichzeitige Navigation beim Schwenken oder Scrollen den Zoomgrad und die Position der beiden Testsendungen. Wenn ein Testversand mehrere Seiten enthält und die gleichzeitige Navigation aktiviert ist, führt das Ändern von Seiten in einem Testversand dazu, dass die Seite im anderen Testversand geändert wird.

**Video-Testsendungen:** Bei Aktivierung in Video-Testsendungen speichert die gleichzeitige Navigation die Zeitdifferenz bei den Zeitleisten der beiden Testsendungen.

So aktivieren Sie die gleichzeitige Navigation, falls sie noch nicht aktiviert ist:

1. Vergleichen Sie Testsendungen auf eine der folgenden Arten:

   * Vergleichen Sie zwei Versionen desselben Testversands (siehe [Testversand-Versionen vergleichen](#compare-proof-versions) in diesem Artikel).
   * Vergleichen Sie zwei separate Testsendungen (siehe [Separate Testsendungen vergleichen](#compare-separate-proofs) in diesem Artikel).

1. Klicken Sie auf das Symbol **[!UICONTROL Simultane Navigation]** .

   ![proof_compare_simultan_icon.png](assets/proof-compare-simultaneous-icon.png)

1. (Optional) Klicken Sie jederzeit auf das Symbol **[!UICONTROL Zurücksetzen]** , um den Zoomfaktor und die Zoomposition (für statischen Test) oder die Timeline (für Videotests) zurückzusetzen.

   ![proof_compare_simultan_reset.png](assets/proof-compare-simultaneous-reset.png)

## Ausstiegsvergleich

1. Schließen Sie den Testversand, den Sie nicht mehr anzeigen möchten, indem Sie auf das Symbol (x) in der oberen linken Ecke des Testversands klicken.

   ![proof_compare_exit.png](assets/proof-compare-exit-350x163.png)

   Der Beweis, dass Sie nicht schließen, bleibt im Testversand-Viewer offen.
