---
product-area: documents
navigation-topic: approvals
title: Überblick über den Entscheidungsstatus eines Dokuments
description: Der Status der Dokumentenentscheidung wird aufgelistet und erläutert
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 30a10ed9-ae11-4ff1-a66c-58ea94fe9959
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/VESaWT8Xq7iU85LiRJCAL-tldNpXtdLqlTFxSqpK3Ok
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 178
ht-degree: 10%

---

# Überblick über den Entscheidungsstatus eines Dokuments

Sie können den Status des Dokuments direkt in der Dokumentliste einsehen:

![Status in Dokumentliste](assets/status-in-doc-list.png)


Die folgenden Status sind verfügbar:

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                 <tr>
                    <td>
                        Überprüfung ausstehend</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                Prüfer und genehmigende Personen wurden benachrichtigt, haben das Asset jedoch noch nicht geöffnet.
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        Wird geprüft</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>Mindestens ein Reviewer hat das Asset angezeigt</p>
                            </li>
                            <li>
                                <p>Mindestens ein Reviewer hat die Überprüfung nicht abgeschlossen</p>
                            </li>
                            <li>
                                <p>Diesem Asset wurden keine genehmigenden Personen zugewiesen</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        Überprüft</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>Alle Reviewer haben ihre Überprüfung abgeschlossen</p>
                            </li>
                            <li>
                                <p>Diesem Asset wurden keine genehmigenden Personen zugewiesen</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>Muss bearbeitet werden</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>Alle Genehmigungen und Prüfungen sind abgeschlossen</p>
                            </li>
                            <li>
                                <p>Mindestens eine genehmigende Person hat eine Entscheidung mit dem Hinweis „Arbeit erforderlich“ getroffen</p>
                                <p>Andere genehmigende Personen haben möglicherweise Entscheidungen von „Genehmigt mit Änderungen“ oder „Genehmigt“ erteilt.
                            </li>
                        </ul>
                    </td>
                </tr>
                  <tr>
                    <td>Mit Änderungen genehmigt</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>Alle Genehmigungen und Prüfungen sind abgeschlossen</p>
                            </li>
                            <li>
                                <p>Mindestens eine genehmigende Person hat eine Entscheidung mit dem Status „Genehmigt mit Änderungen“ getroffen</p>
                                <p>Andere genehmigende Personen haben möglicherweise Entscheidungen vom Typ „Genehmigt“ getroffen.
                            </li>
                            <p>Hinweis: Diese Option steht nicht zur Verfügung, wenn Sie die Frame.io-Integration zur Überprüfung und Genehmigung verwenden.</p>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>Genehmigt</p>
                    </td>
                    <td>
                        <ul>
                           <!--
                           <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            -->
                            <li>
                                <p>Alle genehmigenden Personen haben möglicherweise Entscheidungen vom Typ „Genehmigt“ getroffen.
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>



<!--



<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                 <tr>
                    <td>
                        Pending review</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                Reviewers and approvers have been notified, but have not yet opened the asset.
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        In review</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>At least one reviewer or approver has viewed the asset</p>
                            </li>
                            <li>
                                <p>At least one reviewer has not completed their review</p><p>Or</p>
                                <p>At least one approver has not made an approval decision</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        Reviewed</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                All reviews are complete
                            </li>
                            <li>
                                There are no approvers
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>Needs work</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            <li>
                                <p>At least one approver has made a decision of "Needs work"</p>
                                <p>Other approvers may have given decisions of "Approved with changes" or "Approved"
                            </li>
                        </ul>
                    </td>
                </tr>
                  <tr>
                    <td>Approved with changes</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            <li>
                                <p>At least one approver has made a decision of "Approved with changes"</p>
                                <p>Other approvers may have given decisions of "Approved"
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>Approved</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            <li>
                                <p>All approvers may have given decisions of "Approved"
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>


-->
