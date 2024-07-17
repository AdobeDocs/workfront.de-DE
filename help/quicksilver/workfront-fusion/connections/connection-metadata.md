---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-2-0
title: Verbindungsmetadaten in Adobe Workfront Fusion
description: Adobe Workfront Fusion erfordert zusätzlich zu einer Adobe Workfront-Lizenz eine Adobe Workfront Fusion-Lizenz.
author: Becky
feature: Workfront Fusion
exl-id: af260c63-3385-4d5c-abc2-d5c23175be40
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Verbindungsmetadaten in Adobe Workfront Fusion

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] erfordert zusätzlich zu einer [!DNL Adobe Workfront] -Lizenz eine [!DNL Adobe Workfront Fusion] -Lizenz.

Nicht alle Verbindungen sind gleich. Die Unterschiede zwischen Verbindungen zu verstehen, ist sehr wichtig, um deren Geschäftskontext zu kennen. Fusion verwendet Metadaten zur Identifizierung wichtiger Attribute einer Verbindung.

Beim Erstellen einer neuen Verbindung können Verbindungsmetadaten festgelegt werden. Diese Attribute befinden sich im selben Dialogfeld, das zum Einrichten einer Verbindung verwendet wird:

![Verbindungsmetadaten](assets/connection-metadata-setup.png)

Fusion-Benutzer können Verbindungen im Bereich Verbindungen anzeigen und bearbeiten.

![Verbindungsmetadaten im Bereich &quot;Verbindungen&quot;](assets/connections-area-metadata.png)

## Umgebungstyp

Fusionsverbindungen können sowohl von Produktions- als auch von Nicht-Produktionssystemen verwendet werden. Die Kenntnis des Unterschieds ist sehr wichtig für den Schutz von Produktionsumgebungen. Beachten Sie, dass der Umgebungstyp wie andere Verbindungsmetadaten nur zu Informationszwecken verwendet wird. Die Benutzer sind weiterhin für die genaue Einstellung dieses Attributs verantwortlich.

## Authentifizierungstyp

Fusion-Verbindungen können sowohl für Dienstkonten als auch für persönliche Konten verwendet werden. Dienstkonten werden für die Authentifizierung verwendet, wenn ein Szenario als Fusion automatisiert wird. Personenkonten sind Authentifizierungen, die auf einer bestimmten Person basieren. Welcher Authentifizierungstyp verwendet wird, hängt von den Anforderungen des Szenarios ab. Persönliche Konten sollten für automatisierte Benutzeraktionen verwendet werden. Wenn beispielsweise ein Fusion-Szenario die Genehmigung durch eine bestimmte Person automatisiert, sollte der Authentifizierungstyp für diese Person sein. Andernfalls fungiert Fusion als Fusion und sollte der Typ &quot;Service Account&quot;sein.

Beachten Sie, dass der Typ wie andere Verbindungsmetadaten nur zu Informationszwecken verwendet wird. Die Benutzer sind weiterhin dafür verantwortlich, dieses Attribut manuell genau festzulegen.

Weitere Informationen zu Authentifizierungstypen finden Sie unter [Authentifizierung](https://developer.adobe.com/developer-console/docs/guides/authentication/) im Handbuch zur Adobe-Authentifizierung.
