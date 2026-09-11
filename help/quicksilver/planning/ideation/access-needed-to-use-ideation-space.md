---
title: Zugriff für die Verwendung des Ideenraums erforderlich
description: Adobe Workfront Planning bietet jetzt eine zusätzliche Funktion, mit der Sie Ideen ausarbeiten können, bevor Sie Ihre Kampagnen starten. Nutzen Sie die Leistungsfähigkeit von KI, um Daten umzuwandeln und Eingaben in greifbare Pläne zu lenken und Teams einen fundierten Ausgangspunkt anstelle einer leeren Seite mit Adobe Ideation-Raum zu bieten.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 1%

---


# Zugriff für die Nutzung des Ideenraums erforderlich

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Es ist nur im Rahmen des Programms **Ideation Space Beta** verfügbar. </span>

<span class="preview">Weitere Informationen finden Sie unter [Erste Schritte mit dem Ideenraum für Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>


{{planning-important-intro}}

Adobe Workfront Planning bietet jetzt eine zusätzliche Funktion, mit der Sie Ideen ausarbeiten können, bevor Sie Ihre Kampagnen starten. Nutzen Sie die Leistungsfähigkeit von KI, um Daten umzuwandeln und Eingaben in greifbare Pläne zu lenken und Teams einen fundierten Ausgangspunkt anstelle einer leeren Seite mit Adobe Ideation-Raum zu bieten.

In diesem Artikel werden die Zugriffsberechtigungen beschrieben, die Sie für den Zugriff auf den Ideationsbereich von Workfront Planning benötigen.

Allgemeine Informationen zum Ideation-Bereich finden Sie unter [Erste Schritte mit dem Ideation-Bereich für Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).

## Produktanforderungen

Der Ideation-Bereich ist kein eigenständiges Produkt. Dazu ist ein Workfront Planning-Paket erforderlich, auf das nur über Workfront Planning zugegriffen werden kann. Außerdem sind zusätzliche Produkte erforderlich.

Ihr Unternehmen muss ein Paket für die folgenden Produkte erwerben, um auf den Ideationsbereich zugreifen zu können:

* Ein Adobe Workfront-Workflow-Paket zusätzlich zu einem Planungspaket

  ODER

  Ein Adobe Workfront Planning-Produkt, das als eigenständiges Produkt erworben wurde.
* Eine Adobe GenStudio for Performance Marketing-Lizenz

  >[!TIP]
  >
  >GenStudio for Performance Marketing ist erforderlich, um Zugriff auf die richtigen Schriftartenberechtigungen zu erhalten.


<!--only required for closed beta:* An Adobe Customer Journey Analytics license that includes campaign tracking-->

## Workfront Planning - Anforderungen an die Zugriffsebene

Der Zugriff auf Ideationsbereiche wird in Workfront konfiguriert.

Ihre Workfront-Zugriffsebene muss Folgendes enthalten, um auf den Ideation-Bereich zuzugreifen:

* Eine Standard-Workflow-Lizenz, wenn Ihr Unternehmen ein Workflow-Paket zusätzlich zu einem Planungspaket erworben hat.
* Eine Standard Planning-Lizenz, wenn Ihr Unternehmen mit einem Workflow- und einem Planning-Paket gekauft hat, oder eine Workfront Planning als eigenständiges Produkt.
* Die Einstellung Ideenraum deaktivieren im Abschnitt Zusätzliche Einschränkung festlegen Ihrer Zugriffsebene muss deaktiviert sein. <!--***********check the UI for this***********-->

## Anforderungen an Workfront-Planungsberechtigungen

Jeder Planungsdatensatz ist im Ideationsraum mit einer Zusammenfassung verbunden.

Die Berechtigungen für die Ideationsspeicherübersicht werden von den Berechtigungen für Workfront-Planungsdatensätze übernommen. <!--not sure if this is right, because now you can share the ideation with others??-->

Sie müssen über Verwaltungsberechtigungen für einen Datensatztyp in Planning verfügen, um Datensätze zu erstellen, um einen Datensatz im Ideenbereich zu erstellen oder zu bearbeiten.

Planende Benutzer mit Ansichtsberechtigungen für Datensätze können den Ideenraum eines Datensatzes anzeigen.

Die folgende Tabelle zeigt die Verbindung zwischen den Berechtigungen für Workfront Planning-Datensätze und den kurzen Ideation Space-Berechtigungen:

| Berechtigung auf Datensatzebene planen | Berechtigungen auf kurzer Ebene zu Ideenraum |
|---|---|
| Verwalten der Berechtigungen für einen Datensatz | Kann eine Zusammenfassung im Ideenbereich des Datensatzes erstellen |
| Anzeigen der Berechtigungen für einen Datensatz | Kann die Zusammenfassung dieses Datensatzes im Ideenraum lesen, ihn jedoch nicht ändern |

## Ideenraum-Berechtigungen

<!--this is also duplicated in the intro of the Share an ideation space article-->

Planungsberechtigungen werden in den Ideenraum eines Datensatzes übertragen.

Darüber hinaus können Sie anderen Benutzern die Berechtigung erteilen, den Ideenraum zu verwenden und ihm Ideen hinzuzufügen.

Beachten Sie Folgendes:

* Die Ersteller von Ideen haben immer Editor-Berechtigungen für ihre eigenen Ideen.

* Sie müssen über Editor-Berechtigungen für einen Ideenraum verfügen, um Briefs zu erstellen und sie in andere Programme zu exportieren.

Im Folgenden finden Sie Ideenraum-Berechtigungen und die Funktionen, die sie bieten:

| Ideationsraum-Berechtigung | Funktionen |
|---|---|
| Bearbeiterin bzw. Bearbeiter | Kann den Ideenraum bearbeiten, herunterladen und freigeben |
| Kommentator | Kann den Ideenraum anzeigen und kommentieren |
| Viewer | Kann den Ideenraum anzeigen |

Weitere Informationen zum Freigeben eines Ideenraums finden Sie unter [Freigeben eines Ideenraums](/help/quicksilver/planning/ideation/share-the-ideation-space.md).

<!--there is no additional setup for Workfront layout template assignment because Contributors an below cannot access Ideation space; only Standard users-->


<!-- 
Not sure if this is needed. Maybe all orgs have IMS for all Adobe?? - asking Becky: 

## Org/IMS-level entitlements

Beyond Planning access itself, a customer's IMS Org needs specific entitlements for the full Ideation space experience to work:

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | Missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform / document storage entitlement | Entitlement | Existing documentation indicates users may be able to reach ideation entry points but fail during actual usage if storage-related entitlements are missing |

Historically, some customer teams relied on GenStudio (GenS) provisioning without realizing they could use the Ideation space directly — provisioning conversations should confirm both Planning and GenStudio PEM entitlements are explicitly set up for the Ideation space, not just assumed via GenS.
-->



<!--
From Claude: Internal information, not customer-facing: 

The permissions and entitlement model below reflects what was documented and confirmed as of the Closed Beta (through Aug 2026). Internal teams were still finalizing a formal access-model document and access-level definitions at this time, so treat this as the current best understanding rather than a final spec — confirm against the latest internal documentation before publishing externally.

## Practical checklist for provisioning a customer

1. Confirm the customer has Workfront Planning (via Workflow+Planning or Planning standalone).
2. Confirm the customer's IMS Org has GenStudio PEM entitlements provisioned (not just assumed).
3. Confirm font and document-storage entitlements are active — test actual usage, not just entry-point visibility.
4. Confirm the "strategic ideation" product is enabled at the org level.
5. During Closed Beta, confirm the user-level feature flag is set for named ideation users.
6. Confirm the target users have **create** (not just view) access to the records they need to ideate on.
7. If the Coworker integration inside the Ideation space is in scope, verify its availability separately.

## Packaging

| Detail | Description |
|---|---|
| Included with Workfront Planning | Yes |
| Standalone option | Can also be launched as its own surface |
| Agent platform | Runs within the Adobe Agent Orchestrator |
| Billing | Monetized through Adobe's AI-credits framework |
-->

<!--

Original Claude write-up, in addition to the info above:

## Baseline product requirement

The Ideation space isn't a standalone purchase — you need **Workfront Planning** to access it, through either:

- Adobe Workfront Workflow with a Workfront Planning package, or
- Adobe Workfront Planning as a standalone product

If your org has Workfront Planning, it has the Ideation space too. The Ideation space can't exist without Planning.

For the Closed Beta and Open Beta, the Ideation space is available only to Planning and GenStudio (GenS) customers.

## Customer-level entry requirements (Closed Beta)

To participate in the Closed Beta, customers needed to meet these criteria:

- An active Adobe Customer Journey Analytics (CJA) deployment with campaign tracking in place
- Multi-channel campaigns with a repeatable planning process
- Active use of Workfront Planning for marketing operations
- At least one identified strategist or ideation user who will be the primary Ideation space user

## Org- and user-level enablement

- Workfront surfaces the Ideation space integration to users only after a Workfront administrator enables the **strategic ideation** product at the org level.
- During the Closed Beta, a user-level feature flag also controls access, so org-level enablement alone isn't enough.
- For Open Beta, access is expected to move to an opt-in model, where customers actively configure themselves in, rather than opt-out.

## Record-level permissions

Your Ideation space permissions come from your Workfront Planning record permissions — there's no separate permission system layered on top:

- If you can create a record in Planning, you can also create a canvas in the Ideation space. Any Planning license is sufficient for this.
- If you have read-only access to a record, you have read-only access to the canvas connected to that record.
- If you only have view access to an existing record, you can't open the Ideation space from it. Workfront shows an "Insufficient permissions" message instead.
- Each canvas is related to exactly one record.

>[!NOTE]
>As of August 2026, the team was still defining discrete access levels for the Ideation space. These are expected to include, at minimum, Can read, Can view, and Can create.

## Org and IMS-level entitlements

Beyond Planning access, your organization's IMS Org needs specific entitlements for the Ideation space to work fully.

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | A missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform or document storage entitlement | Entitlement | Users may be able to reach Ideation space entry points but fail during actual use if storage-related entitlements are missing |

>[!IMPORTANT]
>When you provision a customer, confirm that both the Planning and GenStudio PEM entitlements are set up specifically for the Ideation space. Don't assume that GenStudio (GenS) provisioning alone includes Ideation space access.

## Content-sharing and abuse controls

Because the Ideation space lets you create content and share it with other users through Adobe systems, a **Report Abuse** capability is planned as a requirement before General Availability (GA). Workfront needs this roughly one month ahead of GA to support Adobe's platform license agreement process. This capability may reuse the existing Report Abuse functionality from Adobe Horizon rather than being built from scratch.

## Coworker (conversational AI) access

Access to the **Coworker** integration inside the Ideation space, the conversational right-rail assistant, is being rolled out separately from core Ideation space and Planning access:

- As of mid-August 2026, Coworker access wasn't yet generally available for customer testing.
- By August 17, 2026, Coworker was available inside the Ideation space for internal use, but still being refined.
- If you're documenting or testing the Coworker integration inside the Ideation space specifically, verify current availability separately. Don't assume it's included automatically with standard Planning or Ideation space provisioning.

For more information, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

-->
