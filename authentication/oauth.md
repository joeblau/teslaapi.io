# OAuth

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/oauth/token" %}

OAuth grant types supported

* `refresh_token`  
* `password`

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/oauth/revoke" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}
Revokes the `{access_token}` issued by the token command
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="" type="string" required=false %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
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

