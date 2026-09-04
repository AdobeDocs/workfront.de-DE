---
title: Konfigurieren von Geschäftsregeln für Datensatztypen
description: Sie können Geschäftsregeln für den Datensatztyp konfigurieren, mit denen bestimmte Aktionen für Datensätze entsprechend den Feldwerten erzwungen werden können.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: cafe52c228520becb66e2fa9d8121127223a8f71
workflow-type: tm+mt
source-wordcount: '1094'
ht-degree: 2%

---


# Konfigurieren von Geschäftsregeln für Datensatztypen

{{planning-important-intro}}

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach der Veröffentlichung in der Vorschau sind dieselben Funktionen auch monatlich in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Sie können Geschäftsregeln für Adobe Workfront Planning-Datensatztypen konfigurieren, um anzugeben, dass bestimmte Felder erforderlich sind, bevor eine Aktion für einen Datensatz dieses Typs zulässig oder verhindert wird.

Je nach Formulierung der Regel können Sie die folgenden Aktionen für die Datensätze zulassen, wenn die definierten Geschäftsregeln erfüllt sind:

* Datensatz bearbeiten oder nicht bearbeiten
* Löschen oder Löschen eines Datensatzes nicht

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen, um die Schritte in diesem Artikel auszuführen:  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<ul> 
<li><p>Beliebige Workfront oder Workflows mit einem Planungspaket</p></li>
ODER
<li><p>Jedes Planungspaket, wenn es als eigenständiges Produkt gekauft wird</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Workflow-Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning-Lizenz</p></td> 
   <td><p>Planungsstandard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Sie müssen der Zugriffsebene sowohl einen Workflow- als auch einen Planning-Lizenztyp hinzufügen, wenn Sie sowohl einen Workflow als auch ein Planning-Paket haben</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich und einen Datensatztyp</p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen beim Konfigurieren von Geschäftsregeln

* Geschäftsregeln fügen einer Feldänderung oder einer Datensatzlöschung eine Bedingung hinzu. Die Regel kommt nur zu einem bestimmten, beabsichtigten Zeitpunkt ins Spiel: wenn ein Feld dabei ist, zu einem in der Regel konfigurierten Feldwert zu wechseln.

* Eine Regel sieht in einfacher Sprache wie folgt aus: „Bevor Sie diesen Datensatz bearbeiten können, muss das Feld Kampagnenzusammenfassung einen Wert enthalten“.

  Wenn das Feld leer ist, wird die Datensatzbearbeitung blockiert und der/die Benutzende erhält eine klare Nachricht, in der erklärt wird, was er/sie ansprechen muss, bevor er/sie fortfährt. Sobald sie das erforderliche Feld aktualisieren und erneut versuchen, ist die Änderung zulässig.

* Regeln blockieren nicht die Erstellung von Datensätzen. Benutzer können weiterhin Datensätze erstellen, müssen jedoch sicherstellen, dass die erforderlichen Felder nicht leer sind oder den angegebenen Wert enthalten.
* Regeln bearbeiten oder löschen Datensätze nicht automatisch. Die Änderung muss absichtlich erfolgen und von einem Benutzer ausgelöst werden.
* Regeln gelten nicht rückwirkend: alte Datensätze sind nicht betroffen. Die Regelprüfung wird nur ausgeführt, wenn das nächste Mal versucht wird, einen Datensatz zu bearbeiten oder zu löschen.
* Sie können keine Geschäftsregeln zu globalen Datensatztypen in ihren primären oder sekundären Arbeitsbereichen hinzufügen.
* Sie können eine Bedingung für Ihre Geschäftsregel erstellen, die auf alle Feldtypen mit Ausnahme der folgenden verweist:
  * Formelfelder
  * Suchfelder
  * Referenzfelder
