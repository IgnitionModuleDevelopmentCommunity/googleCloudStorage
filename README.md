# googleCloudStorage
Provides script functions for reading and writing files to Google's Cloud Storage.

Note that this is a work in progress.  Feel free to work on the code and contribute any changes.

## Status
This code is not yet functional.  This uses maven includes from the java Google Cloud Client Libraries.

For reference on how to use GCS with Java, check out the docs  
https://cloud.google.com/storage/docs/reference/libraries

## Next steps:
These are the next development steps and can be undertaken by anyone interested in using or contributing to the code.
1. Create script functions to expose things like StorageOptions.getDefaultInstance()
2. Figure out how to use authentication for GCS's new Google Cloud Client Libraries, along with server centric credentials
(https://cloud.google.com/docs/authentication#getting_credentials_for_server-centric_flow has some details, but it uses the old Google API Client Libraries for its example)
3. Write some python examples in Ignition to do the authentication and then call the new storage functions.  Export the project with these examples and upload to this repo.  (Check out the azureServiceBus project in this community for a guide of how this can look.)

## Background
Google has released several libraries over the years for their cloud services.  This module uses the most recent libraries (as of 2017).

"Google Cloud Client Libraries" - These are the newer librares, which this module is based on.
https://cloud.google.com/storage/docs/reference/libraries

"Google API Client Libraries" - Older libraries, with a mess of dependencies, and multiple ways to do things in Google Cloud Storage (Examples: Google API Client Library for Java, Cloud Storage JSON API Client Library for Java)