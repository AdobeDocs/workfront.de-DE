---
title: Festlegen einer benutzerdefinierten Bedingung als Standard für Aufgaben und Probleme
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Wenn ein Benutzer auf Bearbeiten klickt oder einen Aktualisierungskommentar zu einer neuen Aufgabe hinzufügt, der er zugewiesen wurde (ohne manuell eine Bedingung für die Aufgabe festzulegen), zeigt Adobe Workfront die Standardbedingung für Aufgaben an, die in Einrichtung konfiguriert ist. Dasselbe gilt für Probleme.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Benutzerdefinierte Bedingung als Standard für Aufgaben und Probleme festlegen

Wenn ein Benutzer auf Bearbeiten klickt oder einen Aktualisierungskommentar zu einer neuen Aufgabe hinzufügt, der er zugewiesen wurde (ohne manuell eine Bedingung für die Aufgabe festzulegen), zeigt Adobe Workfront die Standardbedingung für Aufgaben an, die in Einrichtung konfiguriert ist. Dasselbe gilt für Probleme.

Workfront verwendet die integrierte Bedingung reibungslos als Standardbedingung für Aufgaben und separat für Probleme. Als Workfront-Administrator können Sie die Standardbedingung für beide Objekttypen in eine von Ihnen erstellte benutzerdefinierte Bedingung ändern.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Legen Sie eine benutzerdefinierte Bedingung als Standardbedingung für Aufgaben oder Probleme fest:

{{step-1-to-setup}}

1. Klicken Sie auf **Projekteinstellungen** > **Bedingungen**.

1. Klicken Sie auf die Registerkarte **Aufgaben** oder **Probleme**.

1. Klicken Sie auf **Standardbedingungen festlegen**.
1. Klicken Sie im Dropdown-Menü auf die benutzerdefinierte Bedingung, die Sie als Standardbedingung für Aufgaben (oder Probleme) festlegen möchten.
1. Klicken Sie auf **Speichern**.

>[!NOTE]
>
>* Benutzer, die einer Aufgabe oder einem Problem zugewiesen sind oder über Verwaltungsberechtigungen verfügen, können ihre Bedingung manuell ändern. Weitere Informationen finden Sie unter [Bedingung für Aufgaben und Probleme aktualisieren](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* Die drei Standardbedingungen für Aufgaben und Probleme, die mit Workfront in Verbindung stehen, sind reibungslos verlaufen, einige Probleme und große Hindernisse. Sie können diese Bedingungen nicht ausblenden oder löschen, aber Sie können ihre Namen und Farben ändern. Alternativ können Sie neue erstellen, die stattdessen verwendet werden sollen, wie unter [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md) beschrieben.
>

Informationen zum Konfigurieren einer benutzerdefinierten Bedingung als Standardbedingung für Projekte finden Sie unter [Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Weitere Informationen zu benutzerdefinierten Bedingungen finden Sie unter [Benutzerdefinierte Bedingungen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
