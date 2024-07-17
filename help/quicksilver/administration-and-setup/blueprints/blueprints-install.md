---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Blueprint installieren
description: Sie können einen Blueprint in Ihrer Produktionsumgebung oder in einer Sandbox-Umgebung installieren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Blueprint installieren

Sie können einen Blueprint in Ihrer Produktionsumgebung oder in einer Sandbox-Umgebung installieren.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan</strong></td> 
   <td> <p> Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] Lizenz</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene</strong></td> 
   <td> <p>[!UICONTROL Systemadministrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Wo sollte ich einen Blueprint installieren? {#where-should-i-install-a-blueprint}

Sie können Ihr Paket in einer der folgenden Umgebungen installieren:

<table style="table-layout:auto">
        <tr>
        <td><strong>Produktion</strong></td>
        <td>Die Produktion ist Ihre Live-Umgebung.</td>
    </tr>
    <tr>
        <td><strong>Sandbox-Vorschau</strong></td>
        <td>Die Sandbox-Vorschau ist eine Testumgebung, die als Replikation Ihrer Live-Umgebung dient und an jedem Wochenende von Workfront aktualisiert wird. Alle Support-Pakete haben Zugriff auf die Sandbox-Vorschau. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Die [!DNL Adobe Workfront] Vorschau-Sandbox-Umgebung</a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 &amp; 2</strong></td>
        <td>Die Sandbox für benutzerdefinierte Aktualisierungen ist eine separate Testumgebung, die von Ihnen manuell aktualisiert wird. Es fallen zusätzliche Kosten an, um die Sandbox "Benutzerdefinierte Aktualisierung"zu erhalten. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">Die [!DNL Adobe Workfront] benutzerdefinierte Aktualisierungs-Sandbox-Umgebung</a>.</td>
    </tr>
</table>

>[!TIP]
>
>Es wird empfohlen, den Blueprint zunächst in einer Sandbox-Umgebung zu installieren. Auf diese Weise können Sie den Inhalt des Blueprints testen und sicherstellen, dass er für Ihre Organisation geeignet ist, ohne Änderungen an den Live-Daten vorzunehmen.

>[!NOTE]
>
>Bestimmte Blueprints können nur zu Testzwecken in der Vorschau-Umgebung installiert werden. Wenn Sie auf reine Vorschau-Inhalte in Ihrer Produktionsumgebung, Sandbox 1 oder Sandbox 2 zugreifen, ist die Schaltfläche &quot;Installieren&quot;nicht aktiv und es wird möglicherweise eine Warnmeldung angezeigt.\
>Außerdem ist die Umstellungsfunktion beim Zugriff auf reine Inhalte der Vorschau eingeschränkt, auch wenn Sie sich in der Umgebung &quot;Vorschau&quot;befinden.

## Blueprint installieren

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe] Workfront und klicken Sie dann auf **[!UICONTROL Blueprints]**.![](assets/main-menu-icon.png)
1. Suchen Sie den zu installierenden Blueprint. Sie können nach Nutzungsszenario, Reifegrad, Installationsstatus und Typ auf der rechten Seite filtern.
1. (Optional) Klicken Sie auf **[!UICONTROL Details]** , um zu erfahren, wie der Blueprint funktioniert.
1. Klicken Sie auf **[!UICONTROL Installieren]**.
1. Wählen Sie die Installation in Ihrer Produktionsumgebung oder in einer Sandbox-Umgebung aus.\
   Weitere Informationen finden Sie unter [Wo soll ich einen Blueprint installieren?](#where-should-i-install-a-blueprint) in diesem Artikel.
1. Auf der Seite [!UICONTROL Konfigurieren] können Sie einen der folgenden Schritte ausführen:

   * Installieren Sie den Blueprint wie besehen. Bei Blueprint-Typen, die keine Konfiguration erfordern, ist dies die einzige Option. Bei Blueprint-Typen, die konfiguriert werden müssen, können Sie optional den Blueprint jetzt installieren und später konfigurieren. Klicken Sie auf **[!UICONTROL Installieren unter is]**.
   * Konfigurieren Sie den Blueprint vor der Installation für Blueprints, die konfiguriert werden müssen. Nehmen Sie die Konfigurationsauswahl vor und klicken Sie auf **[!UICONTROL Blueprint installieren]**\.

     Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../administration-and-setup/blueprints/configure-template-package.md).
Nach Abschluss der Installation zeigt eine Meldung eine Liste der spezifischen Objekte (z. B. Rollen, Teams oder Gruppen) an, die erfolgreich mit dem Blueprint installiert wurden, sowie der Objekte, die nicht installiert werden konnten.

Nach der Installation des Blueprints sind möglicherweise einige zusätzliche Aktionen erforderlich, um ihn vollständig bereitzustellen. Weitere Informationen finden Sie unter [Aktionen, die nach der Installation eines Blueprints ausgeführt werden sollen](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
