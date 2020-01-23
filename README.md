# Lighning_marathon
Lightning marathon 31 July

1) Locker Service In Lightning Blocks :-
Lightning Locker is a powerful security architecture for Lightning components. Lightning Locker enhances security by isolating Lightning components that belong to one namespace from components in a different namespace. Lightning Locker also promotes best practices that improve the supportability of your code by only allowing access to supported APIs and eliminating access to non-published framework internals.

2) Lightning is MVC – T/F = False.  it’s a component-based framework.

3) Dashboard can add how many Lightning Components - Each dashboard can have up to 20 components.

4) Number of Bucket Field - Each report is permitted to have a maximum of 5 individual bucket fields apeice. Each of these bucket fields are permitted to have 20 individual "buckets."

5) <include:slds > - apex:slds. Allows Visualforce pages to reference Lightning Design System styling and to include custom themes. Use this component instead of uploading the Lightning Design System as a static resource. Include <apex:slds /> in a Visualforce page to use Lightning Design System stylesheets in the page.

5)Which is  Removed From Lightning assistance - Salesforce removed the ability to see overdue tasks from the Assistant (related to any object) as they introduced a tasks component on home. 

 

                1) all lead

                2) Opp not worked in 30 days

                3) recent opp

                4)

               

6) Slds for  Grid System - slds-grid
                         - Add a grid container by adding slds-grid to an HTML element
                         - Add as many slds-col elements as you want inside of your grid container

7) How to declare Table in Slds - slds-table
                                - apply the slds-table class to the table element. This class creates a table with formatted cells and                                     allows you to use data table utilities.

8) Meaning of slds--1---4 -  sizing class names are set up in a human-readable format, e.g. .slds-size--1-of-4. This equates to a width of 25%.
refer this : https://archive-1_0_5.lightningdesignsystem.com/components/utilities/sizing

9) What is the Changset to add aura Components -  Aura Component Bundle
refer: https://salesforce.stackexchange.com/questions/232613/how-to-deploy-lightning-component-with-change-sets
     : https://help.salesforce.com/articleView?id=changesets_about_components.htm&type=0

10) which is Not  Macros Type                

                1) Reversible(this is not macro type)


                2) Irreversible

                3) regular 
                4) Bulk

 refer : https://www.forcetalks.com/blog/macros-one-of-the-most-severely-underused-salesforce-feature/

11) Order in Which ltng Out is Called --->relevant link : https://developer.salesforce.com/blogs/developer-relations/2016/02/lightning-components-visualforce-lightning.html

12) Auto Wiring In lightning - a controller <componentName>Controller.js is auto-wired to its component and like all other resources(helper,design,style,documentation,renderer,svg), which means that you can use the controller within the scope of that component.
 refer:https://developer.salesforce.com/docs/atlas.en-us.lightning.meta/lightning/components_bundle.htm

13)How is  Ltng Out  in VF ?-There are three steps to add Aura components to a Visualforce page.
                            -Add the Lightning Components for Visualforce JavaScript library to your Visualforce page using the                                      <apex:includeLightning/> component.
                            -Create and reference a Lightning app that declares your component dependencies.
                            -Write a JavaScript function that creates the component on the page using $Lightning.createComponent().
  refer: https://developer.salesforce.com/docs/atlas.en-us.lightning.meta/lightning/components_visualforce.htm

14 FLS in Lightning data service - True
                                 - FLS is ensured by manually or by lightning Data Service. 
refer  : https://www.forcetalks.com/salesforce-topic/how-to-ensure-fls-while-working-with-lightning-component/

15) Characteristics  OF lightning Framework – It has an event- driven architecture and It includes responsive components

     A. It works with existing Visualforce pages
     B. It uses XML as its data format
     C. It has an event- driven architecture
     D. It includes responsive components


16)Vf Can be used in -Developers can use Visualforce pages to:
  -Override standard buttons, such as the New button for accounts, or the Edit button for contacts
  -Override tab overview pages, such as the Accounts tab home page
  -Define custom tabs
  -Embed components in detail page layouts
  -Create dashboard components or custom help pages
  -Customize, extend, or integrate the sidebars in the Salesforce console (custom console components)
  -Add menu items, actions, and mobile cards in the Salesforce app

17 ) Component To Component Calling  In lightning ( Attributes , Application and component )- We can call component inside component and components inside application.

18) External Lookup - An external lookup relationship links a child standard, custom, or external object to a parent external object. The values of the standard External ID field on the parent external object are matched against the values of the external lookup relationship field. For a child external object, the values of the external lookup relationship field come from the specified External Column Name.
refer : https://help.salesforce.com/articleView?id=external_object_relationships.htm&type=5
      : https://help.salesforce.com/articleView?id=external_object_external_lookup_relationships.htm&type=5

19) Upsert and external Id is used in "  ? - https://www.jitendrazaa.com/blog/salesforce/all-about-upsert-and-external-id-in-dataloader-and-apex-videos/

20)Standard Component Can be placed In App builder :  Canvas

21) When moved to Lightning experience which user will be able to see---

22) How Can you Switch between 2 accounts in Lightning

23) Lightning experience supports

accnt , Contact hierarcy , Shows upto 200 contacts- 2000

24 Reports Sharing ---on the basis of access level(viewwer,manager,editor,no access)

25)Odata 2.0 is Used ?-Salesforce Connect uses Open Data Protocol Version 2.0 or Version 4.0 to access data that’s stored outside Salesforce.

26) How To load Aura :Doinit handler:
This aura handler goes like this:

<Aura> --> lightning specific keyword same as  <apex> in salesforce classic. 
<aura:handler> --> is used to handle stanadard / custom events. 
name="init" --> this is defining the name of aura:handler
value={!this}  --> passing the current information to controller
action ={!c.doInit} --> calling the "doInit" of controller.

27) From where events are fired In Lightning-à 3rd party - 
The third party javascript code is a different story. The lightning documentation says that you can only register/fire events from built-in resources such as components or related controllers/helpers.
It appears you probably want to write a wrapper function in your component which will call the third party code and fire the event when done.


30 )lightning/SF1 can be Customise Using App Builder ?
The Lightning App Builder is a point-and-click tool that makes it easy to create custom pages for the Salesforce mobile app and Lightning Experience, giving your users what they need all in one place. The Lightning App Builder is also a one-stop shop for configuring Lightning apps.

31) How to deploy lightning components using change sets?
Ans - Aura Component bnundle
