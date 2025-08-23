{  
"servers": [  
{  
"address": "udp://1.1.1.1",  
"addresses": ["1.0.0.1", "8.8.8.8"],  
"domains": ["geosite:geolocation-!cn"],  
"expectIPs": ["geoip:!cn","geoip:netflix"],  
"clientSubnet": "1.1.1.0/24",  
"cache_ttl": 600  
},  
{  
"address": "udp://223.5.5.5",  
"addresses": ["223.6.6.6", "119.29.29.29"],  
"domains": ["geosite:cn"],  
"expectIPs": ["geoip:cn","geoip:private"],  
"clientSubnet": "114.114.114.0/24",  
"cache_ttl": 3600  
}  
],  
"retries": 2,  
"timeout": "3s"  
}