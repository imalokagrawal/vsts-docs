---
title: Navigate within the Visual Studio Team Explorer pane
titleSuffix: VSTS & TFS 
description: Download TFS clients, navigate in Team Explorer for Visual Studio Team Services & Team Foundation Server 
keywords: Download TFS clients 
ms.technology: devops-new-user
ms.prod: devops
ms.assetid: fd7a5cf7-7916-4fa0-b5e6-5a83cf377a02
ms.manager: douge
ms.author: kaelli
author: KathrynEE
ms.topic: reference
ms.date: 09/07/2017
monikerRange: '>= tfs-2013'
---


# Navigate in Team Explorer

[!INCLUDE [temp](../_shared/version-vsts-tfs-all-versions.md)]

You use Team Explorer to manage work that is assigned to you, your team, or your team projects, and to coordinate your efforts with other team members to develop a project. Team Explorer is a plug-in that installs with Visual Studio or Eclipse. Working from different platforms, developers and stakeholders can effectively collaborate using Team Explorer connected to team projects hosted on Visual Studio Online or on-premises Team Foundation Server (TFS). 


>[!TIP]  
>You can access the latest version of Visual Studio clients from the [Visual Studio Downloads page](https://visualstudio.microsoft.com/downloads/). Additional options for connecting to VSTS or TFS include:

> - [Team Explorer Everywhere](/../java/download-eclipse-plug-in.md)
> - [VSTS Plugin for Android Studio](/../java/download-android-studio-plug-in.md)  
> - [VSTS Plugin for IntelliJ](/../java/download-intellij-plug-in.md)
> - [Visual Studio Code](/../java/vscode-extension.md)
>For information about compatibility among client and server versions, see [Requirements and compatibility](/tfs/server/requirements).

The operations available to you depend on which source control option-Team Foundation version control (TFVC) or Git-was selected to manage source code when the team project was created.

**Team Explorer plug-in for Visual Studio**

Team Explorer connects Visual Studio to team projects. You can manage source code, work items, and builds. Or, create a team project.

>[!TIP]  
>If you open Visual Studio and the Team Explorer pane doesn't appear, click the **View/Team Explorer** menu option. 


> [!div class="mx-tdBreakAll"]  
> |Home page with Git  |Home page with TFVC  |
> |-------------|----------|
> |<img src="../organizations/projects/_img/te-home-page-git-repo.png" title="Team Explorer Home page with Git as source control" alt="Team Explorer Home page with Git as source control" />|<img src="../organizations/projects/_img/te-home-page-tfvc-repo.png" title="Team Explorer Home page w/ TFVC as source control" alt="Team Explorer Home page w/ TFVC as source control" />|


>[!NOTE]  
>Some pages, such as **Reports** and **Documents**, only appear when an on-premises TFS is configured with the required resources, such as SQL Server Reporting Services and SharePoint.

If you don't need Visual Studio, but do want to connect to VSTS or TFS or get one or more Team Foundation add-ins, you can install the free [Visual Studio Community](https://visualstudio.microsoft.com/downloads/download-visual-studio-vs).

**Team Explorer plug-in for Eclipse**

If you work in Eclipse or on a non-Windows platform, you can [install the Team Explorer plug-in for Eclipse](/../java/download-eclipse-plug-in#_install-the-tee-plugin-for-eclipse). Once installed, you can share your Eclipse projects by adding them to VSTS or TFS using [Git](../repos/git/share-your-code-in-git-eclipse.md) or [TFVC](../repos/tfvc/share-your-code-in-tfvc-eclipse.md).



> [!div class="mx-tdBreakAll"]  
> |Home page with Git (Eclipse) |Home page with TFVC (Eclipse) |
> |-------------|----------|
> |<img src="_img/work-team-explorer/IC774826.png" title="Home page w/ Git as source control - Eclipse" alt="Home page w/ Git as source control - Eclipse" /> |<img src="_img/work-team-explorer/IC774825.png" title="Home page w/ TFVC as source control - Eclipse" alt="Home page w/ TFVC as source control - Eclipse" /> |


> [!NOTE]  
> Some pages, such as **Reports** and **Documents**, only appear when TFS is configured with the required resources, such as SQL Server Reporting Services and SharePoint.


## Choose the page to access the task you want

Based on the page you select and the options configured for your team project.

### Connect page

From the **Connect** page, you can select the team projects you want to connect to and quickly switch context between team projects.

![Team Explorer, Connect](../organizations/projects/_img/te-connect-manage.png)

> [!div class="mx-tdBreakAll"]  
> |Git: Local Git repo |TFVC: Map workspace |
> |-------------|----------|
> |If you connect to a Git repo, you also can [create, add, or clone repositories](../repos/git/creatingrepo.md).<br/>![Team Explorer, Connect, local Git repo options](../organizations/projects/_img/te-connect-local-git-repos.png) |If you connect to a TFVC repo, you'll be prompted to [Configure your workspace (TFVC)](../pipelines/build/options.md) on first connect.<br/>![Team Explorer, Connect, configure TFVC workspace](../organizations/projects/_img/te-tfvc-configure-workspace.png)|



> [!IMPORTANT]  
> From the Visual Studio plug-in, you can [Create a team project](../organizations/projects/create-project.md). The ability to create team projects is not supported from the Eclipse plug-in. You can, however, create team projects from the web portal/collection administration context. 



### Home, Work, and Build pages 


> [!div class="mx-tdBreakAll"]  
> |Home|Work Items  |Build |
> |-------------|----------|----------|
> |-[Configure workspace](../repos/tfvc/share-your-code-in-tfvc-vs.md#configure-your-workspace)<br/>- Open [Web portal](../project/navigation/index.md)<br/>- Open [Task Board](../boards/sprints/task-board.md)<br/>- Open [Team Room](../notifications/collaborate-in-a-team-room.md) |- [Add work items](../boards/backlogs/add-work-items.md)<br/>- [Use the query editor to list and manage queries](../boards/queries/using-queries.md)<br/>- [Organize query folders and set query permissions](../boards/queries/set-query-permissions.md)<br/>- [Open query in Excel](../boards/backlogs/office/bulk-add-modify-work-items-excel.md)<br/>- [Open query in Project](../boards/backlogs/office/create-your-backlog-tasks-using-project.md)<br/>- [Email query results list using Outlook](../boards/queries/share-plans.md)<br/>- [Create reports from query in Excel](../report/excel/create-status-and-trend-excel-reports.md) (TFS only) |- [Create build pipelines](../pipelines/tasks/index.md)<br/>- [View and manage builds](../pipelines/overview.md)<br/>- [Manage the build queue](../pipelines/agents/pools-queues.md) |

> [!NOTE]  
> If inline images aren't displaying correctly, see [Resolve images that don't display in Team Explorer](#images-missing-te). 

### Git and TFVC pages  

The Git and TFVC repos support different pages and functions. You'll see one or the other pages depending on the team project and repro you connect to. For a comparison of the two repos, see [Choosing the right version control for your project](../repos/tfvc/comparison-git-tfvc.md). 


> [!div class="mx-tdBreakAll"]  
> |Git | TFVC  |
> |-------------|----------|
> |- **Changes**: [Save work with commits](../repos/git/commits.md)<br/>- **Branches**: [Create work in branches](../repos/git/branches.md)<br/>- **Pull Requests**: [Review code with pull requests](../repos/git/pullrequest.md)<br/>- **Sync**: [Update code with fetch and pull](../repos/git/pulling.md)) |- **My Work**: [Suspend/resume work](../repos/tfvc/suspend-your-work-manage-your-shelvesets.md)  &#124; [Code review](../repos/tfvc/day-life-alm-developer-suspend-work-fix-bug-conduct-code-review.md)<br/>- **Pending Changes**: [Manage pending changes](../repos/tfvc/develop-code-manage-pending-changes.md) &#124; [Find shelvesets](../repos/tfvc/suspend-your-work-manage-your-shelvesets.md) &#124; [Resolve conflicts](../repos/tfvc/resolve-team-foundation-version-control-conflicts.md)<br/>- **Source Control Explorer**: [Add/view files and folders](../repos/tfvc/add-files-server.md) |

### Report and Document pages (TFS only)

The **Report** page opens the [Reporting Services report site](../report/sql-reports/reporting-services-reports.md). This page appears only when your team project has been configured with SQL Server Analysis Services and Reporting Services. Also, the option to **Create Report in Microsoft Excel** appears only when reporting has been configured for the team project.

From the **Document** page, you can [open project portal](../report/sharepoint-dashboards/share-information-using-the-project-portal.md) and [manage documents and document libraries](../report/sharepoint-dashboards/manage-documents-and-document-libraries.md). This page appears only if your team project has been configured with a SharePoint Products portal.
  
If your team project is missing one or more pages, you may be able to [add functionality to your on premises TFS deployment](/tfs/server/admin/config-tfs-resources).

### Settings page 

From the **Settings** page, you can configure administrative features for either a team project or team project collection. Configuring features in these areas requires you to be a member of a VSTS or TFS administrator group.

Most of the links open to a web portal administration page. Not all settings are available from the Team Explorer plug-in for Eclipse. 
 

> [!div class="mx-tdBreakAll"]  
> |Team project settings | Collection settings (TFS)  |
> |-------------|----------|
> |Required membership: [Project Administrators](../organizations/security/set-project-collection-level-permissions.md?toc=/vsts/organizations/security/toc.json&bc=/vsts/organizations/security/breadcrumb/toc.json)<br/><br/>- [Security (manage project-level permissions)](../organizations/security/set-project-collection-level-permissions.md?toc=/vsts/organizations/security/toc.json&bc=/vsts/organizations/security/breadcrumb/toc.json)<br/>- [Group membership: manage group permissions](../organizations/security/set-project-collection-level-permissions.md?toc=/vsts/organizations/security/toc.json&bc=/vsts/organizations/security/breadcrumb/toc.json)<br/>- Source Control: Configure the [check-in and check-out policies](../repos/tfvc/add-check-policies.md) (TFVC)<br/>- [Work Item Areas (project-wide)](../organizations/settings/set-area-paths.md)<br/>- [Work Item Areas (project-wide)](../organizations/settings/set-iteration-paths-sprints.md)<br/>- [Portal Settings (Enable portal or process guidance)](../report/sharepoint-dashboards/configure-or-add-a-project-portal.md)<br/>-[Project Alerts](../boards/queries/alerts-and-notifications.md) |Required membership: [Project Collection Administrators](../organizations/security/set-project-collection-level-permissions.md)<br/><br/>- [Security (manage project-level permissions)](../organizations/security/permissions.md#collection-level)<br/>- [Group membership: manage group permissions](../organizations/security/permissions.md)<br/>- Source Control: Configure the [default workspace type for the collection](../repos/tfvc/decide-between-using-local-server-workspace.md#manage-project-collection-workspace-settings-for-your-team) (TFVC)<br/>- [Process Template Manager: download or upload a process template](../boards/work-items/guidance/manage-process-templates.md?toc=/vsts/reference/toc.json&bc=/vsts/reference/breadcrumb/toc.json) |

To learn more about administration features, see [About team, project, and organizational-level settings](../organizations/settings/about-settings.md).


## Related articles

You've now got a basic understanding of how to work in the Team Explorer add-in for Visual Studio and Eclipse.

- [Troubleshoot connection](troubleshoot-connection.md?toc=/vsts/user-guide/toc.json&bc=/vsts/user-guide/breadcrumb/toc.json)  

<a id="clients">  </a>

### Clients that connect to VSTS or TFS

In addition to connecting through Team Explorer, you can connect to a team project from these clients: 

- [Web portal](../project/navigation/index.md?toc=/vsts/user-guide/toc.json&bc=/vsts/user-guide/breadcrumb/toc.json) 
- [Visual Studio Code](https://code.visualstudio.com/docs)
- [Visual Studio Community](https://visualstudio.microsoft.com/products/visual-studio-community-vs.aspx) 
- [Eclipse: Team Explorer Everywhere](/../java/download-eclipse-plug-in.md) 
- [Office Excel](../boards/backlogs/office/bulk-add-modify-work-items-excel.md?toc=/vsts/boards/backlogs/toc.json&bc=/vsts/boards/backlogs/breadcrumb/toc.json)
- [Office Project](../boards/backlogs/office/create-your-backlog-tasks-using-project.md?toc=/vsts/boards/backlogs/toc.json&bc=/vsts/boards/backlogs/breadcrumb/toc.json)
- [PowerPoint Storyboarding](../boards/backlogs/office/storyboard-your-ideas-using-powerpoint.md?toc=/vsts/boards/backlogs/toc.json&bc=/vsts/boards/backlogs/breadcrumb/toc.json) 
- [Microsoft Test Manager](https://msdn.microsoft.com/library/jj635157.aspx)
- [Microsoft Feedback Client](../project/feedback/give-feedback.md?toc=/vsts/project/feedback/toc.json&bc=/vsts/project/feedback/breadcrumb/toc.json)   


### Refresh Team Explorer 

If data doesn't appear as expected, the first thing to try is to refresh your client. Refreshing your client updates the local cache with changes that were made in another client or in TFS. To refresh Team Explorer, do one of the following actions:

-   To refresh a page that you are currently viewing, choose ![Refresh icon](../boards/_img/icons/te-refresh-query-icon.png) **Refresh** icon in the menu bar (or choose the F5 key).

-   To refresh the team project you currently have selected, choose ![](_img/work-team-explorer/IC547418.png) **Home**, and then choose ![Refresh icon](../boards/_img/icons/te-refresh-query-icon.png) **Refresh** icon (or choose the F5 key).

-   To refresh the set of teams defined for the team project that you currently have selected, choose the Connect icon, and then choose ![Refresh icon](../boards/_img/icons/te-refresh-query-icon.png) **Refresh** icon (or choose the F5 key).


[!INCLUDE [temp](_shared/when-to-refresh-client.md)]

[!INCLUDE [temp](../_shared/images-not-appearing-vs.md)] 


### Additional tools provided with TFS Power Tools (Visual Studio 2015 & TFS 2015) 

By installing [TFS Power Tools](https://marketplace.visualstudio.com/items?itemName=TFSPowerToolsTeam.MicrosoftVisualStudioTeamFoundationServer2015Power), you gain access to these additional tools through the Team Explorer plug-in for Visual Studio:

-   Process Template Editor
-   Additional check-in policies for Team Foundation Version Control
-   Team Explorer enhancements including Team Members
-   Team Foundation Power Tool Command Line
-   Test Attachment Cleaner
-   Work Item Templates

Additional requirements may apply.

> [!NOTE]  
> For TFS 2017 and later versions, you can [install the TFS Process Template editor from the Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=KarthikBalasubramanianMSFT.TFSProcessTemplateEditor). You can use this version of the Process Editor to modify the old-style work item forms. You can't use it to edit forms associated with the [new web forms](../reference/process/new-work-item-experience.md?toc=/vsts/reference/toc.json&bc=/vsts/reference/breadcrumb/toc.json).  


