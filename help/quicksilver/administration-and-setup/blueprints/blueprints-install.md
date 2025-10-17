---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Blueprint installieren
description: Sie können eine Blueprint in Ihrer Produktionsumgebung oder einer Sandbox-Umgebung installieren.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# Blueprint installieren

<!-- Audited: 5/2025 -->

Sie können eine Blueprint in Ihrer Produktionsumgebung oder einer Sandbox-Umgebung installieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Workfront-Administrator</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Wo sollte ich eine Blueprint installieren? {#where-should-i-install-a-blueprint}

Sie können Ihr Paket in einer der folgenden Umgebungen installieren:

<table style="table-layout:auto">
        <tr>
        <td><strong>Produktion</strong></td>
        <td>Die Produktion ist Ihre Live-Umgebung.</td>
    </tr>
    <tr>
        <td><strong>Sandbox-Vorschau</strong></td>
        <td>Die Sandbox-Vorschau ist eine Testumgebung, die als Replikation Ihrer Live-Umgebung dient und jedes Wochenende von Adobe Workfront aktualisiert wird. Alle Support-Pakete haben Zugriff auf die Sandbox-Vorschau. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Die [!DNL Adobe Workfront] Sandbox-Vorschau-Umgebung</a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 und 2</strong></td>
        <td>Die benutzerdefinierte Aktualisierungs-Sandbox ist eine separate Testumgebung, die von Ihnen manuell aktualisiert wird. Es fallen zusätzliche Kosten an, um die benutzerdefinierte Aktualisierungs-Sandbox zu erhalten. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">Die [!DNL Adobe Workfront] benutzerdefinierte Sandbox-Aktualisierungsumgebung</a>.</td>
    </tr>
</table>

>[!TIP]
>
>Es wird empfohlen, zunächst die Blueprint in einer Sandbox-Umgebung zu installieren. Auf diese Weise können Sie den Inhalt des Blueprints testen und sicherstellen, dass er gut zu Ihrer Organisation passt, ohne Änderungen an Live-Daten vorzunehmen.

>[!NOTE]
>
>Bestimmte Blueprints können nur zu Testzwecken in der Vorschau-Umgebung installiert werden. Wenn Sie in Ihrer Produktionsumgebung, Sandbox 1 oder Sandbox 2 auf Nur-Vorschau-Inhalt zugreifen, ist die Schaltfläche Installieren nicht aktiv und möglicherweise wird eine Warnmeldung angezeigt.\
>Darüber hinaus ist die Funktion zum Umschalten der Umgebung beim Zugriff auf Inhalte, die nur in der Vorschau angezeigt werden, eingeschränkt, selbst wenn Sie sich in der Vorschau-Umgebung befinden.

## Blueprint installieren

{{step1-to-blueprints}}

1. Suchen Sie die Blueprint, die Sie installieren möchten. Sie können rechts auf der Seite nach Anwendungsfall, Reifegrad, Installationsstatus und Typ filtern.
1. (Optional) Klicken Sie auf **[!UICONTROL Details]**, um mehr über die Funktionsweise des Blueprints zu erfahren.
1. Klicken Sie auf **[!UICONTROL Installieren]**.
1. Wählen Sie die Installation in Ihrer Produktionsumgebung oder einer Sandbox-Umgebung aus.\
   Weitere Informationen finden Sie unter [Wo sollte ich eine Blueprint installieren?](#where-should-i-install-a-blueprint) Abschnitt in diesem Artikel.
1. Auf der **Konfigurieren** können Sie eine der folgenden Aktionen ausführen:

   * Blueprint unverändert installieren. Bei Blueprint-Typen, für die keine Konfiguration erforderlich ist, ist dies die einzige Option. Für Blueprint-Typen, die konfiguriert werden müssen, können Sie optional festlegen, dass die Blueprint jetzt installiert und zu einem späteren Zeitpunkt konfiguriert wird. Klicken Sie **[!UICONTROL Unverändert installieren]**.
   * Konfigurieren Sie die Blueprint vor der Installation für Blueprints, die konfiguriert werden müssen. Wählen Sie Ihre Konfiguration aus und klicken Sie dann auf **[!UICONTROL Blueprint installieren]**.

     Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../administration-and-setup/blueprints/configure-template-package.md).

   Die Installation wird abgeschlossen. In einer Meldung wird eine Liste der spezifischen Objekte (z. B. Rollen, Teams oder Gruppen) angezeigt, die mit der Blueprint erfolgreich installiert wurden, sowie der Objekte, die nicht installiert werden konnten.

Nach der Installation der Blueprint sind möglicherweise einige zusätzliche Aktionen erforderlich, um sie vollständig bereitzustellen. Weitere Informationen finden Sie [Aktionen, die nach der Installation eines Blueprints durchgeführt werden sollen](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
