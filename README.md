# Huawei S series switches extractor
Basic extractor for Huawei S series switches logs.

# Configuration

## Huawei switch

```
system-view
        info-center enable
        info-center loghost GRAYLOG_SERVER_IP log-counter disable port 5140
        info-center snmp channel 2
        info-center console channel 2
        info-center monitor channel 2
        info-center timestamp log date
        q
save
y
q
```

## GrayLog

Inputs - Syslog UDP

Port - 5140

# Examples
![image](https://github.com/volodinaleksey/GrayLog-Huawei-S-series-switches-extractor/assets/82817077/9f073707-c035-4ee8-9439-a3b2cdfc0cf8)
![image](https://github.com/volodinaleksey/GrayLog-Huawei-S-series-switches-extractor/assets/82817077/8dab50cc-32b6-45a6-8af1-456797e8e8ad)

# Bugs

Huawei adds extra space in dates:

![omage](https://github.com/volodinaleksey/GrayLog-Huawei-S-series-switches-extractor/assets/82817077/6ce048b8-8a75-463c-bc18-e86330a27c2d)


# URL
Huawei S series switches log messages format documentation:

https://support.huawei.com/enterprise/en/doc/EDOC1000174088/97342dce/log-message-format-description
