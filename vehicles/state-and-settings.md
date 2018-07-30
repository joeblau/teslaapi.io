# State And Settings

{% api-method method="get" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/data\_request/charge\_state" %}
{% api-method-summary %}
Charge State
{% endapi-method-summary %}

{% api-method-description %}
Charge state inforamtion including battery limit, charge miles, charge volate, charge phases, current, charge management, and battery heater status.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name=":id" type="integer" required=true %}
The vehicle `{id}` from the vehicle list response
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Charge state successful response.
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
Mobile Enabled
{% endapi-method-summary %}

{% api-method-description %}
Whether mobile access is enabled.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name=":id" type="integer" required=true %}
The vehicle `{id}` from the vehile list response
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Mobile enabled successful response..
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

{% api-method method="get" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/data\_request/climate\_state" %}
{% api-method-summary %}
Climate State
{% endapi-method-summary %}

{% api-method-description %}
Climate settings including seats, vents battery, steering wheel, and preconditioning state.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name=":id" type="integer" required=true %}
Vehicle `{id}` from vehicle list response
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Climate state successful response.
{% endapi-method-response-example-description %}

```javascript
{
  "response": {
    "inside_temp": null,
    "outside_temp": null,
    "driver_temp_setting": 18.3,
    "passenger_temp_setting": 18.3,
    "left_temp_direction": null,
    "right_temp_direction": null,
    "is_front_defroster_on": false,
    "is_rear_defroster_on": false,
    "fan_status": 0,
    "is_climate_on": false,
    "min_avail_temp": 15.0,
    "max_avail_temp": 28.0,
    "seat_heater_left": false,
    "seat_heater_right": false,
    "seat_heater_rear_left": false,
    "seat_heater_rear_right": false,
    "seat_heater_rear_center": false,
    "seat_heater_rear_right_back": 0,
    "seat_heater_rear_left_back": 0,
    "battery_heater": false,
    "battery_heater_no_power": null,
    "steering_wheel_heater": false,
    "wiper_blade_heater": false,
    "side_mirror_heaters": false,
    "is_preconditioning": false,
    "smart_preconditioning": false,
    "is_auto_conditioning_on": null,
    "timestamp": 1532926836621
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/data\_request/drive\_state" %}
{% api-method-summary %}
Drive State
{% endapi-method-summary %}

{% api-method-description %}
Drive state including latitude, longitude, and heading of the vehicle.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name=":id" type="integer" required=true %}
Vehicle `{id}` from vehicle list response
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Drive state successful response
{% endapi-method-response-example-description %}

```javascript
{
  "response": {
    "shift_state": null,
    "speed": null,
    "power": 0,
    "latitude": 40.459728,
    "longitude": -79.923447,
    "heading": 340,
    "gps_as_of": 1532927048,
    "native_location_supported": 1,
    "native_latitude": 40.459729,
    "native_longitude": -79.923444,
    "native_type": "wgs",
    "timestamp": 1532927316568
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/data\_request/gui\_settings" %}
{% api-method-summary %}
GUI Settings
{% endapi-method-summary %}

{% api-method-description %}
Localization settings inlcuding distance units, temperature units, charge units, and clock hour style.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name=":id" type="integer" required=true %}
Vehicle `{id}` from vehicle list response
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
GUI Settings successful response.
{% endapi-method-response-example-description %}

```javascript
{
  "response": {
    "gui_distance_units": "mi/hr",
    "gui_temperature_units": "F",
    "gui_charge_rate_units": "mi/hr",
    "gui_24_hour_time": false,
    "gui_range_display": "Rated",
    "timestamp": 1532927561350
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

