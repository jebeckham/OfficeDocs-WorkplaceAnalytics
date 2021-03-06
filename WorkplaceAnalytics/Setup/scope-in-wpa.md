---
# Metadata Sample
# required metadata

ROBOTS: NOINDEX,NOFOLLOW
title: Scope in Workplace Analytics
description: Description of scopes plus how to use and set up scopes in Workplace Analytics 
author: paul9955
ms.author: v-pascha
ms.date: 05/23/2019
ms.topic: article
localization_priority: normal 
ms.prod: wpa
ms.collection: M365-analytics
manager: scott.ruble
audience: Admin
---

# Scope in Workplace Analytics

A scope is a data workspace for an analyst. A scope delimits the employee data and organizational attributes that an analyst can use for analysis. Companies define a scope with subset of employee data. To do this, they use various criteria. Here are examples:
 
 * **Organization:** a company can define a scope to be the data of all the employees in one division, or under a particular manager. Example: R & D
 * **Geography:** a multi-national corporation might create different scopes for the data of employees of different countries or parts of countries. Example: Wales 
 * **Role:** a company could select the data of all the employees who have a particular function to include in a scope. Example: Accounting personnel

## Scopes give access to data 

A scope defines what data you work with in Workplace Analytics. If you have one of the analyst roles (Analyst or Analyst Limited), you work with data on the **Explore** and **Queries** pages of Workplace Analytics. You are also assigned one or more scopes, and your scope determines whose data you work with on those pages. If you have the program manager (PM) role, you work on the **Solution** page and your role is not scoped, so you have access to all programs. 

For example, if you are an analyst with the job of finding workplace trends in the sales organization, you must be assigned a scope that encompasses the data of salespeople. You can then view data about salespeople on the **Explore** pages and create queries about salespeople on the **Queries** page. 

## The Global scope

One particular scope encompasses everyone’s data: the "Global" scope. If an analyst has this scope, they can work with all employee data that’s been uploaded to Workplace Analytics. The Global scope is created by the system. While it exists by default, no analysts are given access to it by default. Admins must grant access expressly. 

> [!Note] 
> For existing users, as part of one-time migration in 2019, all existing analysts and their existing queries and settings are being moved to the Global scope. 

## Use a scope

If you are an analyst, you must have a scope selected to be able to go to the **Explore** or **Queries** pages. If you are a PM, you work in the Global scope by default and you can go right to the **Solution** page to manage programs. If you are an admin, you create scopes, but you do not work within one. 

### To use a scope

1.	Open [Workplace Analytics](https://workplaceanalytics.office.com/). If prompted, enter your work credentials. If you are a PM or analyst and you have not been assigned a scope, you’ll see a notice that alerts you to that fact:

    ![Must have at least one scope](../images/wpa/setup/at-least-one-scope.png)  
 
If you see this notice, ask your Workplace Analytics admin to assign you to a scope. You cannot start using Workplace Analytics until an admin assigns you to one or more scopes. If you do not see this notice, go on to the next step.

2.	What you see now depends on your role and scope assignments: If you are analyst (you have the Analyst or Analyst limited role), go to step 3; if you have any other role, go to step 4. 

3.	Step for analysts: 

    * If you have only one scope (even the default "Global" scope), this is the scope that you will use. Skip the rest of these steps. You can go to the **Explore** page or the **Queries** page to start your work. On those pages, you will see only the data to which your scope grants you access.  
    * If you have more than one scope, the **Scope** drop-down menu at the top of the **Home** page displays the scopes that have been assigned to you. Open this menu and select one:

       ![Select a scope](../images/wpa/setup/select-one-no-global.png)
 
      After you’ve chosen the scope to work with, you can skip the rest of these steps and go to the **Explore** page or the **Queries** page.  

4.	If you have a non-analyst role, your choice depends on the role (or roles) that you’ve been assigned:

    * **Both PM and Analyst:** If you have both the PM role and an Analyst role, the data you see depends on the page that you open. Solutions are accessible only in the Global scope. A person with both the PM and analyst roles can access solutions in Global scope and access the **Explore** and **Queries** pages in other scopes that they have been granted. 
    * **PM only:** PMs do not need to select a scope because they automatically use Global scope. If you’re a PM, go to the **Solution** page. 
    * **Not an analyst or program manager:** If you’re signed in to Workplace Analytics and you do not have an analyst or PM role, you are an admin and scope doesn’t affect you. Go to the **Settings** page. 

## Define a scope

Workplace Analytics admins define scopes on the Settings page. One aspect of this task is assigning scopes to analysts. As you, the admin, define a scope, you can assign the scope to one or more analysts.

> [!Important] 
> Plan your scopes carefully before you start to define them. Note the following:
>  * **No more than five scopes.** An organization can have a maximum of five scopes.
>  * **Scopes are not editable.** After you create a scope, the scope cannot be edited. 

### To define a scope

1.	Open the Workplace Analytics **Home** page. If prompted, enter your Microsoft credentials. 
2.	Open the **Settings** page and select **Access control**.
3.	In the **Scope-based access control** area, select **Add scope**:

    ![Admin settings](../images/wpa/setup/admin-settings.png)
 
4.	On the **Access control > New scope** page, type the name of the new scope and optionally type a description. 
5.	**Define filters.** Under **Filters**, add one or more filters to define the data that will fall within the scope that you are creating:

    ![New scope](../images/wpa/setup/new-scope.png)
 
    > [!Note] 
    > You can filter by only one attribute. For example, if you create a filter that uses the Organization attribute, you could produce the following filter clauses:  
    >  * Organization + Equals + <name_of_manager_1> AND 
    >   
    >    Organization + Equals + <name_of_manager_2>
    >   
    > But you cannot add another clause that uses a different attribute, such as:
    >   * Domain + Equals + <domain_name> 

6.	**Select analysts**. Under **Analysts**, select one or more analysts who will have access to this scope. Only the analysts that you select will be able to perform analyses in Workplace Analytics.     
   ![Select analysts](../images/wpa/setup/analysts.png)
 
7.	**Select attributes**. Select which attributes from the organizational data to include in the scope. To exclude an attribute from the scope, leave it unselected. 
 
8.	**Select visibility of attributes**. You might want one or more attributes to not be visible to analysts who work in this scope. For example, "sales quota" might be a sensitive attribute that nevertheless has been uploaded in the organizational data. To hide the "sales quota" attribute, select it and then set its **Visibility** to **Hash in report**. 

    ![Select visibility](../images/wpa/setup/select-visibility.png)



