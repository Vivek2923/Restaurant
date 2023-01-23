# Restaurant
.Net Console Application for Accessing Dynamic CRM 365 
Software Required
.NET FrameWork 2022 (Visual C# language)

Go to https://dynamics.microsoft.com/en-us/dynamics-365-free-trial/. Click on Try for Free.
Create an Organization ID Ex. (XXXXXX@YYYY.onmicrosoft.com). Go to Azure Active Directory and register the app with Client ID (App ID)

Created a new .NET console app project. For this project we are using Visual Studio 2022.

In Solution Explorer, right-click on the project which I created and selected the Manage NuGet Packages and Install
      Microsoft.PowerPlatform.Dataverse.Client
      Microsoft.CrmSdk.CoreAssemblies
      Microsoft.CrmSdk.XrmTooling.CoreAssembly


Used in the Application
      using Microsoft.Crm.Sdk.Messages;
      using Microsoft.PowerPlatform.Dataverse.Client;
      using Microsoft.Xrm.Sdk.Messages;
      using Microsoft.Xrm.Sdk.Query;
      using Microsoft.Xrm.Sdk;
      using Microsoft.Xrm.Tooling.Connector;
      
Authentication type OAuth
For establishing the CRM connection CrmServiceClient class (Username,Password,Organization URL,AppID,ReturnURL,LoginPrompt)
Once the connection is made CRUD operation is performed.


