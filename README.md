# CRC16-CRC16-CCIT-CRC32
CRC16-CRC16-CCIT-CRC32 algorithm javascript


CRC16_CCITT和C语言的一致
```javascript
  for (; i < buffData.length; i++) {
    // byte_val = charach[i].charCodeAt(0);
    // 这里直接使用Buffer
    // var buffData = new Buffer('0001A009030000000000000000', 'hex');
    byte_val = buffData[i];
```
