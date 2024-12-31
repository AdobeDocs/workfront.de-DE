---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Hinzufügen erweiterter Proofing-Optionen mit der Adobe Workfront-API
description: Hinzufügen erweiterter Proofing-Optionen mit der Adobe Workfront-API
author: Becky
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---


# Hinzufügen erweiterter Proofing-Optionen beim Erstellen eines Korrekturabzugs über die Adobe Workfront-API

Beim Erstellen eines Korrekturabzugs in der Workfront-API können Sie erweiterte Proofing-Optionen hinzufügen.

Verwenden Sie einen der folgenden Workflows, um mithilfe der API Korrekturabzugsoptionen zu einem Korrekturabzug hinzuzufügen:

* (Empfohlen) Erstellen Sie einen einfachen Korrekturabzug mit der Workfront-API und fügen Sie dann dem Korrekturabzug mithilfe der ProofHQ-API erweiterte Proofing-Optionen hinzu

* Erstellen eines Korrekturabzugs mit erweiterten Proofing-Optionen mithilfe von JSON in der Workfront-API

## Erstellen eines Korrekturabzugs mit den Workfront- und ProofHQ-APIs (empfohlen) {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

In diesem Abschnitt wird beschrieben, wie Sie einen Korrekturabzug mit erweiterten Proofing-Optionen über die Workfront-API erstellen, indem Sie eine Kombination aus Workfront- und ProofHQ-APIs verwenden.

Die ProofHQ-API umfasst eine Vielzahl von Aktionen, die für Korrekturabzüge in der Workfront-API nicht verfügbar sind. Mithilfe dieser Aktionen können Sie den Korrekturabzug präziser ändern oder konfigurieren, als in der Workfront-API verfügbar ist.

