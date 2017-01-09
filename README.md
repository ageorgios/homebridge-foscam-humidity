# homebridge-foscam-humidity

This is a plugin for [homebridge](https://github.com/nfarina/homebridge) which makes it possible to create a humidity sensor
in HomeKit for Foscam Cameras that have humidity sensor.

# Information
The humidity is retrieved from the CGI API of Foscam Cameras.
```
http://hostname:port/cgi-bin/CGIProxy.fcgi?cmd=getHumidityState
```

## Example config

```json
{
  "accessory": "FoscamHumidity",
  "name": "Foscam Humidity Sensor",
  "description": "The humidity sensor from a Foscam P1 Camera",
  "hostname": "The hostname of the foscam camera",
  "port": "The port of the foscam camera",
  "username": "username of the foscam",
  "password": "password of the foscam"
}
```