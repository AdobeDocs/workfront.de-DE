---
title: Überarbeiten von berechneten Feldformeln mit dem KI-Assistenten
content-type: reference
description: Sie können den KI-Assistenten verwenden, um Fehler in Ihren ungültigen benutzerdefinierten Ausdrücken in berechneten Feldern zu beheben.
author: Becky
feature: Get Started with Workfront
exl-id: 5f144a6f-5c2a-42fc-a961-ab9066432d93
source-git-commit: bec1318d83938964697d76b83062ef11745802e3
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Generieren oder Überarbeiten von berechneten Feldformeln mit dem KI-Assistenten

Sie können den KI-Assistenten verwenden, um Formeln basierend auf einer von Ihnen angegebenen Eingabeaufforderung zu generieren. Sie können auch Fehler in Ihren ungültigen benutzerdefinierten Ausdrücken in berechneten Feldern beheben.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td><p>Neu: Prime oder Ultimate</p>
       <p>oder</p>
       <p>Aktuell: Nicht verfügbar</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Nicht verfügbar</p></td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

* Ihr Workfront-Administrator muss den KI-Assistenten für Ihr Unternehmen aktiviert haben.

  Weitere Informationen finden Sie unter [Voraussetzungen für den KI-](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)) im Artikel KI-Assistent - Übersicht.
* Ihr Workfront-Administrator muss den KI-Assistenten für Ihre Zugriffsebene aktiviert haben.

  Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren des KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

<!--## Generate a calculated field expression-->

## Überarbeiten eines berechneten Feldausdrucks

Beim Erstellen des berechneten Felds im benutzerdefinierten Formular-Builder wird unter dem Feld eine Fehlermeldung angezeigt, wenn die Formel ungültig ist.

![Fehler mit ungültigem Ausdruck](assets/invalid-expression.png)

Der KI-Assistent kann Ihnen dabei helfen, Ihre Formel in einen gültigen berechneten Feldausdruck zu überarbeiten.

So ändern Sie einen ungültigen berechneten Feldausdruck:

1. Klicken Sie auf **KI** Assistent![ Symbol KI-Assistent](assets/ai-assistant-icon.png) in der oberen rechten Ecke des Bildschirms.
1. Geben Sie im Eingabeaufforderungsbereich am unteren Rand des KI-Assistenten eine Eingabeaufforderung ein, z. B.:
   `Rewrite this formula to remove the invalid expression error`
1. Kopieren Sie den ungültigen Ausdruck aus dem benutzerdefinierten Formular-Builder und fügen Sie ihn in den Eingabeaufforderungsbereich ein.
1. Drücken Sie **ENTER**.

   Je nachdem, wie groß oder komplex die Formel ist, kann es einige Minuten dauern, bis der KI-Assistent die überarbeitete Formel erstellt.
1. Zeigen Sie die überarbeitete Formel im Bedienfeld KI-Assistent an.
1. (Optional) Kopieren Sie die überarbeitete Formel aus dem Bedienfeld „KI-Assistent“ und fügen Sie sie in das berechnete Feld im benutzerdefinierten Formular-Builder ein.

>[!NOTE]
>
>Es wird empfohlen, das berechnete Feld zu testen, um sicherzustellen, dass es das erwartete Ergebnis abruft.

Weitere Informationen zu berechneten Feldern in Workfront finden Sie unter [Hinzufügen berechneter Felder zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