Einen Überblick über die ProofHQ-API finden Sie unter [ProofHQ - Übersicht](../../proofhq-api/general/overview.md). Weitere Informationen finden Sie in der [ProofHQ-Dokumentation](https://api.proofhq.com/home.html).

>[!NOTE]
>
>* Die Workfront-API ist eine REST-ful-API. Die ProofHQ-API ist eine SOAP-API.
>* Die in der ProofHQ-API erstellten Testsendungen werden nicht automatisch mit Workfront verknüpft. Daher empfehlen wir, Testsendungen in der Workfront-API zu erstellen, bevor Sie sie mit der ProofHQ-API aktualisieren.
>

### Erstellen eines Korrekturabzugs mit erweiterten Proofing-Optionen

1. Erstellen Sie einen Testversand mithilfe der `Document createProof` in der Workfront-API.

   >[!NOTE]
   >
   >Legen Sie beim Erstellen des Korrekturabzugs `{}` als Wert für den `advancedProofingOptions` fest.

1. Nachdem der Korrekturabzug erstellt wurde, verwenden Sie die ProofHQ-API, um erweiterte Optionen hinzuzufügen.

### Beispiele

Dieser Abschnitt zeigt einige Beispiel-Aktualisierungen, die Sie mit der ProofHQ-API vornehmen können.

**Beispiele:**

* [Ein Korrekturabzug kann heruntergeladen werden, enthält eine Nachricht und wird öffentlich freigegeben](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [Aktualisieren Sie einen Schritt, sodass er nicht privat, nicht obligatorisch und nur mit einer Genehmigung ist](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [Hinzufügen von zwei Empfängern zu einem Korrekturabzug ohne primären Entscheidungsträger](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**Ein Korrekturabzug kann heruntergeladen werden, enthält eine Nachricht und wird öffentlich freigegeben**

Die Dokumentation für diesen Endpunkt finden Sie auf der Seite [ProofHQ API updateProof](https://api.proofhq.com/home/proofs/updateproof.html).

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateProof>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{file_id}}</FileID>
            <OwnerID>0</OwnerID>
            <Name>{{proof_name}}}</Name>
            <Subject>Email subject here</Subject>
            <Message>Email message here</Message>
            <EnableDownload>true</EnableDownload>
            <EnableTeamURL>true</EnableTeamURL>
        </soap:updateProof>
    </soapenv:Body>
</soapenv:Envelope>
```

**Aktualisieren Sie einen Schritt, sodass er nicht privat, nicht obligatorisch und nur mit einer Genehmigung ist**

Die Dokumentation für diesen Endpunkt finden Sie auf der Seite [ProofHQ API updateWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html).

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateWorkflowProofStage>
        <SessionID>{{session_id}}</SessionID>
        <FileID>{{proof_id}}</FileID>
        <Stage>
            <stage_id>{{stage_id}}</stage_id>
            <name>{{stage_name}}</name>
                <stage_one_decision_only>true</stage_one_decision_only>
                <stage_private>false</stage_private>
                <mandatory>false</mandatory>
            </Stage>
        </soap:updateWorkflowProofStage>
    </soapenv:Body>
</soapenv:Envelope>
```

**Fügen Sie zu einem Korrekturabzug zwei Empfänger hinzu, ohne dass ein primärer Entscheidungsträger vorhanden ist**

Die Dokumentation für diesen Endpunkt finden Sie auf der Seite [ProofHQ API addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html).

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:addWorkflowProofReviewers>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{proof_id}}</FileID>
            <Recipients>
                <item>
                <email>{{recipient_email_1}}</email>
                <role>5</role>
                <name>{{recipient_name_1}}</name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
                <item>
                <email> {{recipient_email_2}} </email>
                <role>5</role>
                <name> {{recipient_name_2}} </name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
            </Recipients>
            <SuppressNewProofNotification></SuppressNewProofNotification>
        </soap:addWorkflowProofReviewers>
    </soapenv:Body>
</soapenv:Envelope>
```

## Erstellen eines Korrekturabzugs mit JSON in der Workfront-API

In diesem Abschnitt wird beschrieben, wie Sie einen Korrekturabzug mit erweiterten Proofing-Optionen über die Workfront-API erstellen und dabei JSON als Parameterwert in der Workfront-API verwenden

### Erstellen eines Korrekturabzugs mit erweiterten Proofing-Optionen

Sie können Testsendungen über die Workfront-API erstellen, indem Sie die `Document createProof` Aktion verwenden. Diese Aktion akzeptiert den `advancedProofingOptions`-Parameter mit dem Werttyp `string`. Um erweiterte Proofing-Optionen in Ihre `createProof`-Aktion aufzunehmen, müssen Sie die Optionen im `advancedProofingOptions` Parameter im JSON-Format eingeben.

>[!NOTE]
>
>Es kann schwierig sein, die Felder vorherzusagen, die in Ihre AdvancedProofingOptions-JSON aufgenommen werden sollen. Möglicherweise möchten Sie die Netzwerkdaten Ihres Unternehmens überprüfen, während Sie das erweiterte Proofing in Workfront verwenden, und Ihre JSON-Datei auf den Feldern und Werten basieren, die von Ihrem Unternehmen häufig verwendet werden.
>
>Da diese Felder schwer vorhersehbar sein können, empfehlen wir, einen Korrekturabzug mit der Workfront-API zu erstellen und ihn dann mit der ProofHQ-API zu aktualisieren. Weitere Informationen finden Sie unter [Erstellen eines Korrekturabzugs mit den Workfront- und ProofHQ-APIs (empfohlen)](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) in diesem Artikel

### Beispiel

Dieses Beispiel zeigt Felder und Formatierungen, die Sie beim Erstellen Ihrer JSON für den `advancedProofingOptions` verwenden können. Ihre `advancedProofingOptions` JSON-Datei kann mehr oder weniger Felder enthalten als hier gezeigt.

**Beispiel:**

<!-- [Copy](javascript:void(0);) -->

```
{
    "stages": [
        {
            "name": "stage1",
            "lockOn": 1,
            "position": 1,
            "isPrivate": false,
            "activateOn": 1,
            "recipients": [
                {
                    "name": "",
                    "role": 5,
                    "email": "user1_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": null
                },
                {
                    "name": "",
                    "role": 5,
                    "email": "user2_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": false
                }
            ],
            "isMandatory": false,
            "deadlineDate": null,
            "deadlineTime": null,
            "isOneApproval": true,
            "activateOnDate": null,
            "parentPosition": null,
            "activateOnDecision": null,
            "deadlineCalculateOn": null,
            "deadlineBusinessDays": null
        }
    ],
    "message": "",
    "subject": "",
    "templates": [],
    "hasMessage": true,
    "canDownload": true,
    "customfields": [],
    "hasPublicSharing": true,
    "isAutomatedWorkflow": true,
    "stageBasedVisibility": 0
}
```
