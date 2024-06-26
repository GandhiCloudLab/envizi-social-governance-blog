# Creating Custom Envizi PowerBI Report for Social and Governance Metrics

In today's business world, Environmental, Social, and Governance (ESG) factors are more important than ever. While environmental and governance issues often get the most attention, the social aspect—which includes the human elements related to society, communities, and individuals—is just as important. Tracking and analyzing social metrics can give valuable insights into areas like employee engagement, human rights, health and safety, training programs, gender pay gaps, and diversity, equity, and inclusion.

IBM Envizi helps organizations capture these social and governance metrics. With Envizi, companies can collect data on important social aspects, such as employee onboarding and offboarding, and issues related to modern slavery. This data can be turned into detailed and useful Power BI reports, allowing organizations to make better decisions and create a more socially responsible and inclusive workplace.

In this article, let's look at how organizations can capture social metrics around employee onboarding and offboarding, as well as modern slavery-related aspects, and create Power BI reports from this data.

## Prerequisite

1. Envizi Instance access with `Account Style Wizard` Enabled and `PowerReport Edit` work role added.


## 1. Enable Social Metrics

To show the Social Metrics related data in the monthly data set of the Power BI report, you need to enable Social metrics in Organization Settings.

1. Enable Social metrics in Power BI Report in Organization Settings. This can be done by requesting the Product team.

<img src="images/image1.png">

## 2. Create Account Style

We need to create account styles for the Social metrics related data.

Lets create 2 account styles with the below information.

### Account Style 1 : Emp Hires

Lets create an account style called `Emp Hires`. 

This account style helps to keep the Employee Hires details of the organization. It contains information such as Gender, Qty (Total emp count), Agewise count, Joined, relieved and fired employee count details.

1. Goto `Admin > Account Style Wizard`

<img src="images/image20.png">

2. Create an account style with the following.

- **Scope :** Social Metrics
- **Data Type :** People - Headcount [Number]
- **Primary Column :** Qty
- **Secondary Columns :** Gender, Age-21-30,	Age-31-40,	Age-41-50,	Joining,	Leaving,	Fired

<img src="images/image21.png">
<img src="images/image22.png">


### Account Style 2 : Modern Slavery

Lets create an account style called `Modern Slavery`. 

This account style helps to keep the Modern Slavery details of the organization. It contains information such as Forced Labour, Child Labour, Others and Country details.

1. Create an account style with the following.

- **Scope :** Social Metrics
- **Data Type :** People - Headcount [Number]
- **Primary Column :** Forced Labour
- **Secondary Columns :** Forced Labour, Child Labour, Others and Country

2. You can create the required fields in the account style as like in the below picture.

<img src="images/image23.png">


## 3. Create Accounts

We need to create accounts with the above created Account Styles as like below.
<img src="images/image30.png">
<img src="images/image31.png">

1. Download the below sample files.

- [files/Envizi_SetupConfig_SG_Report.xlsx](./files/Envizi_SetupConfig_SG_Report.xlsx).
- [files/Account_Setup_and_Data_Load-G5-Hires.xlsx](./files/Account_Setup_and_Data_Load-G5-Hires.xlsx).
- [files/Account_Setup_and_Data_Load_G5-Slavery.xlsx](./files/Account_Setup_and_Data_Load_G5-Slavery.xlsx).

2. Make the required changes like Organization column and etc.

3. Upload the file by going to  `Manage > Data files > Upload files` screen.

<img src="images/image32.png">


## 4. Create Power Report

Once the account styles are created, wait for day for the daily refresh to happen. So that the newly created account styles will get reflected in the Monthly Data Set of the Power BI Report.

The account styles that we have created above would reflect like this in PowerReport after a day.

<img src="images/image40.png">


1. Create Social Metrics power report as like below.

<img src="images/image41.png">
<img src="images/image42.png">
<img src="images/image43.png">

You can refer this for detailed explanation of how to create Power Report in Envizi. https://github.com/GandhiCloudLab/envizi-create-custom-power-report


## Resources

1. PowerBI Training: https://yourlearning.ibm.com/activity/PLAN-8FF21DDE262D

2. Design effective reports in Power BI : https://learn.microsoft.com/en-us/collections/o4dhk4z8xpr8q

3. Monthly Dataset - Glossary - Basic Fields https://knowledgebase.envizi.com/home/monthly-dataset-glossary

4. Monthly Dataset - Glossary - Advanced Fields https://knowledgebase.envizi.com/home/monthly-dataset-glossary-advanced-fields

5. Monthly Dataset - Tutorials https://knowledgebase.envizi.com/home/monthly-dataset-tutorials


## Summary and next steps

In conclusion, IBM Envizi ESG Suite provides a comprehensive solution for creating custom power reports with the Social Metrics data of your organization.

For more information about IBM Envizi or to try it out yourself, start your 14-day IBM Envizi ESG Suite trial. You can also request a personalized IBM Envizi demo.