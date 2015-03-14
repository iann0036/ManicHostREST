# Domains
## Methods
### GET /domains
Returns a list of the domains in your account.

#### Request
There are no request parameters for this method.

#### Response
- _domains_ - A list of domains
  - _id_ - The unique identifier of the domain
  - _domain_ - The domain name
  - _expiry_ - The expiry date of the domain as a timestamp

### GET /domains/{id}
Returns information about a specific domain in your account.

#### Request
- _id_ - The unique identifier of the domain

#### Response
- _id_ - The unique identifier of the domain
- _domain_ - The domain name
- _expiry_ - The expiry date of the domain as a timestamp

### DELETE /domains/{id}
Deletes a domain in your account instantly.

#### Request
- _id_ - The unique identifier of the domain

#### Response
- _deletion_ - Boolean confirmation the domain has been deleted

### DELETE /domains/{id}/scheduled
Schedules the deletion of a domain in your account at the end of the billing cycle.

#### Request
- _id_ - The unique identifier of the domain

#### Response
- _deletion_ - Boolean confirmation the domain has been scheduled for deletion
