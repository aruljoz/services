---

copyright:

  years: 2015, 2018
lastupdated: "2018-02-13"

---

{:new_window: target="_blank"}  
{:shortdesc: .shortdesc}


# Adding a new credential
{: #service_credentials}

You can generate a new set of credentials for cases where you want to manually connect an external consumer to an {{site.data.keyword.Bluemix}} service. For example, if you are trying to bind an AWS app to a Watson service, you need to generate a new credential that can be used to bind them together.

## Adding a credential when binding an IAM-enabled service
{: #IAM}

Services that are managed by {{site.data.keyword.Bluemix}} Identity and Access Management (IAM) can generate a resource key, also known as a credential. Credentials are service-specific and vary based on how each service defines the credentials they need to generate. A credential might contain a user name, password, host name, port and a URL. 

However, while the contents of each credential is unique to the service that generates it, all services managed by IAM require that new credentials include an IAM Service access role. Some services might generate additional data that requires paramaters to be passed in. For example, a service might require you to input a language parameter to set the default language returned in the resource key that's generated. 

Complete the following steps to add a new credential to a service that's managed by IAM:

1. From the dashboard, select the name of the service to open the service details page. Then, select the Credentials tab, and click **New Credential + **.
2. From the Add New Credential dialog, provide a **Name**.
3. Specify the role. This value sets the IAM service access role. For more information, see: [IAM Access](/docs/iam/users_roles.html#userroles)
4. Optionally, you can provide a Service ID by either allowing IAM to generate a unique value for you, or by providing an existing Service ID. For more information, see: [Creating and managing service IDs](https://console.stage1.bluemix.net/docs/iam/serviceid.html#serviceids)
3. Optionally, you can provide additional parameters as a valid JSON object containing service-specific configuration parameters, provided either in-line or in a file.

  **Note**. Most services do not require additional parameters, and for services that do, each service defines its own unique list of parameters. For a list of supported configuration parameters, see the documentation for the particular service offering.
4. Click **Add** to generate the new service credential.

## Adding a credential when binding a Cloud Foundry service
{: #cf}

Cloud Foundry services can generate a service key, also known as a credential. Credentials are service-specific and vary based on how each service defines the credentials they need to generate. A service credential might contain a user name, password, host name, port and a URL. 

However, the contents of each credential is unique to the service that generates it. Some services might generate additional data that requires paramaters to be passed in. For example, a service might require you to input a language parameter to set the default language returned in the service key that's generated. 

Complete the following steps to add a new Cloud Foundry credential:

1. From the service details page, select the Credentials tab, and click **New Credential + **.
2. From the Add New Credential dialog, provide a **Name**.
3. Optionally, you can provide additional parameters as a valid JSON object containing service-specific configuration parameters, provided either in-line or in a file.

  **Note**. Most services do not require additional parameters, and for services that do, each service defines its own unique list of parameters. For a list of supported configuration parameters, see the documentation for the particular service offering.
4. Click **Add** to generate the new service credential.

