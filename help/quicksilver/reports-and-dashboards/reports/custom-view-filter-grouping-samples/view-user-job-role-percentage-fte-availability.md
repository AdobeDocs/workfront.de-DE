---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Anteil der User Stellenrollen an der Verfügbarkeit von Vollzeitäquivalenten"
description: Sie können dem Ansicht einer User Liste eine Spalte hinzufügen, um eine Liste der Stellenrollen anzuzeigen, mit denen die User verknüpft ist, sowie den Prozentsatz der VZÄ-Verfügbarkeit für jede Rolle der Stelle, wie in der User Profil definiert.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Ansicht: Prozentsatz der FTE-Verfügbarkeit der Benutzerauftragsrolle

Sie können der Ansicht einer Benutzerliste eine Spalte hinzufügen, um eine Liste der mit dem Benutzer verknüpften Vorgangsrollen sowie den Prozentsatz der FTE-Verfügbarkeit für jede Vorgangsrolle anzuzeigen, wie im Benutzerprofil definiert.

Informationen zum Definieren des Prozentsatzes der FTE-Verfügbarkeit für Benutzer finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![User_mit_Prozent_Verfügbarkeit_per_Rolle.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## Voraussetzungen für den Zugriff

Sie benötigen die folgenden Zugriffsrechte, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Systems Arbeitsfrontplan*</td> 
   <td> <p>Jegliche</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Systems Workfront-Lizenz*</td> 
   <td> <p>Anfrage zum Ändern einer Ansicht </p>
   <p>Abo-Option, um einen Bericht zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Objekt Berechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Um herauszufinden, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben, wenden Sie sich an Ihren Workfront-Administrator.

## Ansicht User Stellenrolle Prozentsatz der VZÄ-Verfügbarkeit

1. OK an eine Liste von Benutzern.
1. Wählen Sie aus dem Dropdownmenü **Ansicht** die Option **Neue Ansicht** aus.

1. Klicken Sie im Bereich **Spaltenvorschau** auf **Spalte hinzufügen**.

1. Klicken Sie auf die Überschrift der neuen Spalte und dann auf Zu **Text Modus** wechseln.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf zum Bearbeiten von **Text** klicken.
1. Entfernen den im Feld &quot;Text Modus **&quot; enthaltenen** Text und ersetzen Sie ihn durch folgenden Code:
   <pre>displayname=Rollen Zeit Prozent<br>listdelimiter=<p><br>listmethod=nested(userRoles).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({role},'-',{timePercentage},'%')<br>valueformat=HTML</pre>

1. Klicken Sie auf &quot; **Speichern**&quot; und dann **auf &quot;Speichern Ansicht**&quot;.

1. (Optional) Geben Sie einen Namen für die Ansicht an und klicken Sie dann auf Speichern Ansicht ****.
