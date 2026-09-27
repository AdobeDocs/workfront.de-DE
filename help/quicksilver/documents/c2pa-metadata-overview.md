---
product-area: documents
navigation-topic: documents-navigation-topic
title: C2PA-Metadaten in Adobe Workfront
description: Erfahren Sie, was C2PA-Metadaten sind und wie Adobe Workfront sie in den Dokumenten beibehält, die Sie hochladen, speichern und herunterladen.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%
---
# C2PA-Metadaten in Adobe Workfront

C2PA-Metadaten sind sichere, manipulationssichere Informationen, die mit einem Teil des Inhalts gesendet werden. Wenn generative KI (GenAI) verwendet wird, um ein Bild, Video oder eine Audiodatei zu erstellen oder zu ändern, werden diese Fakten in C2PA-Metadaten aufgezeichnet, sodass jeder, der die Datei erhält, sehen kann, wie sie erstellt wurde.

C2PA-Metadaten basieren auf dem offenen [C2PA](https://c2pa.org/).

## Was C2PA-Metadaten enthalten

C2PA-Metadaten umfassen:

* Der Name des Anbieters, der das GenAI-Tool bereitgestellt hat.
* Der Name und die Versionsnummer des GenAI-Systems, das zum Erstellen oder Ändern des Inhalts verwendet wird.
* Datum und Uhrzeit der Erstellung oder Änderung des Inhalts.
* Eine eindeutige Kennung.

C2PA-Metadaten enthalten keine personenbezogenen Daten (PII).

## Handhabung von C2PA-Metadaten durch Workfront

Adobe Workfront ändert die Metadaten der Dateien, mit denen Sie arbeiten, nicht. Wenn Sie eine Datei hochladen, die bereits C2PA-Metadaten enthält, behält Workfront diese Informationen unverändert bei, da die Datei in gespeichert und von Workfront heruntergeladen wird.

Da die Metadaten in der Datei selbst eingebettet sind, bleiben sie durch Ihre Workfront-Workflows intakt, sodass die Herkunftsinformationen beim Inhalt bleiben, wenn er Workfront verlässt.
