# OAuth

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/oauth/token" %}
{% api-method-summary %}
Token
{% endapi-method-summary %}

{% api-method-description %}
This endpoint performs a login using the owners plain text email and password from https://my.teslamotors.com/user/login  
  
**client\_id:** `81527cff06843c8634fdc09e8ac0abefb46ac849f38fe1e431c2ef2106796384`  
**client\_secret:** `c7257eb71a564034f9419ee651c7d0e5f7aa6bfbd18bafb5c5c033b093bb2fa3`
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Content-Type" type="string" required=true %}
`application/json`
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="grant\_type" type="string" required=true %}
OAuth grant types supported  
- `refresh_token`  
- `password`
{% endapi-method-parameter %}

{% api-method-parameter name="client\_id" type="string" required=true %}
The OAuth client ID `{client_id}`
{% endapi-method-parameter %}

{% api-method-parameter name="client\_secret" type="string" required=true %}
The OAuth clieint secret: `{client_secret}`
{% endapi-method-parameter %}

{% api-method-parameter name="email" type="string" required=true %}
Owner email address for my.teslamotors.com
{% endapi-method-parameter %}

{% api-method-parameter name="passowrd" type="string" required=true %}
Owner password for my.teslamotors.com
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Bearer access token successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{
  "access_token": "81527cff06843c8634fdc09e8ac0abefb46ac849f38fe1e431c2ef2106796384",
  "token_type": "bearer",
  "expires_in": 3888000,
  "refresh_token": "15mm312ysab7wxgsfzaz74oxxa2v9y2g3agu87oummhgb43dpuws0dwsbqjb431v",
  "created_at": 1532913622
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized access
{% endapi-method-response-example-description %}

```javascript
{
  "response": "authorization_required_for_txid_``}"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/oauth/revoke" %}
{% api-method-summary %}
Revoke
{% endapi-method-summary %}

{% api-method-description %}
Revokes the `{access_token}` issued by the token command
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="token" type="string" required=true %}
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

