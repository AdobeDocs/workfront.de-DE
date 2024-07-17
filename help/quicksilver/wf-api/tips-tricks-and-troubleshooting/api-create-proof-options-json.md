---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Erweiterte Testoptionen mit der Adobe Workfront-API hinzufügen
description: Erweiterte Testoptionen mit der Adobe Workfront-API hinzufügen
author: Becky
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---


# Erweiterte Testoptionen bei der Erstellung eines Testversands über die Adobe Workfront-API hinzufügen

Beim Erstellen eines Testversands in der Workfront-API können Sie erweiterte Testversandoptionen hinzufügen.

Verwenden Sie einen der folgenden Workflows, um mithilfe der API Testversandoptionen zu einem Testversand hinzuzufügen:

* (Empfohlen) Erstellen Sie einen einfachen Testversand mithilfe der Workfront-API und fügen Sie dann mithilfe der ProofHQ-API erweiterte Testversandoptionen zum Testversand hinzu.

* Erstellen eines Testversands mit erweiterten Testoptionen mithilfe von JSON in der Workfront-API

## Erstellen eines Testversands mit den Workfront- und ProofHQ-APIs (empfohlen) {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

In diesem Abschnitt wird beschrieben, wie Sie mithilfe einer Kombination aus Workfront- und ProofHQ-APIs einen Testversand mit erweiterten Testversandoptionen über die Workfront-API erstellen.

Die ProofHQ-API enthält eine Reihe von Aktionen, die für Testsendungen in der Workfront-API nicht verfügbar sind. Mithilfe dieser Aktionen können Sie den Testversand genauer ändern oder konfigurieren, als in der Workfront-API verfügbar ist.

Einen Überblick über die ProofHQ-API finden Sie in der [Übersicht über POOFHQ](../../proofhq-api/general/overview.md) . Weitere Informationen finden Sie in der Dokumentation zu [ProofHQ](https://api.proofhq.com/home.html) .

>[!NOTE]
>
>* Die Workfront-API ist eine REST-fähige API. Die ProofHQ-API ist eine SOAP API.
>* In der ProofHQ-API erstellte Testsendungen werden nicht automatisch mit Workfront verknüpft. Es wird daher empfohlen, in der Workfront-API Testsendungen zu erstellen, bevor diese mit der ProofHQ-API aktualisiert werden.
>

### Erstellen eines Testversands mit erweiterten Testversandoptionen

1. Erstellen Sie einen Testversand mithilfe der Aktion `Document createProof` in der Workfront-API.

   >[!NOTE]
   >
   >Legen Sie beim Erstellen des Testversands `{}` als Wert für den Parameter `advancedProofingOptions` fest.

1. Verwenden Sie nach der Erstellung des Testversands die ProofHQ-API, um alle erweiterten Optionen hinzuzufügen.

### Beispiele

Dieser Abschnitt enthält einige Beispielaktualisierungen, die Sie mit der ProofHQ-API vornehmen können.

**Beispiele:**

* [Ein Testversand kann heruntergeladen werden, hat eine Nachricht und wird öffentlich freigegeben](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [Aktualisieren Sie eine Phase, sodass sie nicht privat, nicht obligatorisch ist und nur eine Genehmigung erfordert](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [Hinzufügen von zwei Empfängern zu einem Testversand ohne Entscheidungsträger](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**Ein Testversand kann heruntergeladen werden, hat eine Nachricht und wird öffentlich freigegeben**

Die Dokumentation für diesen Endpunkt finden Sie auf der Seite [ProofHQ API updateProof](https://api.proofhq.com/home/proofs/updateproof.html) .

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

**Aktualisieren Sie eine Phase, sodass sie nicht privat, nicht obligatorisch ist und nur eine Genehmigung erfordert**

Die Dokumentation für diesen Endpunkt finden Sie auf der Seite [ProofHQ API updateWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html) .

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

**Fügen Sie zwei Empfänger zu einem Testversand ohne primären Entscheidungsträger hinzu**

Die Dokumentation für diesen Endpunkt finden Sie auf der Seite [ProofHQ API addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html) .

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

## Erstellen eines Testversands mit JSON in der Workfront-API

In diesem Abschnitt wird beschrieben, wie Sie einen Testversand mit erweiterten Testversandoptionen über die Workfront-API erstellen und JSON als Parameterwert in der Workfront-API verwenden.

### Erstellen eines Testversands mit erweiterten Testversandoptionen

Sie können Testsendungen über die Workfront-API mit der Aktion `Document createProof` erstellen. Diese Aktion akzeptiert den Parameter `advancedProofingOptions` , der den Werttyp `string` aufweist. Um erweiterte Testversandoptionen in Ihre `createProof` -Aktion aufzunehmen, müssen Sie die Optionen im Parameter `advancedProofingOptions` im JSON-Format eingeben.

>[!NOTE]
>
>Es kann schwierig sein, die Felder vorherzusagen, die in Ihre JSON für advancedProofingOptions einbezogen werden sollen. Möglicherweise möchten Sie die Netzwerkdaten Ihres Unternehmens untersuchen, während Sie erweiterte Testsendungen in Workfront verwenden, und Ihre JSON auf den Feldern und Werten basieren, die üblicherweise von Ihrem Unternehmen verwendet werden.
>
>Da diese Felder schwer vorherzusagen sind, empfehlen wir, einen Testversand mithilfe der Workfront-API zu erstellen und ihn dann mithilfe der ProofHQ-API zu aktualisieren. Weitere Informationen finden Sie unter [Erstellen eines Testversands mit den Workfront- und ProofHQ-APIs (empfohlen)](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) in diesem Artikel

### Beispiel

Dieses Beispiel zeigt Felder und Formatierungen, die Sie beim Erstellen Ihrer JSON-Datei für den Parameter `advancedProofingOptions` verwenden können. Ihre JSON-Datei `advancedProofingOptions` kann mehr oder weniger Felder als hier angezeigt haben.

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
