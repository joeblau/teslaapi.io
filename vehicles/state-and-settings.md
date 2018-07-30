---
description: State and settings of the Vehicle
---

# State And Settings

{% api-method method="get" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/data\_request/charge\_state" %}
{% api-method-summary %}
Get Charge State
{% endapi-method-summary %}

{% api-method-description %}
This endpoint retrieves the charge state and battery information from your vehicle.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name=":id" type="string" required=true %}
The vehicle id from the vehicle list response
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `access_token` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Charge state successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{
  "response": {
    "charging_state": "Complete",
    "fast_charger_type": "\u003cinvalid\u003e",
    "fast_charger_brand": "\u003cinvalid\u003e",
    "charge_limit_soc": 86,
    "charge_limit_soc_std": 90,
    "charge_limit_soc_min": 50,
    "charge_limit_soc_max": 100,
    "charge_to_max_range": false,
    "max_range_charge_counter": 0,
    "fast_charger_present": false,
    "battery_range": 219.06,
    "est_battery_range": 157.1,
    "ideal_battery_range": 280.53,
    "battery_level": 86,
    "usable_battery_level": 86,
    "charge_energy_added": 18.77,
    "charge_miles_added_rated": 58.0,
    "charge_miles_added_ideal": 74.0,
    "charger_voltage": 0,
    "charger_pilot_current": 7,
    "charger_actual_current": 0,
    "charger_power": 0,
    "time_to_full_charge": 0.0,
    "trip_charging": false,
    "charge_rate": 0.0,
    "charge_port_door_open": true,
    "conn_charge_cable": "SAE",
    "scheduled_charging_start_time": null,
    "scheduled_charging_pending": false,
    "user_charge_enable_request": null,
    "charge_enable_request": true,
    "charger_phases": null,
    "charge_port_latch": "Engaged",
    "charge_current_request": 7,
    "charge_current_request_max": 7,
    "managed_charging_active": false,
    "managed_charging_user_canceled": false,
    "managed_charging_start_time": null,
    "battery_heater_on": false,
    "not_enough_power_to_heat": false,
    "timestamp": 1532915238524
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/mobile\_enabled" %}
{% api-method-summary %}
Get Mobile Access State
{% endapi-method-summary %}

{% api-method-description %}
This endpoint retrieves the mobile access availiblity state
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name=":id" type="string" required=true %}
The vehicle id from the vehile list response
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `access_token` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Mobile access state successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{
  "response": true
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