* Regeln gelten für alle, die Datensätze bearbeiten oder löschen können.
* Sie können mehr als eine Geschäftsregel für einen Datensatztyp verwenden.  <!--Syuzanna is checking this because it should be just ONE rule per action: one per edit and one per delete - see this: https://workfront.slack.com/archives/C0BHWEUSJCU/p1788281638322049?thread_ts=1787924876.280359&cid=C0BHWEUSJCU; I also logged a bug for this because it released with more than one per action - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/6a99add600001e9aa90435ec181dec3e/overview-->

  Alle Regeln werden gleichzeitig überprüft. <!-- I have asked Syuzanna and Norayr multiple times HOW are the rules run/ prioritized and I got no answers; when I know, I will update here-->

## Geschäftsregeln konfigurieren

1. Zu einer Seite vom Typ Datensatz wechseln.
1. Klicken Sie in einer beliebigen Ansicht auf das **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und dann auf **Geschäftsregeln**.

   Die Seite mit der Tabelle „Geschäftsregeln“ wird geöffnet.
1. Klicken Sie **Neue Geschäftsregel**.
1. Fügen Sie **Regelfeld** Neues Unternehmen“ im ersten verfügbaren Feld einen Namen für die Geschäftsregel hinzu. Dies ist ein Pflichtfeld
1. (Optional) Fügen Sie eine Beschreibung hinzu, um die Geschäftsregel zu definieren, und klicken Sie dann auf **Speichern**.

   Das Einrichtungsformular für Geschäftsregeln wird geöffnet.

   ![Formular zur Einrichtung von Geschäftsregeln](assets/business-rule-setup-form.png)

1. Wählen Sie im Abschnitt **Wenn** des Einrichtungsformulars für Geschäftsregeln aus, welche Aktionen Sie auf der Grundlage einer bestimmten Regel einschränken oder zulassen möchten. Wählen Sie aus den folgenden Optionen: <!--check UI text-->
   * **Datensatzbearbeitung**: Benutzer dürfen den Datensatz bearbeiten oder nicht bearbeiten, wenn die in dieser Regel definierte Bedingung erfüllt ist.
   * **Löschen eines Datensatzes**: Benutzer können den Datensatz löschen oder nicht löschen, wenn die in dieser Regel definierte Bedingung erfüllt ist.
     <!--add screen shot when UI text is final-->
1. Fügen Sie **Feld „Formel** die Geschäftsregel hinzu. Wählen Sie einen Operator für Ihre Regel **Abschnitt &quot;**&quot; im rechten Bedienfeld aus.

   Sie können beispielsweise &quot;**&quot;** Abschnitt &quot;**Andere** auswählen oder mit der Eingabe von „IF“ beginnen und dann darauf klicken, wenn es in der Vorschlagsliste angezeigt wird.

   >[!TIP]
   >
   >Es wird empfohlen, die Felder und Operatoren aus der Vorschlagsliste auszuwählen, um die Syntax der Regel korrekt zu halten.
1. Wählen Sie und das Feld aus, das Sie als obligatorisch festlegen möchten, damit die Datensätze dieses Datensatztyps entweder bearbeitet oder gelöscht werden können.

   Sie können beispielsweise die folgende Anweisung eingeben, um das Feld **Kampagnenzusammenfassung** erforderlich zu machen:

   ```
      IF(ISBLANK({Campaign summary}),"Campaign summary is a required field. You cannot edit this record without a value for the Campaign summary field.")
   ```

   >[!IMPORTANT]
   >
   >Es wird dringend empfohlen, in die Regelformel die folgenden Informationen aufzunehmen, damit Benutzende leicht verstehen können, wenn eine Aktion, die sie für einen Datensatz ausführen möchten, nicht zulässig ist:
   >
   >* Die genauen Felder, für die die Regel eingerichtet ist.
   >* Die genaue Konsequenz, wenn die Regel nicht erfüllt ist.

   Das Feld **Formel** enthält Indikatoren, wenn ein Feld oder ein Ausdruck falsch ist.  <!--add screen shot?-->

   Im **Dann**-Abschnitt der Geschäftsregel können Sie eine Erläuterung der Funktionsweise der Regel anzeigen.

