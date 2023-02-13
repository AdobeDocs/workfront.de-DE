---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Rich-Text-Feldspeicherung in der API
description: Wenn ein Objekt wie ein Projekt, ein Problem oder eine Aufgabe Rich-Text enthält, wird es gespeichert und über die Workfront-API als Parameterwert zugänglich gemacht.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Rich-Text-Feldspeicherung in der API

Wenn ein Objekt wie ein Projekt, ein Problem oder eine Aufgabe Rich-Text enthält, wird es gespeichert und über die Workfront-API als Parameterwert zugänglich gemacht.

Das Anfordern von Textinformationen aus einem Projektobjekt, das Rich-Text enthält, kann mithilfe des Felds erfolgen **parameterValues**.

Beispielsweise könnte eine einfache HTTP-Anforderung wie folgt aussehen:

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

Wenn dieses Beispielprojekt ein benutzerdefiniertes Formular mit 3 benutzerdefinierten Feldern enthielt: Berechnungsfeld, Absatztext und Rich 1. Dann gibt die obige Anfrage eine Antwort zurück, die der folgenden ähnelt, wobei das Feld &quot;rich 1&quot;ein Rich-Text-Parameterfeld und der Textwert &quot;ist&quot;**Hallo** *Welt!*&quot;:

```
{
	Data: {
		ID: “xxxxxxxxxxxxxxxxxxxxxxx”,
		name: “new project with rich text”,
		objCode: “PROJ”,
		- parameterValues: {
			DE:rich 1: “{
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
		}”,
		DE: paragraph text: “here is some paragraph text”,
		DE: calc field: “here is a calc field entry”,
		}
	}
}
```

Detaillierte Informationen dazu, wie Rich-Text-Informationen gespeichert und über die Adobe Workfront-API abgerufen werden können, finden Sie unter [Rich-Text-Felder in der Adobe Workfront-API](../../../wf-api/general/rich-text-field-api.md).
