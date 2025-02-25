# Install Azure CLI

### Installation Overview
https://learn.microsoft.com/en-us/cli/azure/install-azure-cli

### Install on Windows
https://learn.microsoft.com/en-us/cli/azure/install-azure-cli-windows?tabs=azure-cli

### Install on Linux
https://learn.microsoft.com/en-us/cli/azure/install-azure-cli-linux?pivots=apt

### Install on Mac
https://learn.microsoft.com/en-us/cli/azure/install-azure-cli-macos


Q: What is Azure CLI?

A: Azure CLI (Command-Line Interface) is a cross-platform command-line tool provided by Microsoft for managing Azure resources. It allows users to interact with Azure services and perform various administrative tasks through the command-line interface.

Q: How can I install Azure CLI?

A: Azure CLI can be installed on Windows, macOS, and Linux operating systems. Microsoft provides installation instructions on their official documentation website. The installation process typically involves downloading the appropriate package for your operating system and following the provided instructions.

Q: How can I authenticate Azure CLI to access my Azure subscription?

A: You can authenticate Azure CLI by running the 'az login' command. It will open a browser window, and after successful authentication, Azure CLI will have access to your Azure subscription. You only need to authenticate once, and Azure CLI will retain the access token for subsequent commands.

Q: Can Azure CLI be used to manage resources across different Azure subscriptions?

A: Yes, Azure CLI allows you to work with multiple subscriptions. You can use the 'az account set' command to switch between subscriptions and specify the active subscription for managing resources.

Q: Is there a way to get help on Azure CLI commands?

A: Yes, Azure CLI provides built-in help. You can use the '--help' option with any command to get detailed information about the command syntax, available parameters, and examples of usage.

Q: Can I use Azure CLI commands in scripts and automation?

A: Absolutely! Azure CLI commands are often used in scripts and automation workflows to manage Azure resources programmatically. You can create scripts in various scripting languages and incorporate Azure CLI commands to automate repetitive tasks and streamline resource management.


Fundamental/Beginner Level:

What is the Azure CLI and what is it used for?
(Expect: A command-line tool for managing Azure resources.)
How do you log in to Azure using the CLI?
(Expect: az login)
How do you list all your Azure subscriptions?
(Expect: az account list --output table)
How do you set a default Azure subscription?
(Expect: az account set --subscription <subscription_id_or_name>)
How do you create a resource group?
(Expect: az group create --name <resource_group_name> --location <location>)
How do you list all resources within a resource group?
(Expect: az resource list --resource-group <resource_group_name>)
What is the difference between --output json, --output table, and --output tsv?
(Expect: different formats to display the data, json for machine parsing, table for human readability, and tsv for scripting.)
How do you get help for a specific Azure CLI command?
(Expect: az <command> --help)
Intermediate Level:

How would you create a virtual machine using the Azure CLI?
(Expect: A multi-step process involving creating a resource group, virtual network, subnet, public IP, network security group, and then the VM itself. They should mention the az vm create command and its required parameters.)
How do you deploy an Azure App Service using the CLI?
(Expect: creation of a resource group, app service plan, and then the app service itself. They might also mention deploying code using az webapp deploy.)
How do you scale an Azure App Service using the CLI?
(Expect: using the az appservice plan update command to modify the SKU.)
How do you create and manage Azure Storage accounts using the CLI?
(Expect: creating storage accounts, containers, and uploading/downloading blobs using az storage account, az storage container, and az storage blob commands.)
How do you use variables and loops within Azure CLI scripts?
(Expect: Demonstrating basic scripting concepts, possibly using Bash or PowerShell syntax within the CLI.)
How do you query specific data from the output of an Azure CLI command using JMESPath?
(Expect: Demonstrating the use of the --query parameter with JMESPath expressions.)
How do you deploy an ARM template using Azure CLI?
(Expect: az deployment group create --resource-group <resource_group_name> --template-file <template_file_path>)
How would you secure the credentials used by the Azure CLI?
(Expect: Mentioning service principals, managed identities, and avoiding storing credentials in scripts.)
Advanced Level:

How would you automate the deployment of a complex Azure infrastructure using the Azure CLI?
(Expect: Discussing the use of scripting, ARM templates, and potentially Azure DevOps or other CI/CD tools.)
How do you implement role-based access control (RBAC) using the Azure CLI?
(Expect: Demonstrating the use of az role assignment commands to assign roles to users, groups, or service principals.)
How would you troubleshoot issues with Azure resources using the CLI?
(Expect: Using commands like az monitor log-analytics query, az vm show, and checking resource logs.)
How do you create and manage custom Azure CLI extensions?
(Expect: Understanding how to create and install custom extensions for extending the CLI's functionality.)
How do you create and manage Azure Policies using the Azure CLI?
(Expect: using commands such as az policy definition, az policy assignment.)
How would you create a pipeline that uses the Azure CLI to deploy an application to Azure?
(Expect: knowledge of how to use Azure devops or github actions in conjunction with the Azure CLI.)
Describe how to implement Infrastructure as Code (IaC) using Azure CLI and other tools.
(Expect: Discussion on the use of ARM templates, Bicep, and how the CLI interacts with these tools. Also, an understanding of version control.)
