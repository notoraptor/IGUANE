# IGUANE: A tool to explore Figures-of-Merit for some GPUs

Supported FoMs:
  - DRAC's [UGR/RGU](https://docs.alliancecan.ca/wiki/Allocations_and_compute_scheduling#Reference_GPU_Units)
  - My own proposal, IGUANE/IGUANA.

*Examples*:

    $ ./iguane.py -sr
     2.59 H100-SXM5-80GB
     2.43 H100-NVL-94GB
     1.96 H100-PCIe-80GB
     1.64 L40S
     1.00 A100-SXM4-80GB
     1.00 A100-PCIe-80GB
     0.90 A100-SXM4-40GB
     0.90 A100-PCIe-40GB
     0.81 A6000
     0.50 V100S-PCIe-32GB
     0.48 RTX8000
     0.46 V100-SXM2-32GB
     0.43 V100-PCIe-32GB
     0.42 V100-SXM2-16GB
     0.39 V100-PCIe-16GB
     0.27 P100-SXM2-16GB
     0.25 P100-PCIe-16GB
     0.22 P100-PCIe-12GB
     0.21 T4
    $ ./iguane.py -pd": "
    P100-PCIe-12GB: 0.22040341999886826
    P100-PCIe-16GB: 0.2539403974908297
    P100-SXM2-16GB: 0.2702130531251874
    V100-PCIe-16GB: 0.389666843190366
    V100-PCIe-32GB: 0.429666843190366
    V100-SXM2-16GB: 0.4169849414304501
    V100-SXM2-32GB: 0.4569849414304501
    V100S-PCIe-32GB: 0.49852085809099334
    T4: 0.2143220096336331
    RTX8000: 0.4784166837700395
    A100-PCIe-40GB: 0.9000000000000001
    A100-PCIe-80GB: 1.0
    A100-SXM4-40GB: 0.9000000000000001
    A100-SXM4-80GB: 1.0
    A6000: 0.8145228158992954
    L40S: 1.641054479943445
    H100-PCIe-80GB: 1.9579954847095848
    H100-SXM5-80GB: 2.586680957484816
    H100-NVL-94GB: 2.4280983913222136
    $ ./iguane.py -jsru rgu
    {
      "H100-SXM5-80GB": 12.168321513002363,
      "H100-NVL-94GB": 11.091546985815604,
      "L40S": 10.35952718676123,
      "H100-PCIe-80GB": 9.685106382978724,
      "A6000": 4.931631205673759,
      "A100-SXM4-80GB": 4.800000000000001,
      "A100-PCIe-80GB": 4.800000000000001,
      "A100-SXM4-40GB": 4.0,
      "A100-PCIe-40GB": 4.0,
      "RTX8000": 2.9685106382978725,
      "V100S-PCIe-32GB": 2.6535539795114267,
      "V100-SXM2-32GB": 2.5690780141843974,
      "V100-PCIe-32GB": 2.367344365642238,
      "V100-SXM2-16GB": 2.2490780141843976,
      "V100-PCIe-16GB": 2.047344365642238,
      "T4": 1.3223640661938536,
      "P100-SXM2-16GB": 1.2996690307328604,
      "P100-PCIe-16GB": 1.182505910165485,
      "P100-PCIe-12GB": 1.1025059101654848
    }
