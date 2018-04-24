---
layout: default
title: DT Requisition Guide
permalink: /documentation/dtreqguide/
toc: true
---

# CREATING DT REQUISITIONS IN PEOPLESOFT #
April 4, 2018

## Introduction ##
After years of preparation, months of training, and even more months of delay, the City and County of San Francisco has taken the plunge: goodbye to the decrepit, mainframe world of FAMIS, and hello to the modern, web-based world of PeopleSoft to manage every transaction in the City’s $10 billion budget!

The [SF Employee Portal](https://sfemployeeportalsupport.sfgov.org/support/home) contains a wealth of training and job aides designed for the citywide audience of budget, accounting, and procurement teams. We have tested the [eProcurement: Create a Requisition job aide](https://sfemployeeportalsupport.sfgov.org/support/solutions/articles/22000209326-create-a-requisition), and it is technically accurate. It contains 97% of what you need to know to successfully create a requisition for the Department of Technology. This document will fill in that missing 3%, warn you of potential pitfalls, and stiffen your spine to jump into the future.

## Pep Talk and a Word of Caution ##
We all know that the PeopleSoft rollout remains a work in progress: errors in contract conversion are still being uncovered, most vendors still lack access, many budget codes are confusing or incorrect, individual role-mapping appears to be . . . creative? 
BUT, the PeopleSoft system is live, FAMIS is now frozen, and our ability to keep the lights and Internet on for the City depends on our ability to start flying this plane while the support team finishes building it.

![caution](/images/exclamation.png) The City made the decision to make this an open system. This essentially means that “trust is given, not earned.” We have visibility and access to budgets outside of DT’s. This, combined with the bugs in the system, mean it can be easy to accidentally misroute our requisitions, purchase orders, and contracts. **It’s not the end of the world if-and-when mistakes happen!** This guide will help you avoid some pitfalls, but there will undoubtedly be more pitfalls. That’s okay! If we can’t correct an errant requisition, we can always delete it and start over. Take a deep breath, pour another cup of coffee, and we’ll begin. 

## What You Need and Where to Get It ##
Before you login to the PeopleSoft system, we suggest you first take a few minutes to gather all of the information you will need. If your requisition has missing budget codes, you want to find out now before you invest the time to start entering all the information. Here is what you need to create a DT requisition:
*	[eProcurement: Create a Requisition job aide](https://sfemployeeportalsupport.sfgov.org/support/solutions/articles/22000209326-create-a-requisition)
*	This DT-specific supplemental guide
*	PeopleSoft budget codes for your requisition 

![caution](/images/exclamation.png) The PeopleSoft budget codes provide the key information to ensure that your requisition is attached to the correct portion of the budget and routed to the correct approval path.

### Determining PeopleSoft Budget Codes ###
There are two main sources for determining the new PeopleSoft budget codes for your requisition:
*	[ServiceNow Procurement Ticket](#servicenow-procurement-ticket)
*	[DT FY17-18 Budget Spreadsheet](#dt-fy17-18-budget-spreadsheet)

#### ServiceNow Procurement Ticket ####
To locate the PeopleSoft budget codes in a ServiceNow procurement ticket:
1.	Navigate to the ServiceNow procurement ticket for your requisition.
2.	Scroll down to **Procurement Information** section. By default, the **Budget Section** tab is displayed.
3.	Click on the **Funding Information** tab. There you will (hopefully) see the six PeopleSoft (PS) codes needed to define the requisition!
![SN funding information](/images/SN-funding.png)

#### [DT FY17-18 Budget Spreadsheet] ####
But what if you are working off an old ServiceNow procurement ticket (created before 6/1/17)? DT Budget staff are in the process of mapping PeopleSoft codes to DT Budget Line Items in the spreadsheet, [FY17-18_DT_Budget-ACTIVE.xls](https://sfgov1.sharepoint.com/sites/TIS/Finance/BudgetFinancial/SitePages/Home.aspx), which is posted on DT Budget’s SharePoint home page:
![SN funding information](/images/SP-budget-page.png)

In the spreadsheet, simply search for the DT Budget Line Item for your requisition and then scroll over to locate the PeopleSoft codes.
![SN funding information](/images/DT-budget-spreadsheet.png)

## DT-Specific Guidance for Creating Requisitions ##
The following sections provide additional information that is not covered by the [eProcurement: Create a Requisition job aid](https://sfemployeeportalsupport.sfgov.org/support/solutions/articles/22000209326-create-a-requisition):
* [Entering the Requisition Name](#Entering-the-Requisition-Name)
* [Entering Bulk Budget Codes](#Entering-Bulk-Budget-Codes)
* [Adding new Items to PeopleSoft](#Adding-new-Items-to-PeopleSoft)
* [Confirming and Troubleshooting the Approval Path](#Confirming-and-Troubleshooting-the-Approval-Path)
* [Troubleshooting Incorrect Approval Paths](#Troubleshooting-Incorrect-Approval-Paths)

### Entering the Requisition Name ###
DT has adopted the following naming convention for requisitions to ensure consistency and make the best use of the 30-character limit:
**DT** *ServiceNow-ticket-number brief-description* 

The following screenshot shows the requisition name for ServiceNow ticket 0102084, which is for the renewal of LinkedIn corporate recruiting seats. 
 ![SN funding information](/images/PS-RQ-name.png)
 
We know the 30-character limit for names is arbitrary and annoying. Until this is fixed, we will just need to get creative with our abbreviations.  ¯\_(ツ)_/¯
### Entering Bulk Budget Codes ###
We can now enter the PeopleSoft budget codes once and apply them to all items in the requisition! We no longer need to re-enter them for every. single. item. 
To enter bulk budget codes, perform the following steps:
1.	From the “Requisition” page (Main Menu>eProcurement>Requisition), click **Requisition Settings**.
2.	In the “Requisition Settings” page, scroll down to the “Accounting Defaults” section.
3.	Enter the values for the PeopleSoft budget codes in the Account, Fund, Dept, Authority, Project, and Activity Code fields.
    ![budget chartfields](/images/PS-RQ-chartfields.png)
    
    ![caution](/images/exclamation.png) The PeopleSoft system will allow you to enter invalid budget codes. To avoid this error, pause for a second after entering each code and doublecheck that the PeopleSoft auto-complete function displays the correct code number and description.
4.	Click **OK**. The budget codes will be applied to all line items in the requisition!

### Adding new Items to PeopleSoft ### 
If any items in your requisition are not yet in the PeopleSoft database, you can now manually add them, by performing the following steps:
1.	From the “Requisition” page (Main Menu>eProcurement>Requisition), click **Add More Items**.
2.	Click **Special Requests** to display the “Special Requests” window.
![RQ Special Requests](/images/PS-RQ-special-requests.png)

3.	Enter values for the following fields:
	1.	Item Description
	2.	Price
	3.	Quantity
	4.	Unit of Measure 
	5.	Category
	6.	Supplier ID   

![caution](/images/exclamation.png) Note that the values for **Category** and **Supplier ID** are limited to values that are configured in the PeopleSoft database. If you don’t have these values, click the magnifying glass to search. The **Supplier Name** value auto-populates when you enter the **Supplier ID**.

### Confirming the Approval Path ###
We know that of all the issues with PeopleSoft, the requisition approval process has created the most consternation and gnashing of teeth. We have escalated these issues, and the Controller assures us they are working on it. BUT, until they do, we can still solve many of the common issues we’ve been encountering. Take a deep breath, and let’s proceed.
Once you have fully entered your requisition, perform the following steps to determine if the approval path is correct. 

1.	Once you’ve completed entering your requisition, click the **Preview Approvals** button.
2.	Under the FSP Requisition Approval section, you should see boxes for two approvers: “Requisition A1 Approver” and “Requisition A2 Approver.” If you see more or less than two approvers, something has gone awry. Proceed to [Troubleshooting the Approval Path](#troubleshooting-the-approval-path).
![RQ Special Requests](/images/PS-RQ-preview-approvals.png)
 
3.	Click on the **Multiple Approvers** link above “Requisition A1 Approver” and search for your manager’s name in the pop-up window that displays. If you do not find your manager’s name, proceed to [Troubleshooting the Approval Path](#troubleshooting-the-approval-path)..
4.	Click on the **Multiple Approvers** link above “Requisition A2 Approver” and search for your OCA liaison’s name in the pop-up window that displays. If you do not find your OCA liaison’s name, proceed to Troubleshooting the Approval Path.
    
    ![caution](/images/exclamation.png) There will likely be many unfamiliar and strange names listed in both lists of approvals. Some of this is intentional, some of this is unintentional. The Controller’s office is aware of this and working to fix it. But do not fear. These strange names will not adversely affect your requisition.
5.	If both your manager and OCA liaison are listed in the approval path, you have succeeded! Click the **Return** button to return to the “Requisitions” page and click **Submit for Approval**. Take a moment to bask in the well-deserved sense of accomplishment.

### Troubleshooting Incorrect Approval Paths ###
We have identified the following issues that can cause incorrect approval paths for requisitions. We will update this document as additional issues and solutions are found, so check back early and often.
