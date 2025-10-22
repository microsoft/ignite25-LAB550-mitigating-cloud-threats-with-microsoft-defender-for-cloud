
# Exercise 1 - Enable Microsoft Defender for Cloud

## Lab scenario

You're a Security Operations Analyst working at a company that is implementing cloud workload protection with Microsoft Defender for Cloud. In this lab, you enable Microsoft Defender for Cloud.

### Task 1: Create a Log Analytics Workspace

In this task, you create a Log Analytics workspace for use with Azure Monitoring, Microsoft Sentinel and Microsoft Defender for Cloud.

1. In the Microsoft Edge browser, navigate to the Azure portal at https://portal.azure.com.

    >**Note:** Select the **Resourses** tab for the *Username* and *Password* for the lab. Use the **LabUser** account for this lab.

1. In the **Sign in** dialog box, copy, and paste in the tenant Email account for the admin username provided by your lab hosting provider and then select **Next**.

1. In the **Enter password** dialog box, copy, and paste in the admin's tenant password provided by your lab hosting provider and then select **Sign in**.

1. In the Search bar of the Azure portal, type Log Analytics workspaces, then select the same service name.

1. Select **+Create** from the command bar.

1. Select **Create new** for the Resource group.

1. Enter RG-Defender and select **Ok**.

1. For the Name, enter something unique like: lawIgniteLab.

1. Select **Review + Create**.

1. Once the workspace validation has passed, select **Create**. Wait for the new workspace to be provisioned, this may take a few minutes.

### Task 2: Enable Microsoft Defender for Cloud

In this task, you'll enable and configure Microsoft Defender for Cloud.

1. If you don't have the **Azure Portal** open from the previous task, open it now.

1. In the Search bar of the Microsoft Azure portal, type Defender, then select **Microsoft Defender for Cloud**.

1. In the left navigation menu for Microsoft Defender for Cloud, expand the **Management** section , and select **Environment settings**.

1. Select the **1 Azure Subscription** next to **Key** to open the subscriptions in Environment settings.

1. Scroll to the bottom of the page and find the **Azure** and **Tenant Root Group (1 of 1 subscriptions)**.

1. Start expanding each row until you get to the subscription.

1. Select your subscription from the tree.

1. When the new page opens, select the **Maybe later** for the **Auto-provisioning updated experience**.

1. Review the Azure resources that are now protected with the Defender for Cloud plans.

    >**Important:** If all Defender plans are *Off*, select **Enable all plans**. Select the *$200/month Microsoft Defender for APIs Plan 1* and then select **Save**. Select **Save** at the top of the page and wait for the *"Defender plans (for your) subscription were saved successfully!"* notifications to appear.

### I am skipping the Defender for API, to see if anythign fails.

1. Select the **Settings & monitoring** tab from the Settings area (next to Save).

1. Review the monitoring extensions. It includes configurations for Virtual Machines, Containers, and Storage Accounts. Close the "Settings & monitoring" page by selecting the 'X' on the upper right of the page.

1. Close the settings page by selecting the 'X' on the upper right of the page to go back to the **Environment settings** main page.

1. Scroll to the bottom of the page and expand the tree by selecting the **>** to the left of your subscription.

1. Select the Log analytics workspace you created earlier **uniquenameDefender** to review the available options and pricing.

1. Select **Enable all plans** (to the right of Select Defender plan).

1. Select **Save**. Wait for the *"Microsoft Defender plan for workspace uniquenameDefender were saved successfully!"* notification to appear.

    >**Note:** If the page is not being displayed, refresh your Edge browser and try again.

1. Close the Defender plans page by selecting the 'X' on the upper right of the page to go back to the **Environment settings**

### Task 3: Understanding the Microsoft Defender for Cloud Dashboard

1. In the Search bar of the Microsoft Azure portal, type *Defender*, then select **Microsoft Defender for Cloud**.

1. In the left navigation menu for Microsoft Defender for Cloud, under the *General* section, select **Overview**.

1. The Overview blade provides a unified view into the security posture and includes multiple independent cloud security pillars such as Security posture, Regulatory compliance, Workload protections, Firewall Manager, Inventory, and Information Protection. Each of these pillars also has its dedicated dashboard allowing deeper insights and actions around that vertical, providing easy access and better visibility for security professionals.

    >**Note:** The top menu bar allows you to view and filter subscriptions by selecting the Subscriptions button. In this lab, we will use only one but selecting different/additional subscriptions will adjust the interface to reflect the security posture of the selected subscriptions

    >**Note:** The high-level numbers at the top menu; This view allows you to see a summary of your subscriptions, active recommendations, and security alerts alongside connected cloud accounts.

1. Click on the **What’s new** item in the toolbar – a new tab opens with the latest release notes where you can stay current on the new features, bug fixes, and more.

1. Either close the **What's new** tab or switch back to the **Azure Portal** tab.

1. From the top menu bar, select **Azure subscriptions**. This will bring you into the environment settings where you can select from the available subscriptions.

1. Return to the **Overview** page, and review the **Security posture** tile. You can see your current **Secure score** along with the number of completed controls and recommendations. Selecting this tile will redirect you to a drill-down view across subscriptions.

    >**Note:** It will take around 2 minutes to load the security posture page.

1. On the **Regulatory compliance** tile, you can get insights into your compliance posture based on continuous assessment of both Azure and hybrid cloud environments. This tile shows the following standards which are Microsoft Cloud Security benchmark, and Lowest compliance regulatory standard. To view the data we first need to add Security policies.

1. Selecting this tile will redirect you to the **Regulatory compliance** dashboard – where you can add additional standards and explore the current ones

1. We will continue exploring *Microsoft Defender for Cloud* **Security posture** and **Regulatory compliance** in the next exercise.

## Proceed to Lab2
