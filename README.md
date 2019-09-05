# [DEPRECATED] Subscription service API

## Deprecation Notice

The Subscription service API was deprecated as of January 2018. This service is no longer maintained, and is no longer referenced by any releases of Mojaloop.

For a list of active Mojaloop repos, please refer to [Repo Details](https://mojaloop.io/documentation/repositories/) section of the Mojaloop documentation.

## Summary

This service is used for mapping between the users and phone numbers. It is supporting the following **private** API calls:

### Add subscription ###

* **URL**

  `/rpc/subscription/subscription/add`

* **Method**

  `POST`

* **Data Params**

  **Required**

   * `actorId [string] - Actor id`
   * `phoneNumber [string] - Phone number`
 
* **Success Response**

  * **Code:** 200 <br />
    **Content**
       * `subscriptionId [number] - Subscription id`
       * `actorId [string] - Actor id`
       * `phoneNumber [string] - Phone number`


### Get subscription ###

* **URL**

  `/rpc/subscription/subscription/get`

* **Method**

  `POST`

* **Data Params**

  **Optional**

   * `actorId [string] - Actor id`
   * `phoneNumber [string] - Phone number`
 
* **Success Response**

  * **Code:** 200 <br />
    **Content**
       * `actorId [string] - Actor id`
       * `phoneNumber [string] - Phone number`


### Remove subscription ###

* **URL**

  `/rpc/subscription/subscription/remove`

* **Method**

  `POST`

* **Data Params**

  **Optional**

   * `subscriptionId [number] - Subscription id`
 
* **Success Response**

  * **Code:** 200 <br />
    **Content**
       * `subscriptionId [number] - Subscription id`
