# KoiShi-Bot <small>`only for wibusBot`</small>

> Some Bot Script, Built with TypeScript, Power by KoiShi

## GitHub Hook

The official Plugin: `koishi-plugin-github` has some unexpected error. when i try to fix them, i can do nothing with this.

This Script still use OAuth App. Please create a oauth app first.

- **appID**: string
- **appSecret**: string
- **message** ?: string

## UTM output

This script only use for UTM groups. It can echo some url about UTM.

```bash
# if you input "UTM相关链接"
# Script will output
@starter, This are some url about UTM:
1. https://getutm.app/ | UTM official
2. https://github.com/utmapp/UTM | GitHub Repo
3. https://testflight.apple.com/join/yAy7ZyZx | UTM SE
4. https://testflight.apple.com/join/J9lKqdEN | Jitterbug
5. https://blog.jrcloud.vip/index.php/archives/95/ | QEMU For jb
```

`@starter` is this topic starter, ~~the list can get from json:~~(it is a failed project)

```json
{
  "title": "This are some url about UTM: "
}
```

## Ping & WebScript

It is a common script, for webmaster, you can use it like this: `ping <url>`

```bash
# user:
ping baidu.com
# Bot return: 
PING baidu.com (220.181.38.251): 56 data bytes
64 bytes from 220.181.38.251: icmp_seq=0 ttl=53 time=36.095 ms
64 bytes from 220.181.38.251: icmp_seq=1 ttl=53 time=36.252 ms
64 bytes from 220.181.38.251: icmp_seq=2 ttl=53 time=37.274 ms
64 bytes from 220.181.38.251: icmp_seq=3 ttl=53 time=36.369 ms
--- baidu.com ping statistics ---
4 packets transmitted, 4 packets received, 0.0% packet loss
round-trip min/avg/max/stddev = 36.095/36.498/37.274/0.459 ms
```

> More WebScript are thinking...

## Search

It can find some information on the Internet, and echo the Text

- **platform**,  `Baidu` | `Google`(require Internet environment) | `Sugou`
- **message** : string, for echo the font of Test msg

