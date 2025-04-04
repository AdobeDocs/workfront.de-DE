---
title: Festlegen einer benutzerdefinierten Bedingung als Standard für Aufgaben und Probleme
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Wenn ein(e) Benutzende(r) auf Bearbeiten klickt oder einen Aktualisierungskommentar zu einer neuen Aufgabe hinzufügt, der er/sie zugewiesen wurde (ohne manuell eine Bedingung für die Aufgabe festzulegen), zeigt Adobe Workfront die Standardbedingung für Aufgaben an, die im Setup konfiguriert ist. Dasselbe gilt für Probleme.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Benutzerdefinierte Bedingung als Standard für Aufgaben und Probleme festlegen

Wenn ein(e) Benutzende(r) auf Bearbeiten klickt oder einen Aktualisierungskommentar zu einer neuen Aufgabe hinzufügt, der er/sie zugewiesen wurde (ohne manuell eine Bedingung für die Aufgabe festzulegen), zeigt Adobe Workfront die Standardbedingung für Aufgaben an, die im Setup konfiguriert ist. Dasselbe gilt für Probleme.

Workfront verwendet die integrierte Bedingung reibungslos laufen als Standardbedingung für Aufgaben und separat für Probleme. Als Workfront-Administrator können Sie die Standardbedingung für diese beiden Objekttypen in eine von Ihnen erstellte benutzerdefinierte Bedingung ändern.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Legen Sie eine benutzerdefinierte Bedingung als Standardbedingung für Aufgaben oder für Probleme fest:

{{step-1-to-setup}}

1. Klicken Sie **Projektvoreinstellungen** > **Bedingungen**.

1. Klicken Sie auf **Registerkarte** Aufgaben“ oder **Probleme**.

1. Klicken Sie **Standardbedingungen festlegen**.
1. Klicken Sie im Dropdown-Menü auf die benutzerdefinierte Bedingung, die als Standardbedingung für Aufgaben (oder Probleme) verwendet werden soll.
1. Klicken Sie auf **Speichern**.

>[!NOTE]
>
>* Ein Benutzer, der einer Aufgabe oder einem Problem zugewiesen ist oder Berechtigungen zum Verwalten dafür hat, kann seine Bedingung manuell ändern. Weitere Informationen finden Sie unter [Bedingung für Aufgaben und Probleme aktualisieren](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* Die drei Standardbedingungen für Aufgaben und Probleme, die im Zusammenhang mit Workfront auftreten, funktionieren problemlos, sind Besorgnis erregend und haben schwerwiegende Probleme zur Folge. Sie können diese Bedingungen nicht ausblenden oder löschen, aber Sie können ihre Namen und Farben ändern. Sie können auch neue erstellen, die stattdessen verwendet werden, wie in [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md) beschrieben.
>

Informationen zum Konfigurieren einer benutzerdefinierten Bedingung als Standardbedingung für Projekte finden Sie unter [Festlegen einer benutzerdefinierten Bedingung als Standardbedingung für Projekte](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Informationen zu benutzerdefinierten Bedingungen finden Sie unter [Benutzerdefinierte Bedingungen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
