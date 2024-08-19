---
title: Berechnete Feldformeln mit dem KI-Assistenten überarbeiten
content-type: reference
description: Mit dem KI-Assistenten können Sie Fehler in Ihren ungültigen benutzerdefinierten Ausdrücken in berechneten Feldern beheben.
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
exl-id: 5f144a6f-5c2a-42fc-a961-ab9066432d93
source-git-commit: 513d33c653901394f35c342d8dbf89906017fb3f
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Berechnete Feldformeln mit dem AI-Assistenten generieren oder überarbeiten

Sie können den AI-Assistenten verwenden, um Formeln basierend auf einer von Ihnen angegebenen Eingabeaufforderung zu generieren. Sie können auch Fehler in Ihren ungültigen benutzerdefinierten Ausdrücken in berechneten Feldern beheben.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Berechneten Feldausdruck generieren

## Berechneten Feldausdruck überprüfen

Wenn Sie das berechnete Feld im benutzerdefinierten Formular-Builder erstellen, wird unter dem Feld eine Fehlermeldung angezeigt, wenn die Formel ungültig ist.

![Ungültiger Ausdrucksfehler](assets/invalid-expression.png)

Der KI-Assistent kann Ihnen dabei helfen, Ihre Formel in einen gültigen Ausdruck für berechnete Felder zu überarbeiten.

So überarbeiten Sie einen ungültigen Ausdruck für ein berechnetes Feld:

1. Klicken Sie auf das Symbol **AI-Assistent** ![AI-Assistent-Symbol](assets/ai-assistant-icon.png) oben rechts im Bildschirm.
1. Geben Sie im Eingabeaufforderungsbereich unten im Bedienfeld &quot;AI Assistant&quot;eine Eingabeaufforderung ein, z. B.:
   `Rewrite this formula to remove the invalid expression error`
1. Kopieren Sie den ungültigen Ausdruck aus dem benutzerdefinierten Formular-Builder und fügen Sie ihn in den Eingabeaufforderungsbereich ein.
1. Drücken Sie die Taste **Enter**.

   Je nachdem, wie groß oder komplex die Formel ist, kann es einen Moment dauern, bis der KI-Assistent die überarbeitete Formel generiert.
1. Zeigen Sie die überarbeitete Formel im Bereich &quot;KI-Assistent&quot;an.
1. (Optional) Kopieren Sie die überarbeitete Formel aus dem Bedienfeld &quot;KI-Assistent&quot;und fügen Sie sie in das berechnete Feld im benutzerdefinierten Formularersteller ein.

>[!NOTE]
>
>Es wird empfohlen, das berechnete Feld zu testen, um sicherzustellen, dass es das erwartete Ergebnis abruft.

Weitere Informationen zu berechneten Feldern in Workfront finden Sie unter [Berechnete Felder zu einem Formular hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).
