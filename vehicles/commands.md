# Commands

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/wake\_up" %}
{% api-method-summary %}
Wake Up
{% endapi-method-summary %}

{% api-method-description %}
Wake up the vehicle.
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
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Wake up command successful response.
{% endapi-method-response-example-description %}

```javascript
{
  "response": [
    {
      "id": :id,
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
      "id_s": ":id",
      "calendar_enabled": true,
      "backseat_token": null,
      "backseat_token_updated_at": null
    }
  ],
  "count": 1
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/door\_unlock" %}
{% api-method-summary %}
Unlock Doors
{% endapi-method-summary %}

{% api-method-description %}
Unlock doors of the vehicle
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
Bearer `{access_token}` from authentication
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
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/door\_lock" %}
{% api-method-summary %}
Lock Doors
{% endapi-method-summary %}

{% api-method-description %}
Lock the doors of the vehicle
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
Bearer `{access_token}` from authentication
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
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/honk\_horn" %}
{% api-method-summary %}
Honk Horn
{% endapi-method-summary %}

{% api-method-description %}
Honks the horn of the vehicle once
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
Bearer `{access_token}` from authentication
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
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/flash\_lights" %}
{% api-method-summary %}
Flash Lights
{% endapi-method-summary %}

{% api-method-description %}
Flashes the lights of the vehicle once
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
Bearer `{access_token}` from authentication
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
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/auto\_conditioning\_start" %}
{% api-method-summary %}
Start HVAC System
{% endapi-method-summary %}

{% api-method-description %}
Start vehicle climate control system. The vehicle will automatically determine whether to **heat** or **cool** based on set temperature.
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
Bearer `{access_token}` from authentication
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
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/auto\_conditioning\_stop" %}
{% api-method-summary %}
Stop HVAC System
{% endapi-method-summary %}

{% api-method-description %}
Stop vehicle climate control system.
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
Bearer `{access_token}` from authentication
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
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/set\_temps?driver\_temp=:driver\_temp&passenger\_temp=:passenger\_temp" %}
{% api-method-summary %}
Set Temperature
{% endapi-method-summary %}

{% api-method-description %}
Set vehicle HVAC temperature
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
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name=":driver\_temp" type="number" required=true %}
Desired driver temperature in Celsius
{% endapi-method-parameter %}

{% api-method-parameter name=":passenger\_temp" type="number" required=true %}
Desired passenger temperature in Celsius
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "response": {
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/set\_charge\_limit?percent=:limit\_value" %}
{% api-method-summary %}
Set Charge Limit
{% endapi-method-summary %}

{% api-method-description %}
Set vehicle charge limit
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
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name=":limit\_value" type="number" required=true %}
Percentage of charge to set the vehicle to
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "response": {
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/charge\_max\_range" %}
{% api-method-summary %}
Set Max Range Charge Limit
{% endapi-method-summary %}

{% api-method-description %}
Set vehicle to max charge limit
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
Bearer `{access_token}` from authentication
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
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/charge\_standard" %}
{% api-method-summary %}
Set Standard Charge Limit
{% endapi-method-summary %}

{% api-method-description %}
Set vehicle to standard charge limit
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
Bearer `{access_token}` from authentication
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
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/sun\_roof\_control?state=:state&percent=:percent" %}

* `open` - 100%  
* `closed` - 0%  
* `comfort` - 80%  
* `vent` - 15%  
* `move` - specify {percent}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/actuate\_trunk" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}
Open vehicles trunk or frunk. Call endpoint again to close trunk.
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

```javascript
{
  "response": {
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/remote\_start\_drive?password=:password" %}
{% api-method-summary %}
Remote Start Drive
{% endapi-method-summary %}

{% api-method-description %}
Start vehicle key-less driving mode. The vehicle must be placed in drive within 2 minutes of the response.
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
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name=":password" type="string" required=true %}
Password credentials for my.teslamotors.com
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "response": {
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/charge\_port\_door\_open" %}
{% api-method-summary %}
Open Charge Port
{% endapi-method-summary %}

{% api-method-description %}
Opens vehicle charge port. Also unlocks the charge port if it is locked.
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
Bearer `{access_token}` from authentication
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
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/charge\_port\_door\_close" %}
{% api-method-summary %}
Close Charge Port
{% endapi-method-summary %}

{% api-method-description %}
Closes vehicle charge port.
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
Bearer `{access_token}` from authentication
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
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/charge\_start" %}
{% api-method-summary %}
Start Charging
{% endapi-method-summary %}

{% api-method-description %}
Starts vehicle charging. Vehicle must be plugged in, have power available, and not at charge limit.
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
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name="PARAM\_NAME" type="string" required=true %}
PARAM\_DESC
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "response": {
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/charge\_stop" %}
{% api-method-summary %}
Stop Charging
{% endapi-method-summary %}

{% api-method-description %}
Stop vehicle charging. Vehicle must be charging.
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
Bearer `{access_token}` from authentication
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
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/upcoming\_calendar\_entries" %}
{% api-method-summary %}
Upcoming Calendar Entries
{% endapi-method-summary %}

{% api-method-description %}
Set upcoming calendar entries
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
Bearer `{access_token}` from authentication
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
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/set\_valet\_mode?on=:on&password=:password" %}
{% api-method-summary %}
Set Valet Mode
{% endapi-method-summary %}

{% api-method-description %}
Set vehicle valet mode on or off with a PIN to disable it from within the car. Reuses last PIN from previous valet session. Valet Mode limits the car's top speed to 70MPH and 80kW of acceleration power. It also disables Homelink, Bluetooth and Wifi settings, and the ability to disable mobile access to the car. It also hides your favorites, home, and work locations in navigation.
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
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name=":on" type="boolean" required=true %}
Enable or disable valet mode
{% endapi-method-parameter %}

{% api-method-parameter name=":password" type="string" required=true %}
Four digit pin for valet mode
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "response": {
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/reset\_valet\_pin" %}
{% api-method-summary %}
Reset valet PIN
{% endapi-method-summary %}

{% api-method-description %}
Resets vehicle valet PIN
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
Bearer `{access_token}` from authentication
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
    "result": true,
    "reason": ""
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/speed\_limit\_activate" %}
{% api-method-summary %}
Speed Limit Activate
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
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}
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

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/speed\_limit\_deactivate" %}
{% api-method-summary %}
Speed Limit Deactivate
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
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}
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

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/speed\_limit\_set\_limit" %}
{% api-method-summary %}
Speed Limit Set Limit
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
Bearer `{access_token}` from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}
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

{% api-method method="post" host="https://owner-api.teslamotors.com" path="/api/1/vehicles/:id/command/speed\_limit\_clear\_pin" %}
{% api-method-summary %}
Speed Limit Clear PIN
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name=":id" type="number" required=true %}
The vehicle `{id}` from the vehicle list
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

{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

