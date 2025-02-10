# 2023 Computer Specs


# Overview

\* *Indicates the price of an item I had previously purchased*

| Component | Power | Max Temperature | Price | (Previously<br>Purchased<br>Price*) |
| --- | ---: | ---: | ---: | ---: |
| [CPU](#cpu) | 120 W | 89°C | $358.99 | |
| [Motherboard](#motherboard) | ~195 W | -- | $199.99 | |
| [CPU Cooler](#cpu-cooler) | 5 W | -- | $35.47 | |
| [Thermal Paste/Pad](#thermal-pastepad) | -- | -- | $25.99 | |
| [Memory](#memory) | ~30 W | ~95°C | $204.99 | |
| [Graphics](#graphics) | 170 W | 93°C | -- | ($359.99*) |
| [Storage](#storage) | ~10 W | 85°C | $229.99 | |
| [Case](#case) | 20 W | -- | $189.99 | |
| [Fan Controller/Hub/Splitter](#fan-controllerhubsplitter) | -- | -- | $5.95 | |
| [Power Supply](#power-supply) | +750 W | -- | $99.99 | |
| **Total** | **550 W**<br>(200 W headroom) | -- | **$1351.35** | **($1711.34\*)** |

(PCPartPicker estimated 489 W and Newegg PC Builder estimated 570 W. Newegg
Power Supply Calculator suggested a PSU with 600-699 W.)

| Software | Price |
| --- | ---: |
| [Operating System](#operating-system) | $199.99 |
| **Total** | **$199.99** |

| Peripherals | Price | (Previously<br>Purchased<br>Price*) |
| --- | ---: | ---: |
| [Dell U2311H](#monitors) | -- | ($279.00*) | |
| [Dell U2311H](#monitors) | -- | ($279.00*) | |
| [TODO: New Monitor](#monitors) | $TODO | |
| [TODO: New Keyboard](#keyboard) | $TODO | |
| [TODO: New Mouse](#mouse) | $TODO | |
| [TODO: New Mouse Pad](#mouse-pad) | $TODO | |
| [Speakers](#speakers) | $34.99 | |
| **Total** | **$34.99** | **($592.99\*)** |

| Tools | Price |
| --- | ---: |
| [Precision Screwdriver Set](#tools) | $31.19 |
| [Electric Air Duster](#tools) | $39.95 |
| **Total** | **$71.14** |


# Components

## CPU
- **Product:**
  [AMD Ryzen 7 7800X3D](https://www.amd.com/en/products/apu/amd-ryzen-7-7800x3d)
- **Price:**
  [$358.99](https://www.newegg.com/amd-ryzen-7-7800x3d-ryzen-7-7000-series/p/N82E16819113793)
- **Power:**
  - Best estimate: 120 W
    - The Default Thermal Design Power (TDP) is 120 W
  - PCPartPicker: 15-162 W
- **Max Temperature:** 89°C (TJMax)
- **Features:**
  - Socket: AM5
  - Cores/Threads: 8-Core, 16-Thread
  - Operating Frequency: 4.2 GHz
  - Max Turbo Frequency: 5.0 GHz
  - Cache: 512 KB L1, 8 MB L2, 96 MB L3
  - RAM Support: 2x DDR5-5200 or 4x DDR5-3600
- **Reviews:**
  - [Gamers Nexus: AMD Ryzen 7 7800X3D CPU Review & Benchmarks](https://www.youtube.com/watch?v=B31PwSpClk8)
  - [Gamers Nexus: AMD Ryzen 7 2700X in 2023: Benchmarks vs. 5800X3D, 7800X3D, & More CPU Upgrades](https://www.youtube.com/watch?v=cKgDrW5H5go)
- **Thoughts:**
  - The only use case where I need high-performance CPU is gaming
  - All of the Intel CPUs are very high in power/heat right now
  - The AMD Ryzen 9 7900X3D and AMD Ryzen 9 7950X3D require parking half the CPU
    cores during gaming, otherwise you won't get good performance (and this is
    triggered by the Windows/Xbox Game Bar, which must be installed). None of
    this sounds like something I want to deal with.
  - The AMD 7900X and AMD 7950X aren't as high-power as Intel, but still much
    higher than the X3D variants (which have lower clock speeds but bigger
    caches and tend to perform better in games, but worse in productivity tasks)
- **Hindsight:** No regrets so far...

## Motherboard
- **Product:**
  [ASUS TUF Gaming B650-PLUS WiFi](https://www.asus.com/us/motherboards-components/motherboards/tuf-gaming/tuf-gaming-b650-plus-wifi)
- **Price:**
  [$199.99](https://smile.amazon.com/ASUS-TUF-B650-PLUS-Motherboard-Ethernet/dp/B0BHN7GGBQ)
- **Power:**
  - Best estimate: ~195 W
    - I couldn't find any official documentation on the power consumption of the
      motherboard. The closest thing I found was a
      [review](https://www.guru3d.com/review/asus-tuf-gaming-b650-plus-wifi-review/page-5)
      that benchmarked 198 W under multi-thread load for the entire PC
      (including memory, SSD, etc.). Subtracting 105 W for the
      [7700X](https://www.amd.com/en/products/cpu/amd-ryzen-7-7700x) used in the
      test gives 93 W. So I'm using ~90 W as an estimate for the motherboard
      itself. Obviously this is far from perfect, but hopefully it's a
      reasonable estimate.
    - I'm also going to be conservative and add ~105 W for USB peripherals
      (7.5 W * 8 Type-A ports + 15 W * 3 Type-C ports = 105 W)
  - PCPartPicker: 17-70 W
- **Max Temperature:** N/A (I couldn't find any official documentation on
  temperatures for any of the various motherboard components)
- **Features:**
  - CPU: AM5 for AMD Ryzen 7000 Series
  - Chipset: B650
  - Memory: DDR5, 4xDIMM, Max 128GB, Dual Channel, AMD EXPO
    - Memory Speeds: 7600+(OC) / 7200(OC) / 7000(OC) / 6800(OC) / 6600(OC) /
      6400(OC) / 6200(OC) / 6000(OC) / 5800(OC) / 5600(OC) / 5400(OC) / 5200 /
      5000/ 4800
  - Graphics:
    - 1x DisplayPort
    - 1x HDMI
  - Expansion Slots:
    - CPU:
      - 1x PCIe 4.0/3.0 x16
    - Chipset:
      - 1x PCIe 4.0/3.0 x16
      - 2x PCIe 4.0/3.0 x1
  - Storage:
    - CPU:
      - 1x M.2 (2242/2260/2280 Key M) PCIe 5.0 x4
      - 1x M.2 (2242/2260/2280/22110 Key M) PCIe 4.0 x4
    - Chipset:
      - 1x M.2 slot (2242/2260/2280 Key M) PCIe 4.0 x4 (exclusive with chipset
        PCIe x16)
      - 4x SATA 6 Gb/s
  - Connectivity:
    - Ethernet: 1x Realtek 2.5 Gb
    - WiFi: 2x2 Wi-Fi 6 (802.11 a/b/g/n/ac/ax)
    - Bluetooth: v5.2
  - USB:
    - Rear:
      - 1x Type-C (USB 3.2 Gen 2x2)
      - 1x Type-C (USB 3.2 Gen 2)
      - 2x Type-A (USB 3.2 Gen 2)
      - 4x Type-A (USB 2.0)
    - Internal:
      - 1x Type-C connector (USB 3.2 Gen 1)
      - 1x header (USB 3.2 Gen 1, supports 2 ports)
      - 2x header (USB 2.0, supports 4 ports)
  - Audio: Realtek 7.1 Surround Sound High Definition Audio
    - Rear: 5x audio jacks
    - Front: 1x front panel audio header (AAFP)
  - Fan headers:
    - 1x 4-pin CPU
    - 1x 4-pin CPU OPT
    - 1x 4-pin AIO pump
    - 4x 4-pin chassis
  - Power headers:
    - 1x 24-pin main power
    - 1x 8-pin +12V
    - 1x 4-pin +12V
  - Misc:
    - 1x Thunderbolt (USB4) header
    - 1x COM port
    - 1x BIOS FlashBack button (rear)
    - 1x clear CMOS header
    - 4x Q-LEDs (diagnostic LEDs: CPU, DRAM, VGA, booting devices)
    - 1x 20-3 pin system panel header
    - RGB LED headers:
      - 3x Addressable Gen 2
      - 1x Aura RGB
- **Reviews:**
  - [Hardware Unboxed: AMD B650 Roundup: 35 Motherboards Tested, Complete Buying Guide](https://www.youtube.com/watch?v=ZtHOOyWYiic)
  - [PC Builder: Best Ryzen Motherboard 2023 - Ryzen 7000 & 5000 CPUs (5600X, 7600X, 7800X3D & More)](https://www.youtube.com/watch?v=VL9UkQbPzyw)
- **Thoughts:**
  - In my experience, Gigabyte and MSI have always been very hit-or-miss while
    ASRock and ASUS are usually pretty solid
  - The benefits of the X670 chipset (overclockable CPU, more PCIe lanes, and
    more USB/SATA bandwidth) don't outweigh the current costs
  - The ASUS ROG Strix B650-A is also currently on sale for $199.99 and is
    technically a better motherboard (better audio codec and an extra USB 3.2
    Gen 2 port), but...
    - It has Intel-based ethernet. Intel has been having issues with their
      ethernet controllers (particularly the I225-V and I226-V). The last thing
      I want is to have to deal with ethernet issues, so I'm opting to stick
      with Realtek-based controllers.
    - It's white (including the back panel) and everything else (including my
      case) is black
- **Hindsight:** No regrets so far...

## CPU Cooler
- **Product:**
  [Thermalright Peerless Assassin 120 Black](https://www.thermalright.com/product/peerless-assassin-120-black)
- **Price:**
  [$35.47](https://smile.amazon.com/Thermalright-Peerless-Assassin-Aluminium-Technology/dp/B09S3BGN6M)
- **Power:**
  - Best estimate: 5 W
    - The specs say 0.20 A for the
      [TL-C12-B](https://www.thermalright.com/product/tl-c12-b) fans, so I'm
      estimating ~5 W (2 fans * 12 V * 0.2 A = 4.8 W total).
  - PCPartPicker: 5-10 W
- **Max Temperature:** N/A
- **Features:** N/A
- **Reviews:**
  - [Gaming Nexus: The Champ: $41 Thermalright Peerless Assassin CPU Cooler Review & Benchmarks](https://www.youtube.com/watch?v=Mm4hyIHe1PM)
  - More recent charts:
    - [Gaming Nexus: 2023-07-21](https://www.youtube.com/watch?v=ukYhjjoJnfc)
    - [Gaming Nexus: 2023-08-01](https://www.youtube.com/watch?v=IpTV6-d2tnQ)
  - 120 vs 120 SE:
    - [Jack's Hardware: Thermalright Peerless Assassin 120 vs Peerless Assassin 120 SE](https://www.youtube.com/watch?v=g4oqxMckR1M)
    - [PC Analytics: Review: Peerless Assassin 120 vs 120 SE](https://www.youtube.com/watch?v=M4AAqbv4m1A)
- **Thoughts:**
  - The 120 seems to have better clearance than the 120 SE (for tall RAM heat
    sinks/spreaders)
  - I prefer the appearance of the flat top of the 120 (as opposed to the tubes
    sticking out of the 120 SE)
- **Hindsight:**
  - The fan closest to the RAM can't be mounted all the way down because it
    would hit the RAM heat sinks/spreaders. But I don't think it's too bad. And
    I think that this would probably be an issue with just about any air cooler
    / motherboard combo.

## Thermal Paste/Pad
- **Product:**
  [Thermal Grizzly KryoSheet](https://www.thermal-grizzly.com/en/products/625-kryosheet-en)
- **Price:**
  [$25.99](https://smile.amazon.com/Thermal-Grizzly-KryoSheet-33/dp/B0C61Q77B6)
- **Power:** N/A
- **Max Temperature:** N/A
- **Features:**
  - Thermal conductivity similar to high-performance thermal paste
  - Won't dry out like thermal paste
- **Reviews:**
  - [JayzTwoCents: Cooling CPUs will never be the same after using this!](https://www.youtube.com/watch?v=pTRk52LpRco)
  - [Gamers Nexus: CPU Thermal Issues & Der8auer's Scientific Solutions | Graphene, Direct Die Blocks, & More](https://www.youtube.com/watch?v=k9TH7TeDZM8)
  - [Hardware Unboxed: Hands On With AM5 Direct-Die Cooling & GPU Power Monitoring Tools, feat Thermal Grizzly (der8auer)](https://www.youtube.com/watch?v=v6PfZ9CJVUg)
- **Thoughts:**
  - I never bother to replace my thermal paste (although I do monitor the
    temperature of my CPU, so I suppose I would if temperature became a
    problem), so something that never needs to be replaced sounds nice
  - Graphene is cool (ha!). But seriously, graphene has a lot of very
    interesting properties as a material, so it's nice to see that we've figured
    out how to manufacture enough of it to make a real product.
  - After building the PC,
- **Hindsight:**
  - The graphene pad was flakier than I expected. I don't think it's an issue,
    it's just weird to open the box and see little flakes of it just sitting
    there.
  - The graphene pad is very light, so it was hard to get it to stay put while
    attaching the CPU cooler. Perhaps a drop of liquid could have helped keep it
    in place momentarily. Maybe something very pure that will evaporate (e.g.,
    distilled water) or a drop of thermal paste might work, but I haven't tried
    either of these and there might be reasons not to. More research would be
    prudent.

## Memory
- **Product:**
  [G.SKILL Trident Z5 Neo (F5-6000J3238G32GX2-TZ5N)](https://www.gskill.com/product/165/393/1665020484/F5-6000J3238G32GX2-TZ5N)
- **Price:**
  [$204.99](https://www.newegg.com/g-skill-64gb/p/N82E16820374442)
- **Power:**
  - Best estimate: ~30 W (this
    [video](https://www.youtube.com/watch?v=qOWiwwi7A1g&t=540s) shows one DIMM
    of DDR5-5400 CL38 consuming ~8 W, so I'll give a conservative estimate of
    ~15 W per DIMM for a total estimate of ~30 W)
  - PCPartPicker: 62W (this seems high)
- **Max Temperature:** ~95°C (according to
  [Corsair's FAQ](https://help.corsair.com/hc/en-us/articles/4411158154381-DDR5-RAM-FAQ),
  "the operating temperature for DDR5 is between 0-95 degrees Celsius")
- **Features:**
  - 64 GB (2x 32 GB)
  - DDR5
  - 6000 MT/s
  - CL32-38-38-96
- **Reviews:**
  - [ASUS Memory Support](https://www.asus.com/us/motherboards-components/motherboards/tuf-gaming/tuf-gaming-b650-plus-wifi/helpdesk_qvl_cpu)
  - [G.SKILL QVL](https://www.gskill.com/qvl/165/393/1665020484/F5-6000J3238G32GX2-TZ5N-QVL)
  - [Linus Tech Tips: Does RAM Speed REALLY Matter?? (DDR5 Edition)](https://www.youtube.com/watch?v=b-WFetQjifc)
- **Thoughts:**
  - People have been having issues with RAM on newer AMD machines, particularly
    at speeds above 6400 MT/s, so it's probably best to stick with RAM on the
    qualified vendor lists (both from the motherboard manufacturer and the RAM
    manufacturer)
  - I went with the highest speed on the ASUS QVL that met my requirements (see
    below). That turned out to be G.SKILL, which is a good brand.
    - I need to actually find it for sale in a 2x32 GB configuration (ideally
      without RGB lights)
      - My 2012 computer has 32 GB of RAM, so I'd feel bad if I didn't get at
        least 64 GB
      - 2 DIMMs will generally perform better than 4 DIMMs (but it may cost more
        and/or offer less total RAM)
    - Ideally it supports EXPO (since that's AMD's version of XMP; XMP should
      also work, but due to the issues mentioned above, it seems safer to go
      with AMD's version)
- **Hindsight:**
  - Figuring out whether to use EXPO I or EXPO II or EXPO Tweaked was annoying
    (see **Ai Tweaker > Ai Overclock Tuner** in
    [2023 Computer Configuration#BIOS Settings](configuration.md#bios-settings))
  - Apparently despite AMD advertising EXPO, using overclocked memory can void
    the warranty on your CPU. Oh well.
  - I think that if I were going to buy new RAM, I'd try to find some
    non-overclocked DDR5-5200 (i.e., the "default SPD" / "default JEDEC" speed
    of 5200 MT/s) since that's the max speed supported by the CPU according to
    the specs. Although a brief search shows that it might be difficult to find
    such RAM. So I suppose if I were unable to find non-overclocked DDR5-5200,
    I'd try to find some EXPO DDR5-5200.

## Graphics
> **&#8505;&#65039;<!-- information emoji --> NOTE:** I decided to stick with my
> GeForce RTX 3060 from earlier in 2023.
- **Product:**
  [GeForce RTX 3060 Ventus 2X 12G OC](https://www.msi.com/Graphics-Card/GeForce-RTX-3060-VENTUS-2X-12G-OC)
- **Price:**
  [$359.99](https://smile.amazon.com/gp/product/B08WPRMVWB)
- **Power:**
  - Best estimate: 170 W
  - PCPartPicker: 42-170 W
- **Max Temperature:** 93°C
- **Features:**
  - 3x DisplayPort
  - 1x HDMI
  - 1x 8-pin PCIe power connector
  - 1710 MHz GPU
  - 12 GB GDDR6 video RAM
  - [GeForce RTX 30 Series Specs](https://www.nvidia.com/en-us/geforce/graphics-cards/compare/?section=compare-specs)
  - [GeForce RTX 3060 Family Specs](https://www.nvidia.com/en-us/geforce/graphics-cards/30-series/rtx-3060-3060ti/?section=specs)
- **Reviews:** (just what's on Amazon)
- **Thoughts:**
  - I bought what I could find at the time since graphics cards had been all out
    of stock and were extremely expensive when they were in stock (a situation
    that had been going on for several years)
- **Hindsight:** No regrets so far...

## Storage
- **Product:**
  [WD_BLACK SN850X NVMe SSD](https://www.westerndigital.com/products/internal-drives/wd-black-sn850x-nvme-ssd?sku=WDS400T2X0E)
- **Price:**
  [$229.99](https://smile.amazon.com/WD_BLACK-SN850X-Internal-Gaming-Solid/dp/B0B7CQ2CHH)
- **Power:**
  - Best estimate: ~10 W (based on 8.1 W max listed for the Samsung 990 PRO on
    TechPowerUp linked in the **Thoughts** section below)
  - PCPartPicker: 2-10 W
- **Max Temperature:** 85°C
- **Features:**
  - 4 TB
  - PCIe Gen4 x4
  - M.2 2280 (M-key)
- **Reviews:**
  - General:
    - [PC Builder: STOP Buying Bad SSDs! Best SSD for Gaming 2023 (PC / PS5 / XBOX)](https://www.youtube.com/watch?v=TOBgGHJsHFI)
  - Benchmarks:
    - [PassMark Hard Drive Benchmarks](https://www.harddrivebenchmark.net/high_end_drives.html)
    - [Techtesters: The New King of Gen4 SSDs - Crucial T500 Review](https://www.youtube.com/watch?v=vOBMrjGwzEM)
    - [Techtesters: Samsung 990 Pro 4TB NVMe SSD Review](https://www.youtube.com/watch?v=UYP0JiYJYYo)
    - [Techtesters: WD Black SN850X Gen4 NVMe SSD Review](https://www.youtube.com/watch?v=t5yC1PlhHJE)
    - [Techtesters: Samsung 990 PRO NVMe SSD Review - Versus 22 Other Drives](https://www.youtube.com/watch?v=yoD-zx46VgU)
    - [Techtesters: The Big Gen4 SSD Roundup - Best SSDs for PC & Playstation 5 in 2022](https://www.youtube.com/watch?v=Zy2HtI20eFQ)
    - [Linus Tech Tips: PCIe Gen5 Drives are Here! Are they Worth It?? - Crucial T700 PCIe Gen 5 NVMe SSD](https://www.youtube.com/watch?v=jnMMtbVP0ps)
  - Motherboard support:
    - [ASUS HDD Devices Support](https://www.asus.com/motherboards-components/motherboards/tuf-gaming/tuf-gaming-b650-plus-wifi/helpdesk_qvl_device)
  - Heatsinks:
    - [CrazyTechLab: Massive M.2 SDD HEATSINK ROUNDUP! Best options for PCIe 4 and PCIe 5 SSDs](https://www.youtube.com/watch?v=XlRr7X6Y6iQ)
  - Software:
    - [Simply Tech: Keep Your SN850 NVME SSD In Peak Condition With Western Digital Drive Dashboard](https://www.youtube.com/watch?v=1_PnfGiisSc)
    - [Simply Tech: Benchmark your NVME SSD with Samsung Magician](https://www.youtube.com/watch?v=34Ki4ZdfFr8)
    - [Glenn Berry: How To Use Samsung Magician](https://www.youtube.com/watch?v=LvuNnHLfySs)
    - [StorageReview: Samsung Magician 7 Review (Detailed Walkthrough)](https://www.youtube.com/watch?v=awfcu9zUgYo)
  - Samsung firmware issues:
    - [Gamers Nexus: HW News - Dying Samsung SSD Fix, Intel Mega CPUs, RTX 4070 Rumors](https://www.youtube.com/watch?v=cU0KDQ_ePUE)
    - [JayzTwoCents: Samsung 980 Pro NVMe Failure and how to stop it from happening!](https://www.youtube.com/watch?v=DoAFzdz0h5M)
- **Thoughts:**
  - I was quite torn between the Samsung 990 PRO and the WD_BLACK SN850X.
    Ultimately, I let price decide the winner.
    - **Price:**
      - Samsung 990 PRO: $250
      - WD_BLACK SN850X: $230
    - Performance: the Samsung 990 PRO performs better in most benchmarks, but
      the WD_BLACK SN850X beats it in gaming benchmarks
    - Maximum operating temperature:
      - Samsung 990 PRO: 70°C
      - WD_BLACK SN850X: 85°C
    - Software: the Samsung Magician and Western Digital Dashboard seem pretty
      similar
    - Firmware: Samsung had some firmware issues with the 980 PRO and 990 PRO
      but they seem to be resolved now (although people are criticizing how
      Samsung handled the situation)
  - I was apprehensive about using the motherboard's built-in heatsinks, but at
    least one review seems to indicate that it performs better than most
    third-party heatsinks
  - I wish the SSD manufacturers provided more technical specs. I could not find
    official documentation about some of the technical specs from some of the
    manufacturers' websites. Below are some technical specs from TechPowerUp
    (although I have no idea how accurate they are):
    - [Samsung 990 Pro 4 TB](https://www.techpowerup.com/ssd-specs/samsung-990-pro-4-tb.d863)
    - [Samsung 990 Pro (w/ Heatsink) 4 TB](https://www.techpowerup.com/ssd-specs/samsung-990-pro-w-heatsink-4-tb.d866)
    - [Western Digital SN850X (w/ Heatsink) 4 TB](https://www.techpowerup.com/ssd-specs/western-digital-sn850x-w-heatsink-4-tb.d860)
- **Hindsight:** No regrets so far...

## Case
- **Product:**
  [Fractal Design Torrent](https://www.fractal-design.com/products/cases/torrent/torrent/black-solid)
- **Price:**
  [$189.99](https://www.newegg.com/black-fractal-design-torrent-atx-mid-tower/p/N82E16811352147)
- **Power:**
  - Best estimate: ~20 W (based on the power specs detailed in the
    [Fan Controller/Hub/Splitter](#fan-controllerhubsplitter) section,
    2 * 4.2 W + 3 * 3 W = 17.4 W)
  - PCPartPicker: N/A
- **Max Temperature:** N/A
- **Features:**
  - Front: 1x USB 3.1 Gen 2 Type-C, 2x USB 3.0, HD Audio
  - Fans:
    - Front: 2x 180mm Dynamic X2 GP-18 PWM
    - Bottom: 3x 140mm Dynamic X2 GP-14 PWM
  - Dust Filters: front, bottom
- **Reviews:**
  - [Gamers Nexus: Best PC Cases of 2022: $60 to $300 Airflow, Silence, & Budget Cases](https://www.youtube.com/watch?v=pL5uttjPWZE)
  - [Gamers Nexus: Best Case of 2021 So Far: Fractal Torrent Case Review & Benchmarks](https://www.youtube.com/watch?v=HBxo2_lwKps)
  - [Gamers Nexus: Fractal Puts Everyone to Shame: Fire Hazard Fix Tested (Torrent Case)](https://www.youtube.com/watch?v=R1EcppuGxCY)
- **Thoughts:**
  - I want something quiet with...
    - Good thermals
    - No RGB lights (my computer is in the living room and lights are
      distracting when watching TV)
    - No transparent panels (the inside of my computer is always filled with
      dust because I don't clean it often enough, plus I keep the tower on the
      floor, so there's no point to a transparent panel)
- **Hindsight:**
  - This case is very large. I probably could have gone with the "Compact"
    version (which is still ATX, just smaller) if I were actually able to find
    one for sale when I bought my case (I did try, but everything that wasn't
    shipping all the way from the UK was sold out).

## Fan Controller/Hub/Splitter
- **Product:** PWM Fan Splitter (1 to 2 converter)
- **Price:**
  [$5.95](https://smile.amazon.com/JBtek-Black-Sleeved-Splitter-Converter/dp/B01EF9OI0O)
- **Power:** N/A
- **Max Temperature:** N/A
- **Features:**
  - 1x 4-pin fan header to 1x 4-pin fan header and 1x 3-pin fan header
    - One of the split headers is intentionally missing a pin because one of the
      pins reads the RPM value from the fan and it only makes sense to report
      one value back to the motherboard. However, both fans will get power and
      PWM signals from the motherboard. The only downside is that the fans
      cannot be controlled independently.
- **Reviews:** (just what's on Amazon)
- **Thoughts:**
  - The case I chose comes with 5 fans, but the motherboard I chose only has 4
    fan headers. Luckily, the case also comes with the Nexus 9P Slim PWM fan hub
    pre-installed. However, a fan hub will reduce the control I have over
    individual fans, so it seems to me that I should prefer to use the
    motherboard headers instead of the fan hub.
  - According to the motherboard and case manuals, any two fans should be fine
    to run off a splitter from any motherboard chassis fan header since...
    - The motherboard can supply 12 W at 1 A on each chassis fan header
      (according to the
      [manual](https://dlcdnets.asus.com/pub/ASUS/mb/Socket%20AM5/TUF%20GAMING%20B650-PLUS%20WIFI/E21902_TUF_GAMING_B650-PLUS_WIFI_UM_V3_WEB.pdf#page=13))
    - Each 140mm
      [Dynamic X2 GP-14 PWM](https://www.fractal-design.com/products/fans/dynamic/dynamic-x2-gp-14-pwm/black)
      fan has a maximum of 0.25 A at 12 V (3 W) and an actual input power of
      1.7 W (I'm not sure how they got 1.7 W, but either way it's less than half
      of the motherboard's 12 W, so it should be fine)
    - Each 180mm
      [Dynamic X2 GP-18 PWM](https://www.fractal-design.com/products/fans/dynamic/dynamic-x2-gp-18-pwm/black)
      fan has a maximum of 0.35 A at 12 V (4.2 W) and an actual input power of
      4.2 W (this time the math checks out, so who knows...)
  - While I could use the pre-installed fan hub to control only two of the fans
    instead of using a splitter, it seems like a lot of unnecessary cable
    routing just to power two fans (since the hub requires its own power)
- **Hindsight:** No regrets so far...

## Power Supply
- **Product:** [Corsair RM750e](https://www.corsair.com/us/en/p/psu/cp-9020248-na/rme-series-rm750e-fully-modular-low-noise-atx-power-supply-cp-9020248-na)
- **Price:**
  [$99.99](https://smile.amazon.com/dp/B0BYR1BXC6)
- **Power:** 750 W
- **Max Temperature:** N/A (I couldn't find any official documentation on
  temperatures for the PSU. Supposedly a common maximum temperature for 100%
  power output is ~40°C
  ([example](https://www.corsair.com/us/en/p/psu/cp-9020245-na/sf-l-series-sf850l-fully-modular-low-noise-sfx-power-supply-cp-9020245-na)),
  but I have no idea if that temperature is for internal components or for the
  air intake. Also, the capacitors are usually rated to either 85°C or 105°C,
  for whatever that's worth.)
- **Features:**
  - 750 W
  - Fully modular
  - Cables:
    - 1x ATX motherboard (24-pin, one connector)
    - 2x ATX 12 V / EPS 12 V (4+4-pin, one connector)
    - 1x 12VHPWR (12+4-pin, one connector)
    - 1x dual PCIe (6+2-pin, two connectors)
    - 1x single PCIe (6+2-pin, one connector)
    - 1x straight SATA (3x straight connectors)
    - 1x right-angle SATA (4x right-angle connectors)
    - 1x PATA (4x 4-pin connectors)
  - Gold 80 PLUS Efficiency
  - ATX 3.0 Certified (should support PCIe Gen 5 and resist transient power
    spikes)
  - Modern Standby Compatible (faster wake-from-sleep times and better low-load
    efficiency)
  - 105°C-rated capacitors
- **Reviews:**
  - Benchmarks:
    - [Hardware Busters: Best ATX v3.x & PCIe 5.x Ready PSU Picks 2023 – Hardware Busters](https://hwbusters.com/best_picks/best-atx-v3-0-pcie-5-0-ready-psus-picks-2023-hardware-busters)
    - [Hardware Busters: Corsair RM1000e (2023) Gen5 PSU Review](https://hwbusters.com/psus/corsair-rm1000e-gen5-psu-review)
    - [Gamers Nexus: Amazon's 5 Most Popular Power Supplies: Budget PSU Round-Up](https://www.youtube.com/watch?v=weFJd8dzxAE&list=PLsuVSmND84QtHZ6WXQ4-4YJhq9VVkOOtw)
    - [Cultists Network: PSU Tier List](https://cultists.network/140/psu-tier-list)
  - Efficiency & Noise:
    - [Cybenetics: ATX 3.0 Noise Benchmarks](https://www.cybenetics.com/index.php?option=database&params=4,2,0)
    - [Cybenetics: ATX 3.0 Efficiency Benchmarks](https://www.cybenetics.com/index.php?option=database&params=4,1,0)
    - [Cybenetics: Efficiency Benchmarks](https://www.cybenetics.com/index.php?option=database&params=1,1,0)
    - [Cybenetics: Noise Benchmarks](https://www.cybenetics.com/index.php?option=database&params=1,2,0)
    - [Gamers Nexus: Power Supplies Need a New Rating System (80 Plus Misunderstandings & Cheated Results)](https://www.youtube.com/watch?v=QrhuOwNdkA4&list=PLsuVSmND84QtHZ6WXQ4-4YJhq9VVkOOtw)
  - Corsair RMx Shift Series:
    - [Hardware Busters: Corsair RM750x Shift PSU Review: They Shifted the Modular Panel!](https://hwbusters.com/psus/corsair-rm750x-shift-psu-review-they-shifted-the-modular-panel)
    - [JayzTwoCents: I tried to prove this design was a failure... But then this happened.](https://www.youtube.com/watch?v=Qt7LhtyP0Q0)
  - ATX Spec changes:
    - 12V-2x6:
      - [Hardware Busters: No More 12VHPWR Connector! Say hi to 12V-2×6](https://hwbusters.com/news/no-more-12vhpwr-connector-say-hi-to-12v-2x6)
      - [Hardware Busters: How to Select a new PSU with the upcoming 12VHPWR change?](https://hwbusters.com/psus/how-to-select-a-new-psu-now-with-the-12vhpwr-upcoming-change)
      - [Hardware Busters: ATX v3.1 & PCIe CEM 5.1 are official!](https://hwbusters.com/psus/atx-v3-1-pcie-cem-5-1-are-official)
      - [Hardware Busters: Will my ATX v3.0 PSU or my GPU be compatible with 12V-2×6? Do I need a new cable/PSU/GPU? Everything you need to know!](https://hwbusters.com/psus/will-my-atx-v3-0-psu-or-my-gpu-be-compatible-with-12v-2x6-do-i-need-a-new-cable-psu-gpu-everything-you-need-to-know)
    - 12VHPWR:
      - [JayzTwoCents: The 12VHPWR adapter cable is DANGEROUS! But NVIDIA doesn't agree...](https://www.youtube.com/watch?v=HAZWwwHScaQ)
      - [Gamers Nexus: The Truth About NVIDIA’s RTX 4090 Adapters: Testing, X-Ray, & 12VHPWR Failures](https://www.youtube.com/watch?v=ig2px7ofKhQ)
      - [eTeknix: THE TRUTH: The NVIDIA 40 Series Will NOT Blow Up Your PSU!!! [Feat JonnyGURU]](https://www.youtube.com/watch?v=EvsPZA8CkBY)
    - ATX 3.0:
      - [Techquickie: Do You Need A New Power Supply? - ATX 3.0](https://www.youtube.com/watch?v=EGHyDuPG1ks)
      - [Gamers Nexus: The Brewing Problem with GPU Power Design | Transients](https://www.youtube.com/watch?v=wnRyyCsuHFQ&list=PLsuVSmND84QtHZ6WXQ4-4YJhq9VVkOOtw)
    - ATX12VO:
      - [Gamers Nexus: The Future of Power Supplies - Maybe (Motherboard Cost, Cables, & ATX12VO)](https://www.youtube.com/watch?v=Zc9oRKexV_s&list=PLsuVSmND84QtHZ6WXQ4-4YJhq9VVkOOtw)
  - General PSU Info:
    - [JayzTwoCents: This is the most OVERLOOKED component in most PCs...](https://www.youtube.com/watch?v=0c7aVTLtYg8)
    - [Gamers Nexus: Wasting Money on Power Supplies: How Many Watts You Need for a PC PSU (2020)](https://www.youtube.com/watch?v=X_wtoCBahhM&list=PLsuVSmND84QtHZ6WXQ4-4YJhq9VVkOOtw)
    - [PC Builder: STOP Buying BAD PSUs! Best Power Supply for PC 2023](https://www.youtube.com/watch?v=XMCG9axMmqM)
- **Thoughts:**
  - Based on the benchmarks, price, and its lack of RGB LEDs, I would have loved
    to get a Corsair RMx Shift PSU, but having the ports on the side isn't going
    to be particularly convenient for my case (see the JayzTwoCents video)
  - Due to both recent and upcoming changes to the ATX spec (ATX12VO, ATX 3.0 /
    12VHPWR, ATX 3.1 / 12V-2x6, etc.), I think it might make sense to buy a
    cheaper PSU now and plan on potentially replacing it once the changes have
    been finalized
  - Having an ATX 3.0 PSU is probably nice for the changes to the spec about
    handling transients. However, due to the issues with the 12VHPWR connector,
    it probably makes sense to get a PSU that does NOT use the 12VHPWR connector
    on the PSU side to eliminate at least one point of failure.
- **Hindsight:**
  - It took a ton of research to figure out what the heck is going on with all
    these ATX spec changes. From what I've stumbled across since I made my
    purchase, I think ATX 3.1 is probably a small change over ATX 3.0 on the PSU
    side (assuming your PSU is using two 8-pin connectors instead of a
    problematic 12VHPWR connector). Therefore, if I were to buy a new PSU, I
    would do a little more research into how future-proof ATX 3.0 PSUs can be,
    and depending on those results, I might opt for a slightly better (more
    expensive, more efficient, quieter, and/or larger power capacity) ATX 3.0
    PSU that uses two 8-pin connectors on the PSU side (instead of a problematic
    12VHPWR connector).


# Software

## Operating System
- TODO

## ASUS Armoury Crate
- TODO

## MyASUS
- TODO

## Western Digital Dashboard
- TODO


# Peripherals

## Monitors
- TODO: sticking with my current monitors

## Keyboard
- TODO: new keyboard

## Mouse
- TODO: new mouse

## Mouse Pad
- TODO: new mouse pad

## Speakers
- **Product:**
  [Creative Pebble V3](https://us.creative.com/p/speakers/creative-pebble-v3)
- **Price:** [$34.99](https://smile.amazon.com/dp/B08F57GSJ7)
- **Features:**
  - USB-C, 3.5mm, and/or Bluetooth 5.0 connectivity
- **Reviews:**
  - [Creative Pebble Pro vs Pebble V3 Comparison and Review - The best budget USB powered speakers?](https://www.youtube.com/watch?v=75B5aLUmJYc)
  - [Creative Pebble Speaker Wars: Which Version is Worth Your Money?](https://www.youtube.com/watch?v=eBvwdJKL24c)
- **Thoughts:**
  - I rarely use my computer speakers, so I want something small and relatively
    inexpensive
  - A USB connection (digital) to the computer would be nice, rather than a
    3.5mm connection (analog), simply because in my experience, cheap analog
    audio components can have bad connections
  - Built-in Bluetooth seems like a nice feature that I might occasionally use
    to play music from my phone
- **Hindsight:** No regrets so far...


# Tools
- [Precision Screwdriver Set](https://smile.amazon.com/STREBITO-Precision-Screwdriver-Improvement-Electronic/dp/B099K2QG9T)
- [Electric Air Duster](https://smile.amazon.com/SIN-SHINE-Compressed-Electric-AD01-Black/dp/B083LNC6NR)


# Build Process

## POST Issues
- TODO: describe POST issues
  (https://www.reddit.com/r/buildapc/comments/z037cl/asus_tuf_gaming_b650_plus_motherboard_dram_light)
