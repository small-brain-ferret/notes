## Wheel Dimensions

| Parameter           | Value |
| ------------------- | ----- |
| Main wheel diameter | 70 mm |
| Main wheel radius   | 35 mm |
| Nose wheel diameter | 60 mm |
| Nose wheel radius   | 30 mm |

---

## Longitudinal Geometry

|Parameter|Value|How derived|
|---|---|---|
|CG station from nose datum|315 mm|Assumed 35% of 900 mm fuselage|
|Nose gear station from nose datum|80 mm|Clears nose contour|
|Main gear station from nose datum|356.5 mm|CG + Ma = 315 + 41.5|
|Wheelbase B|276.5 mm|Mf + Ma = 235 + 41.5|
|Mf — CG to nose gear|235 mm|315 − 80|
|Ma — CG to main gear|41.5 mm|Derived: upper bound of nose load range|

---

## Lateral Geometry

|Parameter|Value|How derived|
|---|---|---|
|Main gear track width|345.6 mm|2 × H\_CG / tan(38°)|
|Half-track width|172.8 mm|Track / 2|

---

## Vertical Geometry

| Parameter                        | Value  | How derived                                  |
| -------------------------------- | ------ | -------------------------------------------- |
| Main gear mount height           | 100 mm | Existing design                              |
| Nose gear mount height           | 105 mm | Leg\_h\_main + R\_main − R\_nose = 100 + 35 − 30 |
| Estimated CG height above ground | 135 mm | Leg\_h\_main + R\_main = 100 + 35               |

---

## Nose Gear Structural Dimensions

| Parameter                | Value  | How derived                 |
| ------------------------ | ------ | --------------------------- |
| Strut overall height     | 105 mm | Nose gear mount height      |
| Mounting plate length    | 60 mm  | Standard light UAV hardware |
| Mounting plate width     | 40 mm  | Standard light UAV hardware |
| Mounting plate thickness | 3 mm   |                             |

---

## Stability / Configuration Parameters

| Parameter               | Value | Raymer Requirement |
| ----------------------- | ----- | ------------------ |
| Nose gear load fraction | 15.0% | 8–15%              |
| Tipback angle           | 17.1° | > 15°              |
| Overturn angle          | 38.0° | < 63°              |
