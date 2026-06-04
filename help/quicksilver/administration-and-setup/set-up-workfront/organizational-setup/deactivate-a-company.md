---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Deaktivieren oder Reaktivieren eines Unternehmens
description: Sie können ein Unternehmen, das Sie nicht mehr verwenden, deaktivieren und dabei alle zugehörigen historischen Daten beibehalten. Wenn Sie ein Unternehmen deaktivieren, das bereits irgendwo im System verwendet wird, funktioniert es weiterhin wie immer. Es wird nicht entfernt oder blockiert.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
TQID: https://experienceleague.adobe.com/GrxcFYKSrmJsaITu6twBnTZxfkMcvsnRdfn7-qoSXI4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 335
ht-degree: 12%

---

# Deaktivieren oder Reaktivieren eines Unternehmens

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

Sie können ein Unternehmen, das Sie nicht mehr verwenden, deaktivieren und dabei alle zugehörigen historischen Daten beibehalten. Wenn Sie ein Unternehmen deaktivieren, das bereits irgendwo im System verwendet wird, funktioniert es weiterhin wie immer. Es wird nicht entfernt oder blockiert.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] Packstück</p> </td> 
   <td><p>Beliebig</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] Lizenz</p> </td> 
   <td><p>[!UICONTROL Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
  <td> <p>Sie müssen eine der folgenden Möglichkeiten haben:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene [!UICONTROL Systemadministrator], mit der Sie jede Firma im System bearbeiten können.</p> </li> 
     <li> <p>Administrativer Zugriff auf die Verwaltung von Unternehmen, wodurch Sie jedes Unternehmen im System bearbeiten können.</p> </li> 
    </ul> <p><b>HINWEIS</b>:
     <ul> 
      <li> <p>Sie können auch Firmen verwalten, die mit einer beliebigen Gruppe verknüpft sind, der Sie als Gruppenadministrator zugewiesen sind.</p> </li> 
      <li> <p>Um Benutzer zum [!DNL Workfront] hinzuzufügen oder daraus zu entfernen, benötigen Sie eine der folgenden Eigenschaften:</p> 
       <ul> 
        <li> <p>Zugriffsebene des [!UICONTROL Systemadministrators]. </p> </li> 
        <li> <p><b>[!UICONTROL Users]</b> Einstellung in der Zugriffsebene konfiguriert, um den[!UICONTROL Edit]</b>-Zugriff zu <b>, wobei <b>[!UICONTROL Create]</b> und mindestens eine der beiden <b>[!UICONTROL User Admin]</b> Optionen unter <b> </b>[!UICONTROL Feinabstimmung der Einstellungen]<img src="assets/gear-icon-in-access-levels.png"> aktiviert ist. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Wenn <b>[!UICONTROL User Admin (Group Users)]</b> aktiviert ist, müssen Sie unter diesen beiden Optionen Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Deaktivieren oder Reaktivieren eines Unternehmens

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL Firmen]** ![Symbol Firmen](assets/companies-icon-left-panel.png).

1. Wählen Sie ein oder mehrere Unternehmen zum Deaktivieren oder Reaktivieren aus.
1. Klicken Sie **[!UICONTROL Bearbeiten]**.<!--MAKE THIS A SEPARATE NUMBERED LINE<span class="preview">(Conditional) In the Preview environment, disable the **[!UICONTROL Is Active]** option to deactivate it, or enable the option to activate it.</span>-->
1. Deaktivieren Sie für ein einzelnes Unternehmen die Option **[!UICONTROL Ist aktiv]**, um sie zu deaktivieren, oder aktivieren Sie die Option, um sie zu aktivieren. <!--ADD TO THE FRONT OF THIS SENTENCE In the Production environment, -->

   ODER

   Bei mehreren Unternehmen wählen Sie **[!UICONTROL Nein]** aus dem Dropdown-Menü **[!UICONTROL Ist aktiv]** aus, um sie zu deaktivieren, oder **[!UICONTROL Ja]**, um sie zu aktivieren.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.
