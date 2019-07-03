# State And Settings

{% api-method method="get" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/data" %}
{% api-method-summary %}
Vehicle Data \(Legacy\)
{% endapi-method-summary %}

{% api-method-description %}
All of the **legacy** vehicle data
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name=":id" type="integer" required=true %}
The vehicle `{id}` from the vehicle list
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `{access_token}` from authorization
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "response": {
    "id": :id,
    "user_id": :user_id,
    "vehicle_id": :vehicle_id,
    "vin": ":vin",
    "display_name": ":name",
    "option_codes": "AD15,AF02,AH00,APF0,APH2,APPA,AU00,BCMB,BP00,BR00,BS00,BTX4,CC02,CDM0,CH05,COUS,CW02,DRLH,DSH7,DV4W,FG02,FR01,GLFR,HC00,HP00,IDBO,INBPB,IX01,LP01,LT3B,MDLX,ME02,MI02,PF00,PI01,PK00,PMBL,QLPB,RCX0,RENA,RFPX,S02B,SP00,SR04,ST02,SU01,TIC4,TM00,TP03,TR01,TRA1,TW01,UM01,USSB,UTAB,WT20,X001,X003,X007,X011,X014,X021,X025,X026,X028,X031,X037,X040,X042,YFFC,SC05",
    "color": null,
    "tokens": [
      ":token1",
      ":token2"
    ],
    "state": "online",
    "in_service": null,
    "id_s": ":ids",
    "calendar_enabled": true,
    "backseat_token": null,
    "backseat_token_updated_at": null,
    "gui_settings": {
      "gui_distance_units": "mi/hr",
      "gui_temperature_units": "F",
      "gui_charge_rate_units": "mi/hr",
      "gui_24_hour_time": false,
      "gui_range_display": "Rated",
      "timestamp": 1532986218050
    },
    "vehicle_state": {
      "api_version": 3,
      "autopark_state": "unavailable",
      "autopark_state_v2": "standby",
      "autopark_style": "dead_man",
      "calendar_supported": true,
      "car_version": "2018.21.9 75bdbc11",
      "center_display_state": 0,
      "df": 0,
      "dr": 0,
      "ft": 0,
      "homelink_nearby": false,
      "last_autopark_error": "no_error",
      "locked": true,
      "notifications_supported": true,
      "odometer": 14522.605889,
      "parsed_calendar_supported": true,
      "pf": 0,
      "pr": 0,
      "remote_start": false,
      "remote_start_supported": true,
      "rt": 0,
      "sun_roof_percent_open": null,
      "sun_roof_state": "unknown",
      "timestamp": 1532986223303,
      "valet_mode": false,
      "vehicle_name": ":name"
    },
    "climate_state": {
      "inside_temp": 27.0,
      "outside_temp": 24.0,
      "driver_temp_setting": 18.3,
      "passenger_temp_setting": 18.3,
      "left_temp_direction": -280,
      "right_temp_direction": -280,
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
      "battery_heater_no_power": false,
      "steering_wheel_heater": false,
      "wiper_blade_heater": false,
      "side_mirror_heaters": false,
      "is_preconditioning": false,
      "smart_preconditioning": false,
      "is_auto_conditioning_on": false,
      "timestamp": 1532986223306
    },
    "charge_state": {
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
      "battery_range": 212.26,
      "est_battery_range": 152.09,
      "ideal_battery_range": 271.83,
      "battery_level": 83,
      "usable_battery_level": 83,
      "charge_energy_added": 16.57,
      "charge_miles_added_rated": 51.0,
      "charge_miles_added_ideal": 65.5,
      "charger_voltage": 0,
      "charger_pilot_current": 6,
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
      "charge_current_request": 6,
      "charge_current_request_max": 6,
      "managed_charging_active": false,
      "managed_charging_user_canceled": false,
      "managed_charging_start_time": null,
      "battery_heater_on": false,
      "not_enough_power_to_heat": false,
      "timestamp": 1532986223305
    },
    "drive_state": {
      "shift_state": null,
      "speed": null,
      "power": 0,
      "latitude": 40.459728,
      "longitude": -79.923447,
      "heading": 340,
      "gps_as_of": 1532986222,
      "native_location_supported": 1,
      "native_latitude": 40.459729,
      "native_longitude": -79.923444,
      "native_type": "wgs",
      "timestamp": 1532986223305
    },
    "vehicle_config": {
      "can_actuate_trunks": true,
      "car_special_type": "base",
      "car_type": "modelx",
      "charge_port_type": "US",
      "eu_vehicle": false,
      "exterior_color": "MetallicBlack",
      "has_ludicrous_mode": false,
      "motorized_charge_port": true,
      "perf_config": "P1",
      "plg": true,
      "rear_seat_heaters": 3,
      "rear_seat_type": 3,
      "rhd": false,
      "roof_color": "None",
      "seat_type": 0,
      "spoiler_type": "Passive",
      "sun_roof_installed": 0,
      "third_row_seats": "FuturisFoldFlat",
      "timestamp": 1532986223303,
      "trim_badging": "90d",
      "wheel_type": "AeroTurbine20"
    }
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/vehicle\_data" %}
{% api-method-summary %}
Vehicle Data
{% endapi-method-summary %}

{% api-method-description %}
All of the vehicle data
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name=":id" type="integer" required=true %}
The vehicle `{id}` from the vehicle list
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `{access_token}` from authorization
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "response": {
    "id": 45226696177987462,
    "user_id": 134950,
    "vehicle_id": 163057375,
    "vin": ":vin",
    "display_name": ":name",
    "option_codes": "AD15,AF02,AH00,APF0,APH2,APPA,AU00,BCMB,BP00,BR00,BS00,BTX4,CC02,CDM0,CH05,COUS,CW02,DRLH,DSH7,DV4W,FG02,FR01,GLFR,HC00,HP00,IDBO,INBPB,IX01,LP01,LT3B,MDLX,ME02,MI02,PF00,PI01,PK00,PMBL,QLPB,RCX0,RENA,RFPX,S02B,SP00,SR04,ST02,SU01,TIC4,TM00,TP03,TR01,TRA1,TW01,UM01,USSB,UTAB,WT20,X001,X003,X007,X011,X014,X021,X025,X026,X028,X031,X037,X040,X042,YFFC,SC05",
    "color": null,
    "tokens": [
      ":token1",
      ":token2"
    ],
    "state": "online",
    "in_service": false,
    "id_s": ":ids",
    "calendar_enabled": true,
    "api_version": 6,
    "backseat_token": null,
    "backseat_token_updated_at": null,
    "charge_state": {
      "battery_heater_on": false,
      "battery_level": 74,
      "battery_range": 186.57,
      "charge_current_request": 48,
      "charge_current_request_max": 48,
      "charge_enable_request": true,
      "charge_energy_added": 29.64,
      "charge_limit_soc": 90,
      "charge_limit_soc_max": 100,
      "charge_limit_soc_min": 50,
      "charge_limit_soc_std": 90,
      "charge_miles_added_ideal": 117.0,
      "charge_miles_added_rated": 91.5,
      "charge_port_cold_weather_mode": null,
      "charge_port_door_open": false,
      "charge_port_latch": "Engaged",
      "charge_rate": 0.0,
      "charge_to_max_range": false,
      "charger_actual_current": 0,
      "charger_phases": null,
      "charger_pilot_current": 48,
      "charger_power": 0,
      "charger_voltage": 0,
      "charging_state": "Disconnected",
      "conn_charge_cable": "<invalid>",
      "est_battery_range": 146.18,
      "fast_charger_brand": "<invalid>",
      "fast_charger_present": false,
      "fast_charger_type": "<invalid>",
      "ideal_battery_range": 238.93,
      "managed_charging_active": false,
      "managed_charging_start_time": null,
      "managed_charging_user_canceled": false,
      "max_range_charge_counter": 0,
      "not_enough_power_to_heat": false,
      "scheduled_charging_pending": false,
      "scheduled_charging_start_time": null,
      "time_to_full_charge": 0.0,
      "timestamp": 1558229319159,
      "trip_charging": false,
      "usable_battery_level": 74,
      "user_charge_enable_request": null
    },
    "climate_state": {
      "battery_heater": false,
      "battery_heater_no_power": false,
      "climate_keeper_mode": "off",
      "driver_temp_setting": 20.0,
      "fan_status": 0,
      "inside_temp": 29.0,
      "is_auto_conditioning_on": false,
      "is_climate_on": false,
      "is_front_defroster_on": false,
      "is_preconditioning": false,
      "is_rear_defroster_on": false,
      "left_temp_direction": -240,
      "max_avail_temp": 28.0,
      "min_avail_temp": 15.0,
      "outside_temp": 24.0,
      "passenger_temp_setting": 20.0,
      "remote_heater_control_enabled": false,
      "right_temp_direction": -240,
      "seat_heater_left": 0,
      "seat_heater_rear_left": 0,
      "seat_heater_rear_right": 0,
      "seat_heater_right": 0,
      "seat_heater_third_row_left": 0,
      "seat_heater_third_row_right": 0,
      "side_mirror_heaters": false,
      "smart_preconditioning": false,
      "steering_wheel_heater": false,
      "timestamp": 1558229319159,
      "wiper_blade_heater": false
    },
    "drive_state": {
      "gps_as_of": 1558229088,
      "heading": 163,
      "latitude": 40.459698,
      "longitude": -79.92347,
      "native_latitude": 40.459698,
      "native_location_supported": 1,
      "native_longitude": -79.92347,
      "native_type": "wgs",
      "power": null,
      "shift_state": null,
      "speed": null,
      "timestamp": 1558229319160
    },
    "gui_settings": {
      "gui_24_hour_time": false,
      "gui_charge_rate_units": "mi/hr",
      "gui_distance_units": "mi/hr",
      "gui_range_display": "Rated",
      "gui_temperature_units": "F",
      "timestamp": 1558229319160
    },
    "vehicle_config": {
      "can_accept_navigation_requests": true,
      "can_actuate_trunks": true,
      "car_special_type": "base",
      "car_type": "modelx",
      "charge_port_type": "US",
      "eu_vehicle": false,
      "exterior_color": "MetallicBlack",
      "has_air_suspension": true,
      "has_ludicrous_mode": false,
      "motorized_charge_port": true,
      "perf_config": "P1",
      "plg": true,
      "rear_seat_heaters": 3,
      "rear_seat_type": 3,
      "rhd": false,
      "roof_color": "None",
      "seat_type": 0,
      "spoiler_type": "Passive",
      "sun_roof_installed": 0,
      "third_row_seats": "FuturisFoldFlat",
      "timestamp": 1558229319160,
      "trim_badging": "90d",
      "wheel_type": "AeroTurbine20"
    },
    "vehicle_state": {
      "api_version": 6,
      "autopark_state_v2": "ready",
      "autopark_style": "dead_man",
      "calendar_supported": true,
      "car_version": "2019.12.1.1 4b1dd29",
      "center_display_state": 0,
      "df": 0,
      "dr": 0,
      "ft": 0,
      "homelink_nearby": false,
      "is_user_present": false,
      "last_autopark_error": "no_error",
      "locked": true,
      "media_state": {
        "remote_control_enabled": true
      },
      "notifications_supported": true,
      "odometer": 20101.093888,
      "parsed_calendar_supported": true,
      "pf": 0,
      "pr": 0,
      "remote_start": false,
      "remote_start_enabled": true,
      "remote_start_supported": true,
      "rt": 0,
      "sentry_mode": false,
      "software_update": {
        "expected_duration_sec": 2700,
        "status": ""
      },
      "speed_limit_mode": {
        "active": false,
        "current_limit_mph": 85.0,
        "max_limit_mph": 90,
        "min_limit_mph": 50,
        "pin_code_set": false
      },
      "sun_roof_percent_open": null,
      "sun_roof_state": "unknown",
      "timestamp": 1558229319158,
      "valet_mode": false,
      "vehicle_name": ":name"
    }
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/service\_data" %}
{% api-method-summary %}
Vehicle Service Data
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name=":id" type="integer" required=true %}
The vehicle `{id}` from the vehicle list
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `{access_token}` from authorization
{% endapi-method-parameter %}
{% endapi-method-headers %}
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

{% api-method method="get" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/data\_request/charge\_state" %}
{% api-method-summary %}
Charge State
{% endapi-method-summary %}

{% api-method-description %}
Charge state information including battery limit, charge miles, charge voltage, charge phases, current, charge management, and battery heater status.
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
Localization settings including distance units, temperature units, charge units, and clock hour style.
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

