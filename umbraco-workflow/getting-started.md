# Getting Started

In this article, you can read about [Umbraco Workflow](https://umbraco.com/products/umbraco-workflow/) and how to get started.

## Umbraco Workflow Overview

Umbraco Workflow allows the creation of multi-stage approval workflows when writing and publishing content. Umbraco Workflow extends Umbraco's out-of-the-box publishing model with multi-stage and configurable approval workflows. A workflow process comprises of multiple steps and multiple users assigned to the group responsible for providing approval at each step.

Umbraco Workflow adds a [Content App](../umbraco-cms/extending/content-apps.md) to all content nodes in the **Content** section where a workflow is enabled. For more information, see the [Workflow Content App](#workflow-content-app) section.

A user can be a member of multiple groups in the same workflow. To initiate an approval workflow, a user updates the content, saves their changes, then selects **Request publish**.

The workflow Dashboard updates to reflect the state of each task, providing an overview of a user's submissions and tasks. Tasks can be approved, cancelled, or rejected from the **Dashboard** or from the content node **Workflow** tab. For more information, see the [Workflow Dashboards and Buttons](#workflow-dashboards-and-buttons) section.

## Video Tutorial

{% embed url="https://www.youtube.com/watch?ab_channel=UmbracoLearningBase&v=5M1CtFVZCBo" %}
Umbraco Workflow Overview
{% endembed %}

## Workflow Dashboards and Buttons

Umbraco Workflow has its default Dashboards. By default, when you install Umbraco Workflow, you receive two Dashboards: the *User Dashboard* and the *Admin Dashboard*. Additionally, Umbraco Workflow replaces the default Umbraco button set in the editor drawer.

### Dashboards

Umbraco Workflow adds two Dashboards to your Umbraco project:

- **User Dashboard** - This Workflow Dashboard is added in the **Content** section. It displays the tasks requiring approval from the user, current user’s submissions, and stale content.

  ![Workflow Dashboard in the Content Section](images/WorkflowDashboard_ContentSection.png)

- **Admin Dashboard** - This Workflow Dashboard is the default view in the **Workflow** section. It displays a chart of recent workflow activity and any relevant upgrade-related messages. You can also set the days to view the workflow activity chart for the specified range of days.

  ![Workflow Dashboard in the Workflow Section](images/WorkflowDashboard_WorkflowSection.png)

### Buttons

When a workflow is active on the current node, the **Publish** button is replaced, linking to the workflow content app.

![Disabled content edits](images/Buttons.png)

When no workflow is active, the button state is determined by the current user's permissions.

Umbraco Workflow overrides Umbraco's User/Group publishing permissions. If the user has permission to update the node, they will be able to initiate a workflow process on that node. Umbraco Workflow shifts Umbraco from a centrally administered publishing model (controlled by a site administrator) to a distributed model. In this model, editors publish content based on their responsibilities assigned during the workflows.

In cases, where the content is already in a workflow, a notification is displayed at the top of the editor. Depending on the Workflow **Settings**, you can enable/disable editing access on a content node in a workflow.

![Disabled content edits](images/blocked_content.png)

For nodes where the workflow has been disabled, the default Umbraco options are displayed.

![Default Button](images/Default_Buttons.png)

## Workflow Content App

Umbraco Workflow adds a [Content App](../umbraco-cms/extending/content-apps.md) to all content nodes in the **Content** section where a workflow is enabled. The Workflow content app includes three sub-sections:

- [Active workflow](#active-workflow)
- [Configuration](#configuration)
- [History](#history)

![Workflow content app](images/content-app.png)

### Active Workflow

The Active workflow sub-section provides an interface for managing workflows for the current content node. When you initiate a workflow on the current node, the **Active workflow** sub-section requires information such as:

- Change Description.
- [Optional] Scheduled date to publish the changes requested in the node.

![Active workflow initiate request](images/Active-workflow-initiate-request.png)

When the current node is pending workflow approval, the **Active workflow** sub-section displays detailed information such as:

- Option to [approve, reject, or cancel pending workflow tasks](#approve-reject-or-cancel-pending-workflow-tasks).
- View change description and track differences across pending and completed workflows.
- View the group responsible for approving the pending workflow.
- View pending language variant(s) workflow.
- View the workflow activity (eg. pending approval/task approvals/rejects) for the current workflow process.

![Active Workflow sub-section](images/Active_Workflow_detailed_info.png)

You can access Active Workflows from two places - the **Content** section and the **Workflow** section (depending on your user permission). Workflow Administrators (those users with access to the Workflow section) can access workflows assigned to a different group. In the **Workflow History**, these are noted as being performed by the admin.

In multi-lingual sites, variant content can be submitted in one of these workflows:

- Only the current variant.
- All variants for publishing in a single workflow process using the workflow applied to the default variant.
- Each variant into a separate workflow.

For example, the German version of your content can be approved by German speaker's group and the English version by the English speaker's group.

#### Approve, Reject, or Cancel pending workflow tasks

<TBD>

### Configuration

The Configuration sub-section provides an interface for configuring the content approval flow for the current node. It also displays any inherited or Document type approval flows applied to the current content node.

![Configuration sub-section](images/Configuration-sub-section.png)

#### Content Approval Flow

You can add different groups for different stages of content approval flow. Content Approval flow groups can be reordered via drag and drop. You can also apply the approval flow either for publish and unpublish workflow or only publish workflow.

![Content approval flow](images/content-approval-flow.gif)

#### Approval Flow Types

Approval Flows are available in three types: Content approval flow, Inherited approval flow, and Document type approval flow.

A given content node may have all three approval flow types applied but only one will be applied as per the following order of priority:

- **Content approval flow:** set directly on a content node via the **Configuration** section in the **Workflow** tab . This type will take priority over all others.
- **Document type approval flow:** set in the **Settings** section. This approval flow will apply to all content nodes of the selected Document Type unless the node has a Content approval flow set. This feature requires a license.
- **Inherited approval flow:** if a node has no Content approval flow set, nor a flow applied to its Document Type, Umbraco Workflow will traverse the content tree until it finds a node with a Content approval flow and will use this flow for the current change.

![Approval Flow Types](images/approval-flow-types.png)

Review the current responsibilities for Approval Groups in the **Roles** tab of the **Approval Groups** section for **Node-based approvals** and **Document type approvals** only. For more information see the [Roles](approval-groups.md#roles) section in the [Approval Groups](approval-groups.md) article.

![Approval Groups Roles](images/approval-groups-roles.png)

Document type approval flows can also include conditional stages i.e., only include **Translators** in the workflow when the **Description** property has changed. For more information on settings conditions in Document type approval flows, see the [Document type approval flows](workflow-settings.md#document-type-approval-flows) section in the [Workflow Settings](workflow-settings.md) article.

{% hint style="info" %}
Configuration cannot be modified when a content node is in a workflow process.
{% endhint %}

### History

The History sub-section provides a chronological audit trail of workflow activity for the current node. It displays a table containing the following information:

- Page name with the Language variant.
- Type of Publish.
- Who the workflow is requested by.
- The date the workflow was requested.
- Comments.
- Status of the workflow.

![History sub-section](images/History-sub-section.png)

You can also **Filter** the records based on the information listed above. Additionally, you can adjust the total number of records displayed on a page.

The **Detail** button at the end of the record displays an overlay with content similar to the Active workflow sub-section.

![Details overlay](images/Workflow-Content-app-Details-overlay.png)