1. Klicken Sie **Aktivieren**, um die Regel für diesen Datensatztyp zu aktivieren, und klicken Sie dann auf **Speichern**.

   Regeln werden sofort nach ihrer Aktivierung angewendet und alle Benutzer, die zum Bearbeiten oder Löschen von Datensätzen im ausgewählten Datensatztyp berechtigt sind, müssen sie befolgen.
1. (Optional und empfohlen) Klicken Sie auf den Rückwärtspfeil links neben **Geschäftsregeln** in der Kopfzeile der Seite, um die Seite für den Datensatztyp anzuzeigen, und gehen Sie zu einer Tabellenansicht oder öffnen Sie die Seite eines Datensatzes. Versuchen Sie dann, einen Datensatz zu bearbeiten oder zu löschen, um die soeben erstellte Regel zu testen.

## Verwalten von Geschäftsregeln

Sie können bestehende Geschäftsregeln bearbeiten, löschen oder deaktivieren.

Bestehende Datensätze werden durch Bearbeiten einer vorhandenen Regel nicht geändert. Die bearbeitete Regel gilt nur für vorhandene Datensätze, wenn versucht wird, sie zu bearbeiten oder zu löschen.

1. Kehren Sie zur **„Geschäftsregeln** für den Datensatztyp zurück.
1. Suchen Sie die Regel, die Sie ändern möchten.
1. Bewegen Sie den Mauszeiger über den Regelnamen und klicken Sie dann auf das **Mehr** Menü ![Mehr](assets/more-menu.png) und dann auf eine der folgenden Optionen:

   * **Bearbeiten**: Dadurch wird die Seite zur Einrichtung der Geschäftsregel geöffnet, auf der Sie Informationen zur Geschäftsregel bearbeiten können.
   * **Deaktivieren**: <!--check this in the UI: right now, it says Disable--> Dies verhindert, dass die Regel ausgelöst wird, aber behält sie für die Zukunft bei, sofern erforderlich.
   * **Löschen**: Alle Informationen zur Regel werden gelöscht. Gelöschte Regeln können nicht wiederhergestellt werden.

   Die bearbeiteten Regeln oder die Deaktivierung von Regeln gelten nur für zukünftige Datensätze und werden nicht rückwirkend angewendet.

   <!--add NEW screen shot below if UI is fixed with Deactivate at release; it was fixed in devTest-->

   <!--![Business rule more menu expanded](assets/business-rule-more-menu-in-table-expanded.png)-->

<!--

***********FROM CLAUDE - BELOW - MUST EDIT*******************


### What business rules actually do

Business rules attach a condition to a **status change**. Instead of enforcing complete data the moment someone creates a record (which would slow everyone down), the rule only kicks in at one specific, deliberate moment: when a status is about to change to a status you've configured.

A rule looks like this in plain language:

> "Before a record can move to **Ready for Execution**, the field **Brand** must have a value."

If the field is empty, the status change is blocked and the person gets a clear message telling them what to fix. Once they fill it in and try again, the change goes through.

A few important things this is *not*:

* **It doesn't block record creation.** People can still create a new record instantly and fill it in over time, exactly like today. 
* **It doesn't auto-fill anything or auto-change statuses.** A person always has to make the status change themselves.
* **It doesn't retroactively flag old records.** Records that are already sitting in the target status aren't affected — the check only runs the next time someone tries to move a record *into* that status.

### Step 1: Open the business rules configuration area

Business rules live alongside your other admin setup — you won't need to hunt for a separate "Planning" panel. From your workflow setup area:

1. Go to the main **workflow setup / admin configuration** area for your workspace.
2. Look for the **business rules** section for the record type you want to configure (for example, "Materials" or "Campaigns").


### Step 2: Choose the record type

Rules are configured per record type, so pick the one you want to add a rule to. For example, if you want to make sure every Materials record has key fields filled in before execution, select **Materials**.

### Step 3: Create a new rule

For each rule, you'll specify three things:

