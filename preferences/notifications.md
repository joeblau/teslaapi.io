# Notifications

{% api-method method="get" host="https://owner-api.teslamotors.com" path="/api/1/notification\_preferences" %}
{% api-method-summary %}
Notification Preferences
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `{access_token}` from authorization.
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name="locale" type="string" required=true %}
`en`
{% endapi-method-parameter %}

{% api-method-parameter name="device\_token" type="string" required=true %}
Sender device token
{% endapi-method-parameter %}

{% api-method-parameter name="device\_type" type="string" required=true %}
Notification subscriptoin device type  
- `ios`  
- `android`
{% endapi-method-parameter %}

{% api-method-parameter name="platfrom" type="string" required=true %}
Notificatoin subscriptoin platfrom  
- ios  
- android
{% endapi-method-parameter %}

{% api-method-parameter name="app\_version" type="number" required=true %}
App version sending notification
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

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/notification\_preferences" %}
{% api-method-summary %}
Notification Preferences
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `{access_token}` from authorization.
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="locale" type="string" required=true %}
`en`
{% endapi-method-parameter %}

{% api-method-parameter name="device\_token" type="string" required=true %}
Sender device token
{% endapi-method-parameter %}

{% api-method-parameter name="device\_type" type="string" required=true %}
Notifiaction subscriptoin device type  
- `ios`  
- `android`
{% endapi-method-parameter %}

{% api-method-parameter name="platform" type="string" required=true %}
Notification subscriptoin platfrom  
- `ios`  
- `android`
{% endapi-method-parameter %}

{% api-method-parameter name="app\_version" type="string" required=true %}
App version sending notification
{% endapi-method-parameter %}

{% api-method-parameter name="notification\_preferences" type="object" required=true %}
List of notification subscriptoins  
  
`{  
"alarm":true,  
"autopark_forward_started":true,  
"autopark_completed_success":true,  
"autopark_unavailable_plugged_in":true,  
"charging_started":true,  
"charging_interrupted":true,  
"charging_complete":true,  
"key_added":true,  
"key_removed":true,  
"update_available":true,  
"climate_keeper_ended_soc":true,  
"car_active":true,  
"refer_friend":true,  
"secret_level":true,  
"please_move_car":true,  
"grid_fault_contactor_trip":true,  
"grid_resync_success":true​  
}`  
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



