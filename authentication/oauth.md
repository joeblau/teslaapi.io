# OAuth

OAuth grant types supported

* `refresh_token`  
* `password`

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/oauth/token" %}
{% api-method-summary %}
Get Access Token
{% endapi-method-summary %}

{% api-method-description %}
Performs the login and returns the access token for all subsequent actions
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Content-Type" type="string" required=true %}
`application/json`
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="password" type="string" required=true %}
tesla.com user password
{% endapi-method-parameter %}

{% api-method-parameter name="email" type="string" required=true %}
tesla.com user email address
{% endapi-method-parameter %}

{% api-method-parameter name="client\_secret" type="string" required=true %}
`c7257eb71a564034f9419ee651c7d0e5f7aa6bfbd18bafb5c5c033b093bb2fa3`
{% endapi-method-parameter %}

{% api-method-parameter name="client\_id" type="string" required=true %}
`81527cff06843c8634fdc09e8ac0abefb46ac849f38fe1e431c2ef2106796384`
{% endapi-method-parameter %}

{% api-method-parameter name="grant\_type" type="string" required=true %}
`password` or `refresh_token`
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "access_token":"ACCESS_TOKEN_FOR_ALL_API_CALLS",
  "token_type":"bearer",
  "expires_in":3888000,
  "refresh_token":"REFRESH_TOKEN_FOR_REFRESH_API_CALL",
  "created_at":1571519135
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/oauth/revoke" %}
{% api-method-summary %}
Revoke Access Token
{% endapi-method-summary %}

{% api-method-description %}
Revokes the `{access_token}` issued by the token command
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="Content-Type" type="string" required=false %}
`application/json`
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="token" type="string" required=false %}
`{access_token}`
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

