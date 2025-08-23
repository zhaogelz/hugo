本机有公网ip6和域名的情况下，可以直接用ip6端口转发代理ip4，然后ip6绑定域名，通过域名：端口，访问本地  
将本地（192.168.3.8）通过ip6端口800代理  
netsh interface portproxy add v6tov4 listenport=8000 listenaddress=:: connectport=8000 connectaddress=192.168.3.8
 
[http://gw.15390974.xyz:8000/login](http://gw.15390974.xyz:8000/login)
 
不绑定域名，直接用ip6也行，需加方括号：  
[http://[2408:8270:824:9bd0:3479:1665:3169:2]:8000](http://[2408:8270:824:9bd0:3479:1665:3169:2]:8000)