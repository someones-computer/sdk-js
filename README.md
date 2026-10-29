# @someones-computer/sdk-js@1.0.0

A TypeScript SDK client for the localhost API.

## Usage

First, install the SDK from npm.

```bash
npm install @someones-computer/sdk-js --save
```

Next, try it out.


```ts
import {
  Configuration,
  AdoptionApprovalApi,
} from '@someones-computer/sdk-js';
import type { AdoptionApprovalsDecideRequest } from '@someones-computer/sdk-js';

async function example() {
  console.log("🚀 Testing @someones-computer/sdk-js SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AdoptionApprovalApi(config);

  const body = {
    // AdoptionApprovalAdoptionApprovalInput | The new AdoptionApproval resource
    adoptionApprovalAdoptionApprovalInput: ...,
  } satisfies AdoptionApprovalsDecideRequest;

  try {
    const data = await api.adoptionApprovalsDecide(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```


## Documentation

### API Endpoints

All URIs are relative to *http://localhost*

| Class | Method | HTTP request | Description
| ----- | ------ | ------------ | -------------
*AdoptionApprovalApi* | [**adoptionApprovalsDecide**](docs/AdoptionApprovalApi.md#adoptionapprovalsdecide) | **POST** /api/adoption_approvals | Creates a AdoptionApproval resource.
*AdoptionApprovalApi* | [**adoptionApprovalsGet**](docs/AdoptionApprovalApi.md#adoptionapprovalsget) | **GET** /api/adoption_approvals/{id} | Retrieves a AdoptionApproval resource.
*AdoptionApprovalApi* | [**adoptionApprovalsList**](docs/AdoptionApprovalApi.md#adoptionapprovalslist) | **GET** /api/adoption_approvals | Retrieves the collection of AdoptionApproval resources.
*AdoptionApprovalApi* | [**adoptionApprovalsWithdraw**](docs/AdoptionApprovalApi.md#adoptionapprovalswithdraw) | **DELETE** /api/adoption_approvals/{id} | Removes the AdoptionApproval resource.
*ApplicationApi* | [**applicationsCreate**](docs/ApplicationApi.md#applicationscreate) | **POST** /api/applications | Creates a Application resource.
*ApplicationApi* | [**applicationsDelete**](docs/ApplicationApi.md#applicationsdelete) | **DELETE** /api/applications/{id} | Removes the Application resource.
*ApplicationApi* | [**applicationsGet**](docs/ApplicationApi.md#applicationsget) | **GET** /api/applications/{id} | Retrieves a Application resource.
*ApplicationApi* | [**applicationsList**](docs/ApplicationApi.md#applicationslist) | **GET** /api/applications | Retrieves the collection of Application resources.
*ApplicationApi* | [**applicationsUpdate**](docs/ApplicationApi.md#applicationsupdate) | **PATCH** /api/applications/{id} | Updates the Application resource.
*CreditTransactionApi* | [**creditTransactionsGet**](docs/CreditTransactionApi.md#credittransactionsget) | **GET** /api/credit_transactions/{id} | Retrieves a CreditTransaction resource.
*CreditTransactionApi* | [**creditTransactionsList**](docs/CreditTransactionApi.md#credittransactionslist) | **GET** /api/credit_transactions | Retrieves the collection of CreditTransaction resources.
*DeploymentApi* | [**deploymentsBundleUploadConfirm**](docs/DeploymentApi.md#deploymentsbundleuploadconfirm) | **POST** /api/deployments/bundle_uploads/confirm | Creates a Deployment resource.
*DeploymentApi* | [**deploymentsBundleUploadDeclare**](docs/DeploymentApi.md#deploymentsbundleuploaddeclare) | **POST** /api/deployments/bundle_uploads | Creates a Deployment resource.
*DeploymentApi* | [**deploymentsCreate**](docs/DeploymentApi.md#deploymentscreate) | **POST** /api/deployments | Creates a Deployment resource.
*DeploymentApi* | [**deploymentsDelete**](docs/DeploymentApi.md#deploymentsdelete) | **DELETE** /api/deployments/{id} | Removes the Deployment resource.
*DeploymentApi* | [**deploymentsEndpoints**](docs/DeploymentApi.md#deploymentsendpoints) | **GET** /api/deployments/{id}/endpoints | Retrieves the collection of Deployment resources.
*DeploymentApi* | [**deploymentsGet**](docs/DeploymentApi.md#deploymentsget) | **GET** /api/deployments/{id} | Retrieves a Deployment resource.
*DeploymentApi* | [**deploymentsList**](docs/DeploymentApi.md#deploymentslist) | **GET** /api/deployments | Retrieves the collection of Deployment resources.
*DeploymentApi* | [**deploymentsUpdate**](docs/DeploymentApi.md#deploymentsupdate) | **PATCH** /api/deployments/{id} | Updates the Deployment resource.
*DeploymentAccessGateApi* | [**deploymentAccessGatesCreate**](docs/DeploymentAccessGateApi.md#deploymentaccessgatescreate) | **POST** /api/deployment_access_gates | Creates a DeploymentAccessGate resource.
*DeploymentAccessGateApi* | [**deploymentAccessGatesDelete**](docs/DeploymentAccessGateApi.md#deploymentaccessgatesdelete) | **DELETE** /api/deployment_access_gates/{id} | Removes the DeploymentAccessGate resource.
*DeploymentAccessGateApi* | [**deploymentAccessGatesGet**](docs/DeploymentAccessGateApi.md#deploymentaccessgatesget) | **GET** /api/deployment_access_gates/{id} | Retrieves a DeploymentAccessGate resource.
*DeploymentAccessGateApi* | [**deploymentAccessGatesList**](docs/DeploymentAccessGateApi.md#deploymentaccessgateslist) | **GET** /api/deployment_access_gates | Retrieves the collection of DeploymentAccessGate resources.
*DeploymentAccessGateApi* | [**deploymentAccessGatesUpdate**](docs/DeploymentAccessGateApi.md#deploymentaccessgatesupdate) | **PATCH** /api/deployment_access_gates/{id} | Updates the DeploymentAccessGate resource.
*ManagedServiceApi* | [**managedServicesCreate**](docs/ManagedServiceApi.md#managedservicescreate) | **POST** /api/managed_services | Creates a ManagedService resource.
*ManagedServiceApi* | [**managedServicesDelete**](docs/ManagedServiceApi.md#managedservicesdelete) | **DELETE** /api/managed_services/{id} | Removes the ManagedService resource.
*ManagedServiceApi* | [**managedServicesGet**](docs/ManagedServiceApi.md#managedservicesget) | **GET** /api/managed_services/{id} | Retrieves a ManagedService resource.
*ManagedServiceApi* | [**managedServicesList**](docs/ManagedServiceApi.md#managedserviceslist) | **GET** /api/managed_services | Retrieves the collection of ManagedService resources.
*ManagedServiceApi* | [**managedServicesListRetired**](docs/ManagedServiceApi.md#managedserviceslistretired) | **GET** /api/managed_services/retired | Retrieves the collection of ManagedService resources.
*ManagedServiceApi* | [**managedServicesRestore**](docs/ManagedServiceApi.md#managedservicesrestore) | **POST** /api/managed_services/{id}/restore | Creates a ManagedService resource.
*ManagedServiceApi* | [**managedServicesResume**](docs/ManagedServiceApi.md#managedservicesresume) | **POST** /api/managed_services/{id}/resume | Creates a ManagedService resource.
*ManagedServiceApi* | [**managedServicesSuspend**](docs/ManagedServiceApi.md#managedservicessuspend) | **POST** /api/managed_services/{id}/suspend | Creates a ManagedService resource.
*OrganizationApi* | [**organizationsCreate**](docs/OrganizationApi.md#organizationscreate) | **POST** /api/organizations | Creates a Organization resource.
*OrganizationApi* | [**organizationsDelete**](docs/OrganizationApi.md#organizationsdelete) | **DELETE** /api/organizations/{id} | Removes the Organization resource.
*OrganizationApi* | [**organizationsGet**](docs/OrganizationApi.md#organizationsget) | **GET** /api/organizations/{id} | Retrieves a Organization resource.
*OrganizationApi* | [**organizationsList**](docs/OrganizationApi.md#organizationslist) | **GET** /api/organizations | Retrieves the collection of Organization resources.
*OrganizationApi* | [**organizationsUpdate**](docs/OrganizationApi.md#organizationsupdate) | **PATCH** /api/organizations/{id} | Updates the Organization resource.
*ServiceBindingApi* | [**serviceBindingsCreate**](docs/ServiceBindingApi.md#servicebindingscreate) | **POST** /api/service_bindings | Creates a ServiceBinding resource.
*ServiceBindingApi* | [**serviceBindingsDelete**](docs/ServiceBindingApi.md#servicebindingsdelete) | **DELETE** /api/service_bindings/{id} | Removes the ServiceBinding resource.
*ServiceBindingApi* | [**serviceBindingsGet**](docs/ServiceBindingApi.md#servicebindingsget) | **GET** /api/service_bindings/{id} | Retrieves a ServiceBinding resource.
*ServiceBindingApi* | [**serviceBindingsList**](docs/ServiceBindingApi.md#servicebindingslist) | **GET** /api/service_bindings | Retrieves the collection of ServiceBinding resources.
*SwarmApi* | [**swarmsCreate**](docs/SwarmApi.md#swarmscreate) | **POST** /api/swarms | Creates a Swarm resource.
*SwarmApi* | [**swarmsDelete**](docs/SwarmApi.md#swarmsdelete) | **DELETE** /api/swarms/{id} | Removes the Swarm resource.
*SwarmApi* | [**swarmsGet**](docs/SwarmApi.md#swarmsget) | **GET** /api/swarms/{id} | Retrieves a Swarm resource.
*SwarmApi* | [**swarmsList**](docs/SwarmApi.md#swarmslist) | **GET** /api/swarms | Retrieves the collection of Swarm resources.
*SwarmApi* | [**swarmsUpdate**](docs/SwarmApi.md#swarmsupdate) | **PATCH** /api/swarms/{id} | Updates the Swarm resource.
*VolumeApi* | [**volumesCreate**](docs/VolumeApi.md#volumescreate) | **POST** /api/volumes | Creates a Volume resource.
*VolumeApi* | [**volumesDelete**](docs/VolumeApi.md#volumesdelete) | **DELETE** /api/volumes/{id} | Removes the Volume resource.
*VolumeApi* | [**volumesGet**](docs/VolumeApi.md#volumesget) | **GET** /api/volumes/{id} | Retrieves a Volume resource.
*VolumeApi* | [**volumesList**](docs/VolumeApi.md#volumeslist) | **GET** /api/volumes | Retrieves the collection of Volume resources.


### Models

- [AdoptionApproval](docs/AdoptionApproval.md)
- [AdoptionApprovalAdoptionApprovalInput](docs/AdoptionApprovalAdoptionApprovalInput.md)
- [Application](docs/Application.md)
- [ApplicationJsonMergePatch](docs/ApplicationJsonMergePatch.md)
- [BundleAdditionalContextInput](docs/BundleAdditionalContextInput.md)
- [BundleContextInput](docs/BundleContextInput.md)
- [BundleForwardedImageInput](docs/BundleForwardedImageInput.md)
- [BundleUploadTarget](docs/BundleUploadTarget.md)
- [ConstraintViolation](docs/ConstraintViolation.md)
- [ConstraintViolationViolationsInner](docs/ConstraintViolationViolationsInner.md)
- [CreditTransaction](docs/CreditTransaction.md)
- [CreditTransactionEngineMillis](docs/CreditTransactionEngineMillis.md)
- [CreditTransactionUsageBytes](docs/CreditTransactionUsageBytes.md)
- [Deployment](docs/Deployment.md)
- [DeploymentAccessGate](docs/DeploymentAccessGate.md)
- [DeploymentAccessGateJsonMergePatch](docs/DeploymentAccessGateJsonMergePatch.md)
- [DeploymentBundleUploadConfirmInput](docs/DeploymentBundleUploadConfirmInput.md)
- [DeploymentBundleUploadConfirmOutput](docs/DeploymentBundleUploadConfirmOutput.md)
- [DeploymentBundleUploadDeclareInput](docs/DeploymentBundleUploadDeclareInput.md)
- [DeploymentBundleUploadDeclareOutput](docs/DeploymentBundleUploadDeclareOutput.md)
- [DeploymentDeploymentEndpoint](docs/DeploymentDeploymentEndpoint.md)
- [DeploymentJsonMergePatch](docs/DeploymentJsonMergePatch.md)
- [DeploymentJsonMergePatchBuildContextsValueValue](docs/DeploymentJsonMergePatchBuildContextsValueValue.md)
- [Failure](docs/Failure.md)
- [Machine](docs/Machine.md)
- [ManagedService](docs/ManagedService.md)
- [ManagedServiceEngine](docs/ManagedServiceEngine.md)
- [ManagedServiceLastLoadMillis](docs/ManagedServiceLastLoadMillis.md)
- [ManagedServiceManagedServiceInput](docs/ManagedServiceManagedServiceInput.md)
- [ManagedServicePendingLoadMillis](docs/ManagedServicePendingLoadMillis.md)
- [ManagedServiceQuotaBytes](docs/ManagedServiceQuotaBytes.md)
- [ManagedServiceUsageBytes](docs/ManagedServiceUsageBytes.md)
- [Membership](docs/Membership.md)
- [ModelError](docs/ModelError.md)
- [Organization](docs/Organization.md)
- [OrganizationJsonMergePatch](docs/OrganizationJsonMergePatch.md)
- [OrganizationSignal](docs/OrganizationSignal.md)
- [PortAllocation](docs/PortAllocation.md)
- [ProxmoxInstance](docs/ProxmoxInstance.md)
- [Service](docs/Service.md)
- [ServiceBinding](docs/ServiceBinding.md)
- [ServiceBindingServiceBindingInput](docs/ServiceBindingServiceBindingInput.md)
- [ServiceCpuLimit](docs/ServiceCpuLimit.md)
- [ServiceCpuReservation](docs/ServiceCpuReservation.md)
- [ServiceHealthcheckValue](docs/ServiceHealthcheckValue.md)
- [ServiceMemLimit](docs/ServiceMemLimit.md)
- [ServiceMemReservation](docs/ServiceMemReservation.md)
- [ServicePortsInnerValue](docs/ServicePortsInnerValue.md)
- [Swarm](docs/Swarm.md)
- [SwarmJsonMergePatch](docs/SwarmJsonMergePatch.md)
- [SwarmNode](docs/SwarmNode.md)
- [User](docs/User.md)
- [Volume](docs/Volume.md)
- [VolumeVolumeInput](docs/VolumeVolumeInput.md)

### Authorization


Authentication schemes defined for the API:
<a id="bearerAuth"></a>
#### bearerAuth


- **Type**: HTTP Bearer Token authentication

## About

This TypeScript SDK client supports the [Fetch API](https://fetch.spec.whatwg.org/)
and is automatically generated by the
[OpenAPI Generator](https://openapi-generator.tech) project:

- API version: `1.0.0`
- Package version: `1.0.0`
- Generator version: `7.26.0`
- Build package: `org.openapitools.codegen.languages.TypeScriptFetchClientCodegen`

The generated npm module supports the following:

- Environments
  * Node.js
  * Webpack
  * Browserify
- Language levels
  * ES5 - you must have a Promises/A+ library installed
  * ES6
- Module systems
  * CommonJS
  * ES6 module system


## Development

Bugs and feature requests for the someones.computer ecosystem are tracked
centrally at
[Grey.ooo/Someones.Computer](https://git.grey.ooo/Grey.ooo/Someones.Computer) —
this repo's own issue tracker is disabled. Pull requests are still welcome here.

### Building

To build the TypeScript source code, you need to have Node.js and npm installed.
After cloning the repository, navigate to the project directory and run:

```bash
npm install
npm run build
```

### Publishing

Once you've built the package, you can publish it to npm:

```bash
npm publish
```

## License

[]()
