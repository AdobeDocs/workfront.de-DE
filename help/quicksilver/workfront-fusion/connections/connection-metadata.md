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
>[!DNL Adobe Workfront Fusion] benötigt zusätzlich zu einer [!DNL Adobe Workfront] eine [!DNL Adobe Workfront Fusion].

Nicht alle Verbindungen sind gleich. Die Unterschiede zwischen Verbindungen zu verstehen, ist sehr wichtig, um den Geschäftskontext zu kennen. Fusion verwendet Metadaten, um wichtige Attribute einer Verbindung zu identifizieren.

Verbindungsmetadaten können beim Erstellen einer neuen Verbindung festgelegt werden. Diese Attribute befinden sich im selben Dialogfeld, das zum Einrichten einer Verbindung verwendet wird:

![Verbindungsmetadaten](assets/connection-metadata-setup.png)

Fusion-Benutzer können Verbindungen im Bereich Verbindungen anzeigen und bearbeiten.

![Verbindungsmetadaten im Bereich „Verbindungen“](assets/connections-area-metadata.png)

## Umgebungstyp

Fusion-Verbindungen können sowohl von Produktions- als auch von Nicht-Produktionssystemen verwendet werden. Die Kenntnis der Unterschiede ist für den Schutz von Produktionsumgebungen sehr wichtig. Beachten Sie, dass der Umgebungstyp wie andere Verbindungsmetadaten nur zu Informationszwecken verwendet wird. Die Benutzer sind weiterhin für die korrekte Einstellung dieses Attributs verantwortlich.

## Authentifizierungstyp

Fusion-Verbindungen können sowohl für Service-Konten als auch für persönliche Konten verwendet werden. Service-Konten werden für die Authentifizierung verwendet, wenn ein Szenario als Fusion automatisiert wird. Personenbezogene Konten sind Authentifizierungen, die auf einer bestimmten Person basieren. Welcher Authentifizierungstyp verwendet wird, hängt von den Anforderungen des Szenarios ab. Für automatisierte Benutzeraktionen sollten persönliche Konten verwendet werden. Wenn beispielsweise ein Fusion-Szenario die Genehmigung durch eine bestimmte Person automatisiert, sollte der Authentifizierungstyp für diese Person sein. Andernfalls fungiert Fusion als Fusion, und der Typ sollte „Service-Konto“ sein.

Beachten Sie, dass der -Typ wie andere Verbindungsmetadaten nur zu Informationszwecken verwendet wird. Benutzer sind weiterhin dafür verantwortlich, dieses Attribut manuell genau festzulegen.

Weitere Informationen zu Authentifizierungstypen finden Sie unter [Authentifizierung](https://developer.adobe.com/developer-console/docs/guides/authentication/) im Authentifizierungshandbuch der Adobe.
