# Subscriptions

{% api-method method="get" host="https://owner-api.teslamotors.com" path="/api/1/vehicle\_subscriptions" %}
{% api-method-summary %}
Vehicle Subscriptions
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `{access_token}` from authorization
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name="device\_token" type="string" required=true %}
Sender device token
{% endapi-method-parameter %}

{% api-method-parameter name="device\_type" type="string" required=true %}
Subscription device type  
- `ios`  
- `android`
{% endapi-method-parameter %}

{% api-method-parameter name="bigint" type="boolean" required=true %}
`false`
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
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

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicle\_subscriptions" %}
{% api-method-summary %}
Vehicle Subscriptions
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `{access_token}` from authorization
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="device\_token" type="string" required=true %}
Sender device token
{% endapi-method-parameter %}

{% api-method-parameter name="device\_type" type="string" required=true %}
Subscription device type  
- `ios`  
- `android`
{% endapi-method-parameter %}

{% api-method-parameter name="vehicle\_subscriptions" type="array" required=true %}
`["1237331239112123"]`
{% endapi-method-parameter %}

{% api-method-parameter name="bigint" type="boolean" required=true %}
`false`
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
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

