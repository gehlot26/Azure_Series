# Day-03 : Resource, Resource Groups and Azure Resource Manager

## What is a Resource in Azure ?
- A resource is simply any servive we create or use in Azure. Eg:- Virtual Machine


## What is a Resource Group ?
- A Resource group is a logical container that holds related resources together.
- A Resource group helps us organize, manage and delete resources together.

Why Rsource Groups are useful:
- Organization:- keep project resources together.
- Easy Cleanup:- delete the resource group = delete everything inside it.
- Cost tracking:- see how much one project is costing us.
- Access control:- give/restrict access to group level.

Important rules:
- Every resource needs a group, we cannot create a resource without resource group.
- One resource = One group, a resource cannot be in two groups at once.
- Groups can't be nested, we cannot put a group inside a group.


## What is Azure Resource Manager (ARM) ?
- Azure Resource Manager is the backbone of Azure. It is the layer that handles everytihng we do in azure.
- Whenever we create, update or delete anything in azure whether through azure portal or azure cli, all of it goes through ARM first.
