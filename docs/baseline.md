# GNSS-SDR Python Baseline

## Source

Branch: it4999-develop

Commit:
93d89669322d9b00a371944a6699a0927675b8c3

## Environment

OS: Ubuntu 24.04

Python: 3.13.14
NumPy: 2.5.3
SciPy: 1.18.1
Matplotlib: 3.11.1

## Dataset

Name:
GPSdata-DiscreteComponents-fs38_192-if9_55.bin

SHA256:
C5CA7CCF361D4C80BF5FA27E920D610919B9D9AD245450895C3D71AAD77A7325

File size:
1912602624 bytes

Signal:
GPS L1 C/A

File type:
Real samples

Data type:
int8

Sampling frequency:
38192000 Hz

Intermediate frequency:
9550000 Hz

Processing duration:
40000 ms

Skip samples:
0

Command:

python main.py -f="<path>" -s=38192000 -d=int8

## Acquisition

Acquired PRNs:

3, 6, 9, 15, 18, 21, 22, 26, 29

Number of acquired satellites:
9

Number of tracking channels:
8

Selected tracking PRNs:

21, 22, 15, 18, 26, 6, 9, 3

| Channel | PRN | Carrier frequency (Hz) | Doppler (Hz) | Code phase (samples) |
|---|---:|---:|---:|---:|
| 0 | 21 | 9547450 approx. | -2546 | 13403 |
| 1 | 22 | 9549740 approx. | -261 | 6287 |
| 2 | 15 | 9549950 approx. | -51 | 36320 |
| 3 | 18 | 9548270 approx. | -1727 | 20723 |
| 4 | 26 | 9545040 approx. | -4959 | 26826 |
| 5 | 6 | 9544340 approx. | -5660 | 28201 |
| 6 | 9 | 9550880 approx. | 877 | 4695 |
| 7 | 3 | 9549950 approx. | -51 | 34211 |

## Tracking

Tracking duration:
40000 ms

Tracked satellites:
8

Result:
PASS

Known baseline behavior:
Tracking is executed twice when no trackingResults_python.npy
cache exists.

## Navigation / PVT

Navigation:
PASS

PVT:
PASS

Navigation solution period:
500 ms

Mean position approximately:

Latitude:
40.00803 deg

Longitude:
-105.26269 deg

Height:
1630.4 m

Mean PDOP:
approximately 1.888877

## Known baseline issues

- probeData reports "unable to read file" despite raw-data plots
  and normal GNSS processing succeeding.
- Tracking is executed twice when tracking cache is absent.
- trackingResults_python.npy is a runtime cache and is not
  version-controlled.