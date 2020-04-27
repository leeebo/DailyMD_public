
## 程序烧录

```
esptool.py -p (PORT) -b 921600 write_flash --flash_mode dio --flash_size detect --flash_freq 40m 0x10000 bin/ESPlane2S2.bin 0x1000 bin/bootloader.bin 0x8000 bin/partition-table.bin
```

## 小飞机热点密码

SSID：ESPLANE_XXXX (XXXX根据 MAC 设置）
PASSWORD：12345678

## 注意事项

1. 请先确认电池正负！！
2. 电机 M1、M3 红线（白线）接正极，黑线接负极
3. 电机 M2、M4 红线（白线）接负极，黑线接正级
4. 注意 M1、M3 接 B 桨，注意 M2、M4 接 A 桨
5. 上电前后请置于平地，保持静止，将自动进行传感器校准
