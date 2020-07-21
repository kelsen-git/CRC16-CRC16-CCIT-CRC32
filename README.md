# CRC16-CCIT javascript
CRC16-CRC16-CCIT-CRC32 algorithm javascript


CRC16_CCITT和C语言的一致
```javascript
  for (; i < buffData.length; i++) {
    // byte_val = charach[i].charCodeAt(0);
    // 这里直接使用Buffer
    // var buffData = new Buffer('0001A0', 'hex');
    byte_val = buffData[i];
```

在返回之前添加
```javascript
    // 高低位互换，输出符合相关工具对Modbus CRC16的运算
    if (formatLow){
      crc = ((crc & 0xff00) >> 8) | ((crc & 0x00ff) << 8);
    }
```
