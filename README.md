# Devportal-JWT_APIs

## Description

API collection to call the JWT related endpoints in the devportal.

## Installation

This API collection has been created in [Postman](https://www.postman.com/).

### Postman

To install Postman, follow these steps:

1. Visit the [Postman website](https://www.postman.com/downloads/).
2. Download the version suitable for your OS.
3. Run the installer.

## API List

The `Devportal JWT.postman_collection.json` file contains the following APIs:

- `POST /api/v1/management/sites/{siteId}/applications/{appId}/signjwt`: Signs a JWT body payload.
- `POST /api/v1/management/sites/{siteId}/verifyjwt`: Verifies the signed JWT payload generated with the signjwt endpoint.
- `POST /api/v1/gateway/oauth2/jwttoken`: Uses the signed JWT payload generated with the signjwt endpoint to generate an access_token.

## Usage

After importing the `Devportal JWT.postman_collection.json` file into Postman, you need to configure the described variables in the overview section and then you can use the APIs by sending requests to them.

The required variables are the following:

- `devportal`: The Devportal Server FQDN without the trailing slash.
- `appId`: An application registered in the Devportal instance that have an **Auto Register Trusted Service** associated or that is registered in the **specific site (siteId)**.
- `siteId`: One registrar site that is available in the Devportal instance.
- `siteSecret`: The site secret for the siteId.

Please refer to the overview section as it contains more information about the endpoints and their use.