| What you set | Example |
|---|---|
| **Record type** | Materials |
| **Target status** | Ready for Execution |
| **Required field** | Brand |

In other words: "When a Materials record's status is changed to **Ready for Execution**, the field **Brand** must have a value."

You can add more than one rule for the same status. For example, you might require Brand, Therapeutic Area, Indication, and Estimated Launch Date all to be filled in before a record can move to "Ready for Execution" — each is its own rule, and all of them are checked together.

**What fields can you require?**

* Connected record fields (e.g., a linked Brand or Indication record) — the rule passes as soon as at least one record is linked.
* Standard text fields (single-line or paragraph) — the rule passes once there's any value.
* Date fields — the rule passes once a date is set.

**What you can't use yet:** formula fields and lookup fields aren't supported as rule targets in this release, since they're calculated in the background rather than filled in directly by a person.

### Step 4: Write the message people will see

When you create a rule, you'll also provide the message that shows up if someone tries to make the change without the field filled in. Keep it specific and actionable — something like:

> "Brand is required."

You don't need to worry about formatting a whole error banner — the system handles combining messages if multiple rules are violated at once (see below).

### Step 5: Save the rule

Once saved, the rule takes effect **immediately** for everyone in the workspace — no need to log out, refresh, or wait for a deployment. The very next time anyone tries to move a record into that status, the rule is checked.

### What your team will actually experience

Here's what changes for the people using Planning day to day, once a rule is live.

#### If a required field is empty

1. A planner opens a record and changes the status to the gated status (say, "Ready for Execution").
2. The system checks all rules tied to that status.
3. If a required field is empty, the change is **rejected** — the status reverts back to what it was.
4. A toast message appears, naming exactly which field(s) are missing:
   > *"Status change blocked: 'Brand' and 'Estimated Launch Date' must be populated before moving to 'Ready for Execution.'"*
5. The planner fills in the missing field(s) and tries the status change again.
6. This time, the rule passes, and the status updates normally.

#### If everything is already filled in

Nothing changes. The status updates instantly, with no extra steps or popups. Business rules are invisible until they're actually needed.

#### If several fields are missing at once

All the violated rules are checked together, and the message lists every missing field in one go — planners don't have to fix one field, try again, get told about the next one, and repeat.

### Step 6: Edit or remove a rule later

Rules aren't set in stone. To make changes:

1. Go back to the business rules configuration area for the record type.
2. Find the rule you want to change.
3. Edit the required field, target status, or message — or delete the rule entirely.
4. Save. The change applies immediately to future status changes.

Keep in mind: editing or deleting a rule **only affects transitions going forward.** Records that already made it into the target status before the change aren't reevaluated.
3## A few things worth knowing

* **This is separate from locking records after a status change.** Business rules (as described here) only check field completeness *before* a status change goes through. A different, related feature governs whether a record becomes fully locked from edits/deletion once it reaches a certain status — that's not what's covered here.
* **Bulk status changes** (changing status on many records at once) aren't fully defined yet for how they interact with business rules — if your team relies heavily on bulk actions, check with your Adobe contact on current behavior.
* **If a rule can't be evaluated** due to a system error, the transition is blocked rather than silently allowed through — you'll never end up with an incomplete record slipping past a rule because of a backend hiccup.
* **Turning the feature off** doesn't delete your configured rules — they're just paused. Turning it back on restores them exactly as they were, no reconfiguration needed.

### Quick reference: setting up your first rule

1. Confirm the feature is enabled for your tenant.
2. Go to workflow setup → business rules for your record type.
3. Choose the record type (e.g., Materials).
4. Create a rule: target status + required field.
5. Write a clear, specific error message.
6. Save — it's live immediately.
7. Repeat for each field you want to require.
8. Test it yourself: try changing a record's status with the field empty, confirm you see the expected message, fill in the field, and confirm the status change now goes through.

That's it — from here on, anyone converting a record forward will get a clear nudge if something's missing, instead of a downstream project quietly showing up incomplete.

-->