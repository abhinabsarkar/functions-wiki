# Azure Functions - Wiki

## Code samples, Use cases
* [Upload Files Into Azure Blob Storage Using Azure Functions In C#](https://www.c-sharpcorner.com/article/how-to-upload-files-into-azure-blog-storage-using-azure-functions-in-c-sharp/)
* [Send And Read Messages From Azure Service Bus Queues Using Azure Functions in C#](https://www.c-sharpcorner.com/article/how-to-send-read-messages-from-azure-service-bus-queues-using-azure/)
* [Durable functions & chaining](https://github.com/abhinabsarkar/az-functions)

### Managed Identity for Azure Functions
* [Azure Function returning SAS token for Storage account](https://github.com/abhinabsarkar/fn-sas-token-conn-string)
* [Using Managed Identity between Azure Functions and Azure Storage](https://github.com/abhinabsarkar/fn-sas-url-mngd-identity)
* [Using Managed Identity between Azure Functions and Azure Storage - Detailed sample code](https://learn.microsoft.com/en-us/samples/azure-samples/functions-storage-managed-identity/using-managed-identity-between-azure-functions-and-azure-storage/)
    * [Permissions required to the identity](https://learn.microsoft.com/en-us/azure/azure-functions/functions-reference?tabs=blob#grant-permission-to-the-identity)
    * Uses `UserDelegationKey` to generate the SAS token (required when using Managed Identity)
        > The token can be generated without the UserDelegationKey if not using Managed Identity. Refer [Get User Delegation Key](https://learn.microsoft.com/en-us/rest/api/storageservices/get-user-delegation-key)
    * Create & return SAS URL for Storage
    * Fetch & return Storage Account keys
    * Regenerate Storage Account Keys