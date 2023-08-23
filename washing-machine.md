![Washing Machine](pictures/iot-machine.png)

## Get hardware level operations e.g. wash_count
```
Topic: v1/hw/get/6310301016/model-01/WSH-SN001
Payload: {
    "action"    : "get",
    "project"   : "6310301016",
    "model"     : "model-01",
    "serial"    : "WSH-SN01",
    "name"      : "wash_count",
    "value"     : "120"
}
```

## Get firmware version
```
Topic: v1/hw/get/6310301016/model-01/WSH-SN001
Payload: {
    "action"    : "get",
    "project"   : "6310301016",
    "model"     : "model-01",
    "serial"    : "WSH-SN01",
    "name"      : "get firmware",
    "value"     : "19"
}
```

## Get manufacture id and geo-location or location placement
```
Topic: v1/hw/get/6310301016/model-01/WSH-SN001
Payload: {
    "action"    : "get",
    "project"   : "6310301016",
    "model"     : "model-01",
    "serial"    : "WSH-SN01",
    "name"      : "manufacture id",
    "value"     : "A"
}

Payload: {
    "action"    : "get",
    "project"   : "6310301016",
    "model"     : "model-01",
    "serial"    : "WSH-SN01",
    "name"      : "location",
    "value"     : "Bangkok"
}
```

## Set geo-location or location placement
```
Topic: v1/hw/set/6310301016/model-01/WSH-SN001
Payload: {
    "action"    : "set",
    "project"   : "6310301016",
    "model"     : "model-01",
    "serial"    : "WSH-SN01",
    "name"      : "location",
    "value"     : "Kanchanaburi"
}
```

## Monitor machine sensor
```
Topic: v1/hw/monitor/6310301016/model-01/WSH-SN001
Payload: {
"action"    : "monitor",
    "project"   : "6310301016",
    "model"     : "model-01",
    "serial"    : "WSH-SN01",
    "name"      : "Vibration Sensor",
    "value"     : "140"
}
```

## Set machie status to "maint" to indicate this machine need to be maintenance.
```
Topic: v1/hw/set/6310301016/model-01/WSH-SN001
Payload: {
"action"    : "set",
    "project"   : "6310301016",
    "model"     : "model-01",
    "serial"    : "WSH-SN01",
    "name"      : "status",
    "value"     : "main"
}
```
