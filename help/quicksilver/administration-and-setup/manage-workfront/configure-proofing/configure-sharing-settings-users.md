---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Freigabeeinstellungen für Ihre Benutzer konfigurieren
description: Als Adobe Workfront-Administrator oder Workfront Proof-Administrator können Sie die Benutzerkonten konfigurieren, für die Testsendungen freigegeben werden können, festlegen, ob die Benutzer alle Versionen eines Testversands sehen können und wann Benutzer Zugriff auf freigegebene Elemente erhalten.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 0%

---

# Freigabeeinstellungen für Ihre Benutzer konfigurieren

Als Adobe Workfront-Administrator oder Workfront Proof-Administrator können Sie die Benutzerkonten konfigurieren, für die Testsendungen freigegeben werden können, festlegen, ob die Benutzer alle Versionen eines Testversands sehen können und wann Benutzer Zugriff auf freigegebene Elemente erhalten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Premium oder Auswahl</p> <p>Weitere Informationen zum Testen des Zugriffs mit den verschiedenen Plänen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeit oder Plan</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>In Ihrem Profil für Testberechtigungen muss "Administrator"ausgewählt sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Konfigurieren des Testzugriffs eines Benutzers</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## Freigabe für andere Konten konfigurieren

{{step1-to-proofing}}

1. Klicken Sie auf **Einstellungen** > **Kontoeinstellungen** und dann auf die Registerkarte **Einstellungen**.

1. Klicken Sie im Abschnitt **Freigabe** rechts neben **Freigabe für** zulassen auf **Einrichten**.

1. Wählen Sie in der angezeigten Dropdown-Liste eine Option aus, um festzulegen, ob Sie Testsendungen für jedermann verfügbar machen, die Freigabe Ihrer Testsendungen auf Ihr eigenes Konto beschränken oder auf Ihr eigenes Konto und die Partnerkonten, mit denen Sie zusammenarbeiten, beschränken möchten.
1. Klicken Sie auf **Speichern.**

## Sichtbarkeit für alle Versionen eines freigegebenen Testversands konfigurieren

{{step1-to-proofing}}

1. Klicken Sie auf **Einstellungen** > **Kontoeinstellungen** und dann auf die Registerkarte **Einstellungen**.

1. Wählen Sie im Abschnitt **Freigabe** rechts neben **Empfänger können alle Versionen anzeigen** die Option **Aktivieren** oder **Deaktivieren** aus, um anzugeben, ob Sie Empfängern erlauben möchten, alle Versionen eines Testversands im Testversand-Viewer anzuzeigen, wenn die Testversand-URL aktiviert ist.

## Konfigurieren der Sichtbarkeit des Testversands basierend auf der Workflow-Staging-Aktivität

Sie können angeben, wann Testsendungen mit einem automatisierten Workflow für Benutzer, die mit einer bestimmten Phase verbunden sind, sichtbar sind.

>[!NOTE]
>
>* Diese Option ist nur bei Verwendung der eigenständigen Workfront Proof-Anwendung verfügbar. Sie steht nicht zur Verfügung, wenn eine Workfront Proof-Instanz verwendet wird, die in Workfront integriert ist, oder wenn ein Testversand in Workfront durchgeführt wird.
>* Benutzer erhalten eine E-Mail-Benachrichtigung über den Testversand erst, nachdem er in die Phase gelangt ist, mit der der Benutzer verknüpft ist, unabhängig von dieser Einstellung.
>

So konfigurieren Sie, wann Testsendungen mit einem automatisierten Workflow für Benutzer sichtbar sind:

{{step1-to-proofing}}

1. Klicken Sie auf **Einstellungen** > **Kontoeinstellungen** und dann auf die Registerkarte **Einstellungen**.

1. Aktivieren oder deaktivieren Sie im Abschnitt **Freigabe** die Sichtbarkeit des Testversands basierend auf der Aktivierung der Bühne **.**

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Deaktiviert</strong> (Standard)</td> 
      <td>Testsendungen sind für Benutzer zum Zeitpunkt der Erstellung des Testversands sichtbar.<br><p>Jeder Benutzer, der einer Phase im Workflow für den Testversand zugeordnet ist, kann den Testversand unmittelbar nach der Erstellung des Testversands in den Suchergebnissen sehen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aktiviert</strong> </td> 
      <td> <p>Testsendungen sind für Benutzer erst sichtbar, nachdem die Phase, mit der sie verknüpft sind, <strong>aktiv</strong> geworden ist.</p> <p><b>NOTE</b>:   
        <ul> 
         <li><em style="font-style: normal;">Nach der Aktivierung dieser Option sind vorhandene Testsendungen weiterhin für Benutzer sichtbar, die sie beim Erstellen anzeigen konnten.</em> </li> 
         <li>Nachdem ein Benutzer Zugriff auf eine Version eines Testversands erhält (da die Phase, mit der der Benutzer verknüpft ist, aktiv wird), kann der Benutzer nur die Version sehen, in der die Bühne aktiviert ist. Wenn eine frühere Version die Stufe, mit der der Benutzer verknüpft ist, nie erreicht hat, kann der Benutzer diese Version des Testversands nicht sehen.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
