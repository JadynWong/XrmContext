# Release Notes

### 1.2.0 - March 29 2016
* Added functionality that helps with alternate keys for entities, 
  and in order to support this, the dependency `Microsoft.CrmSdk.CoreAssemblies` has been increased to the newest version again
* Added a comment description for entity classes
* Added several functions to easily create CRM requests from entity objects
* Added static retrieve methods (`.Retrieve_<keyname>`) on entity classes that makes it possible to retrieve records using alternate keys
* Added methods (`.AltKey_<keyname>`) that helps set the alternate keys correctly on an entity object before upserting it
* Added `.Retrieve<T>`, `.Upsert`, `.Assign` and `.SetState` extension methods on `IOrganizationService` to simplify the use of these requests
* Added `.PerformAsBulk` extension method on `IOrganizationService` that performs requests as bulk
* To support multiple versions of `CrmSdk.CoreAssemblies` in the target library, a new "***/sdkversion***" argument has been added

### 1.1.2 - February 24 2016
* Added "***/genconfig***" argument which generates a dummy configuration file to use
* Added "***/useconfig***" argument, see [usage for more information](tool-usage.html#Configuration-file)
* Added version print when using the executable
* Changed exit-code for the executable to be 1 instead of 0, when it encounters an exception

### 1.1.1 - December 29 2015
* Improved retrieval of CRM metadata
* Fixed incorrect argument description

### 1.1.0 - December 18 2015
* Reduced version requirements to support backward-compatibility:
  * Reduced requirement of the dependency `Microsoft.CrmSdk.CoreAssemblies` to 5.0.18 or greater
  * Reduced used .NET Framework to version 4.5.2

### 1.0.1 - December 07 2015
* Fixed an incorrect string set in some `AttributeLogicalName` attributes.

### 1.0.0 - October 15 2015
* Initial public release