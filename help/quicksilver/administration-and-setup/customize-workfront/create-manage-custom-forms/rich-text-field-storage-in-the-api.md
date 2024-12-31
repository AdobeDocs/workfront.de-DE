---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Speicherung von Rich-Text-Feldern in der API
description: Wenn ein Objekt wie ein Projekt, ein Problem oder eine Aufgabe Rich-Text enthält, wird es über die Workfront-API gespeichert und kann als Parameterwert darauf zugegriffen werden.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: 3f7f4557c18bbb91ece850f910350d926a9e84bf
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# Speicherung von Rich-Text-Feldern in der API

Wenn ein Objekt wie ein Projekt, ein Problem oder eine Aufgabe Rich-Text enthält, wird es über die Workfront-API gespeichert und kann als Parameterwert darauf zugegriffen werden.

Das Anfordern von Textinformationen aus einem Projektobjekt, das Rich-Text enthält, kann mit dem Feld **parameterValues** erfolgen.

Eine einfache HTTP-Anfrage könnte beispielsweise der folgenden ähneln:

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

Wenn dieses Beispielprojekt ein benutzerdefiniertes Formular mit drei benutzerdefinierten Feldern enthält: berechnetes Feld, Absatztext und Rich 1. Dann würde die obige Anfrage eine Antwort zurückgeben, die der folgenden ähnelt, wobei das Feld „rich 1“ ein Rich-Text-Parameterfeld ist und der Textwert &quot;**Hello** *World!*&quot; lautet:

```
{
    Data: {
        ID: "xxxxxxxxxxxxxxxxxxxxxxx",
        name: "new project with rich text",
        objCode: "PROJ",
        - parameterValues: {
            DE:rich 1: "{
                "blocks":[
                {
                    "key":"7eibh",
                    "text":"Hello Word!",
                    "type":"unstyled",
                    "depth":0,
                    "inlineStyleRanges":[
                    {
                        "offset":0,
                        "length":6,
                        "style":"BOLD"
                    },
                    {
                        "offset":6,
                        "length":5,
                        "style":"ITALIC"
                    }
                    ],
                    "entityRanges":[
                    ],
                "data":{
                }
                }
                ],
            "entityMap":{
            }
        }",
        DE: paragraph text: "here is some paragraph text",
        DE: calc field: "here is a calc field entry",
        }
    }
}
```

Weitere Informationen dazu, wie Rich-Text-Informationen gespeichert und über die Adobe Workfront-API abgerufen werden können, finden Sie unter [Rich-Text-Felder in der Adobe Workfront-API](../../../wf-api/general/rich-text-field-api.md).
