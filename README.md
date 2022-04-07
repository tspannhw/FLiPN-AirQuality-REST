# FLiPN-AirQuality-REST
Apache NiFi, Apache Pulsar.   Air Quality Readings



### Example Read

````
bin/pulsar-client consume "persistent://public/default/airqualityglobal" -s aqrg-reader -n 0 -t Shared

----- got message -----
key:[5ac41180-38fe-42d7-92df-f5629421d719], properties:[], content:{"apigw-requestid":"QN4Ori9eoAMEJZA=","date":"Thu, 07 Apr 2022 15:45:46 GMT","country":"US","lastUpdated":"2022-04-07T05:05:19+00:00","unit":"particles/cm³","city":"","latitude":"37.82407","parameter":"um025","location":"Mountain Ave","server-timing":"total;dur=208.18","value":"0.04","longitude":"-122.22308"}
----- got message -----
key:[b9e5ca85-65aa-4592-adba-45eade4090b0], properties:[], content:{"apigw-requestid":"QN4Ori9eoAMEJZA=","date":"Thu, 07 Apr 2022 15:45:46 GMT","country":"US","lastUpdated":"2022-04-07T05:05:19+00:00","unit":"µg/m³","city":"","latitude":"37.109264","parameter":"pm10","location":"Adams Rd","server-timing":"total;dur=208.18","value":"18.5","longitude":"-121.91823"}

````
