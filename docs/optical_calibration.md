# Optical Calibration tutorial

## Calibrate with one Generation 1 Basestation:

`Note:` The Gen1 Lighthouse should be in mode "A" and no other Basestations should be in view

`Note:` The Device must be connected via USB for calibration

```
vrtrackingcalib.exe /bodycal ht_4p.json 800 200
```

## Calibrate with  one Generation 2 Basestation:

`Note:` The Device must be connected via USB for calibration

```
vrtrackingcalib.exe /usedisambiguation synconbeam /bodycal ht_4p.json 800 200
```

## Calibrate a device with some (no hits) Sensors

`Note:` The Device must be connected via USB for calibration

`Note:` This is not recommended for production and should only be used in prototypes where the defective sensor can not be repaired - Tracking Performance may suffer!

```
vrtrackingcalib.exe /deletemissingsensors /usedisambiguation synconbeam /bodycal ht_4p.json 800 200
```

