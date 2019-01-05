---
title: Workspace Editor
---

# Workspace Editor

Workspace Editor allows to create/delete workspace. Workspace is always mapped with your environment. It's good to create two or more workspace for your Dev and Prod environment. Let's consider my organization name is **BlueLeaf**. It's good idea to create Workspace like `BlueLeafDev` and `BlueLeafProd`

## What workspace holds

Workspace holds all your page segment, engagement informations. Also workspace has it's own HBase table which will have all your engagement data. Workspace name should be unique across world.

## Create Workspace

1. Navigate to workspace editor https://analligence.nexttimespace.com/analligence/workspace
2. Click on **Create Workspace** button, you may see side bar asking for workspace name.
3. Provice a valid workspace name.
4. Workspace will be created all required backend configurations will be up and ready for workspace.
5. When you create workspace, you could be noticing the selected workspace appears on top. If you have multiple workspace, that's the way you could switch between workspaces.

 <img style="max-height: 20rem; padding: 1rem 5rem;" src="/docs/imgs/analligence_create_workspace.png">

## Delete workspace

Click on the delete icon on workspace editor to delete workspace.

_Note: All data will be deleted including customer engagement data, segments, configuration and everything mapped with the workspace. This action cannot be undone_

## Next Step

Creating Catalog is our next step. Check out [Catalog Editor](/docs/editors/catalog-editor)