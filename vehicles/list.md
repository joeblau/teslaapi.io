# List

{% api-method method="get" host="https://owner-api.teslamotors.com" path="/api/1/vehicles" %}
{% api-method-summary %}
Vehicle List
{% endapi-method-summary %}

{% api-method-description %}
This endpoint retrieves the list of vehicles.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Bearer `{access_token}` response from authentication
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
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
      "id_s": ":ids",
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



