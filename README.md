---
page_type: sample
languages:
- java
products:
- azure
extensions:
  services: Compute
  platforms: java
---

# Getting Started with Compute - Manage Disk Encryption Set - in Java #


  Azure Compute sample for managing disk encryption sets -
   - Create a key vault kv1 and key k1
   - Create a disk encryption set, des1, with key vault kv1, key k1 and encryption type
      ENCRYPTION_AT_REST_WITH_CUSTOMER_KEY
   - Grant the disk encryption set access to the key vault by defining key vault access policy
   - Create a new key vault kv2 with RBAC enabled and key k2
   - Create a new disk encryption set des2 with key vault kv2, key k2, encryption type
      ENCRYPTION_AT_REST_WITH_PLATFORM_AND_CUSTOMER_KEYS and grant it role-based access to kv2
   - Create a virtual machine, with os disk encrypted by des1 and a data disk encrypted by des2
 

## Running this Sample ##

To run this sample:

See [DefaultAzureCredential](https://github.com/Azure/azure-sdk-for-java/tree/main/sdk/identity/azure-identity#defaultazurecredential) and prepare the authentication works best for you. For more details on authentication, please refer to [AUTH.md](https://github.com/Azure/azure-sdk-for-java/blob/main/sdk/resourcemanager/docs/AUTH.md).

    git clone https://github.com/Azure-Samples/compute-java-manage-disk-encryption-set.git

    cd compute-java-manage-disk-encryption-set

    mvn clean compile exec:java

## More information ##

For general documentation as well as quickstarts on how to use Azure Management Libraries for Java, please see [here](https://aka.ms/azsdk/java/mgmt).

Start to develop applications with Java on Azure [here](http://azure.com/java).

If you don't have a Microsoft Azure subscription you can get a FREE trial account [here](http://go.microsoft.com/fwlink/?LinkId=330212).

---

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.