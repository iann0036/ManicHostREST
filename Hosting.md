# Hosting
## Methods
### GET /hosting
Returns a list of the hosting packages in your account.

#### Request
There are no request parameters for this method.

#### Response
- _hosting_ - A list of hosting packages
  - _id_ - The unique identifier of the hosting package
  - _domain_ - The main domain name
  - _plan_ - The associated hosting plan
  - _expiry_ - The expiry date of the hosting package as a timestamp

### GET /hosting/{id}
Returns information about a specific hosting package in your account.

#### Request
- _id_ - The unique identifier of the hosting package

#### Response
- _id_ - The unique identifier of the hosting package
- _domain_ - The main domain name
- _plan_ - The associated hosting plan
- _expiry_ - The expiry date of the hosting package as a timestamp

### DELETE /hosting/{id}
Deletes a hosting package in your account instantly.

#### Request
- _id_ - The unique identifier of the hosting package

#### Response
- _deletion_ - Boolean confirmation the hosting package has been deleted

### DELETE /hosting/{id}/scheduled
Schedules the deletion of a hosting package in your account at the end of the billing cycle.

#### Request
- _id_ - The unique identifier of the hosting package

#### Response
- _deletion_ - Boolean confirmation the hosting package has been scheduled for deletion
