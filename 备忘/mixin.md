mixin:
dns:
enable: true
default-nameserver:
 223.5.5.5
 1.1.1.1
enhanced-mode: redir-host
nameserver:
 223.5.5.5
 223.6.6.6
 https://223.5.5.5/resolve
fallback:
 1.1.1.1
 208.67.220.222:5353
 https://dns.rubyfish.cn/dns-query
 https://doh.opendns.com/dns-query
 tls://1.1.1.1:853
fallback-filter:
geoip: true
tun:
       enable: true
       stack: gvisor
       dns-hijack:
              198.18.0.2:53
auto-route: true
auto-detect-interface: true