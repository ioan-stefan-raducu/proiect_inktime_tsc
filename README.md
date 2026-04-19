

# Proiect TSC 2026

Raducu Ioan Stefan 335CA

## Descriere proiect
InkTime este un dispozitiv open source de tip smartwatch construit în cadrul clasei de proiectare hardware din UNSTPB. Device-ul are integrat un MCU nRF52840, senzori IMU și un display E-paper într-o carcasă compactă. Designul consideră aspectele legate de consum minim de energie, optimizarea PCB-ului pentru producție.

## Schema bloc
![schema bloc](<block_scheme.png>)
Se pot vedea in schema bloc componentele conectate prin sageti. Sagetiile au urmatoarele semnificatii:
- rosu - trasee de putere
- albastru deschis - conexiuni I2C
- albastru inchis - conexiuni SPI
- mov - trasee diferentiale
- gri - conexiuni GPIO sau fara a apartine categoriilor de mai sus

Iată tabelul **BOM (Bill of Materials)** pentru proiectul tău, extras și organizat din datele furnizate. Am grupat componentele pentru o mai bună lizibilitate, am adăugat link-urile de achiziție (prioritizând JLC/Mouser unde au fost disponibile) și link-urile către documentația tehnică.

## Bill of Materials

| Componentă / Valoare | Cant. | Capsulă | Producător / Part Number | Sursă Achiziție (JLC/Mouser) | Datasheet |
| :--- | :---: | :--- | :--- | :--- | :--- |
| **nRF52840** | 1 | aQFN-73 | Nordic / nRF52840-QIAA | [Mouser Link](https://www.mouser.ro/c/?q=nRF52840) | [Datasheet](https://infocenter.nordicsemi.com/pdf/nRF52840_PS_v1.1.pdf) |
| **BMA423** | 1 | 12-pin LGA | Bosch / BMA423 | [Mouser Link](https://www.mouser.co.uk/ProductDetail/Bosch-Sensortec/BMA423?qs=HXFqYaX1Q2xC%252BSgeGoX3mg%3D%3D) | [Datasheet](https://www.bosch-sensortec.com/media/boschsensortec/downloads/datasheets/bst-bma423-ds004.pdf) |
| **BQ25180YBGR** | 1 | BGA-8 | TI / BQ25180YBGR | [Mouser Link](https://www.mouser.co.uk/ProductDetail/Texas-Instruments/BQ25180YBGR?qs=doiCPypUmgEWjAK%252BJAX6Tw%3D%3D) | [Datasheet](https://www.ti.com/lit/ds/symlink/bq25180.pdf) |
| **MAX17048G+T10** | 1 | TDFN-8 | Analog Devices / MAX17048 | [Mouser Link](https://www.mouser.ro/Search/Refine?Keyword=MAX17048G%2BT10) | [Datasheet](https://datasheets.maximintegrated.com/en/ds/MAX17048-MAX17049.pdf) |
| **DRV2605YZFR** | 1 | BGA-9 | TI / DRV2605YZFR | [Mouser Link](https://www.mouser.ro/Search/Refine?Keyword=DRV2605YZFR) | [Datasheet](https://www.ti.com/lit/ds/symlink/drv2605.pdf) |
| **RT6160AWSC** | 1 | WLCSP-15 | Richtek / RT6160AWSC | [Mouser Link](https://www.mouser.co.uk/ProductDetail/Richtek/RT6160AWSC?qs=amGC7iS6iy%2FLd9PSoixZXQ%3D%3D) | [Datasheet](https://www.richtek.com/assets/product_file/RT6160/DS6160-03.pdf) |
| **2450AT18B100E** | 1 | 3216 (1206) | Johanson / Antenă 2.45GHz | [Mouser Link](https://www.mouser.co.uk/ProductDetail/Johanson-Technology/2450AT18B100E?qs=yCnrNFeXz%252Bh5MFsFIXGZGA%3D%3D) | [Datasheet](https://www.johansontechnology.com/datasheets/2450AT18B100E/2450AT18B100E.pdf) |
| **744043680 (L4)** | 1 | 4.8x4.8mm | Wurth / 68µH Inductor | [JLC Part](https://jlcpcb.com/partdetail/Wurth_Elektronik-744043680/C167448) | [Datasheet](https://www.we-online.com/catalog/datasheet/744043680.pdf) |
| **FTC252012SR47** | 1 | 2520 (1008) | TDK / 0.47µH Inductor | [JLC Part (C5832368)](https://jlcpcb.com/partdetail/6763488-FTC252012SR47MBCA/C5832368) | [Datasheet](https://product.tdk.com/en/system/files/dam/doc/product/inductor/inductor/smd/catalog/inductor_commercial_power_ftc252012s_en.pdf) |
| **503480-2400** | 1 | FPC-24 | Molex / Conector EPD | [Mouser Link](https://www.mouser.co.uk/ProductDetail/Molex/503480-2400?qs=OAhjpuo3Vu7efIoxFh9AOw%3D%3D) | [Datasheet](https://www.molex.com/pdm_docs/sd/5034802400_sd.pdf) |
| **USB-C 16P** | 1 | SMT | Kinghelm / KH-TYPE-C-16P | [JLC Part](https://jlcpcb.com/partdetail/Kinghelm-KH_TYPE_C_16P/C5186522) | [Datasheet](https://datasheet.lcsc.com/lcsc/2112151030_Kinghelm-KH-TYPE-C-16P_C2930266.pdf) |
| **EVP-AKE31A** | 3 | SMT (Buton) | Panasonic / Tactile SW | [Mouser Link](https://www.mouser.ro/Search/Refine?Keyword=EVP-AKE31A) | [Datasheet](https://industrial.panasonic.com/ww/products/pt/tactile-sw/models/EVPAKE31A) |
| **USBLC6-2SC6Y** | 1 | SOT-23-6 | ST / Protecție ESD | [JLC Part](https://jlcpcb.com/partdetail/STMicroelectronics-USBLC6_2SC6Y/C7519) | [Datasheet](https://www.st.com/resource/en/datasheet/usblc6-2.pdf) |
| **MBR0530** | 3 | SOD-123 | ON Semi / Schottky 0.5A | [JLC Part](https://jlcpcb.com/partdetail/onsemi-MBR0530T1G/C2131) | [Datasheet](https://www.onsemi.com/pdf/datasheet/mbr0530t1-d.pdf) |
| **SI1308EDL** | 1 | SC-70-3 | Vishay / N-Ch MOSFET | [Mouser Link](https://www.mouser.ro/Search/Refine?Keyword=SI1308EDL) | [Datasheet](https://www.vishay.com/docs/72013/si1308edl.pdf) |
| **DMG2305UX-7** | 1 | SOT-23 | Diodes Inc / P-Ch MOSFET | [JLC Part](https://jlcpcb.com/partdetail/Diodes_Incorporated-DMG2305UX_7/C128526) | [Datasheet](https://www.diodes.com/assets/Datasheets/DMG2305UX.pdf) |

### Rezistente si condensatoare

| Valoare | Cant. | Capsulă | Tip | JLC |
| :--- | :---: | :--- | :--- | :--- |
| **1uF / 50V** | 10 | 0402 | Condensator (EPD) | [C52923](https://jlcpcb.com/partdetail/Samsung_Electro_Mechanics-CL05A105KB5NQNC/C52923) |
| **10uF** | 4 | 0402 | Condensator | [C15525](https://jlcpcb.com/partdetail/Samsung_Electro_Mechanics-CL05A106MQ5NUNC/C15525) |
| **100nF** | 5 | 0201 | Condensator | [C1619](https://jlcpcb.com/partdetail/Murata_Electronics-GRM033R61A104KE84D/C1619) |
| **10K** | 6 | 0201 | Rezistență | [C25744](https://jlcpcb.com/partdetail/Yageo-RC0201JR_0710KL/C25744) |
| **5.1K (5K1)** | 2 | 0201 | Rezistență (USB CC) | [C25785](https://jlcpcb.com/partdetail/Yageo-RC0201JR_075K1L/C25785) |
| **3.3K (3K3)** | 2 | 0201 | Rezistență | [C25891](https://jlcpcb.com/partdetail/Yageo-RC0201JR_073K3L/C25891) |

## Functionalitati hardware

Pentru urmatoarele functionalitati hardware se vor folosi numele circuitelor asa cum sunt reprezentate in schematic. La conectarea cu alte circuite se vor mentiona circuitele cu semnalele puse in paranteza, langa mentionarea lor.

### LiPo Battery
Circuitul LiPo battery este conectorul catre baterie. El este amplasat aproape de circuitul DC/DC(VREG, 3V3) si Fuel Gauge(3V3, VBAT) formand un ansamblu. Acest amsamblu este amplasat langa E-Paper Connector si USB Connector(VBUS) pentru a izola zonele care se ocupa cu traseele de putere sau au putere mare de restul componentelor, pentru a evita interferentele. Este conectat la microcontroller prin protocolul I2C.

### Fuel Gauge
Circuitul Fuel Gauge se ocupa cu masurarea nivelului bateriei si alertarea microprocesorului cand bateria este descarcata. El este conectat la microcontroller prin protocolul I2C si semnalul ALERT (probabil folosit ca intrerupere).

### DC/DC
Circuitul DC/DC este adaptorul de tensiune al PCB-ului. El trimite semnale de putere folsind PWM pentru a regla tensiunea. Este conectat la procesor cu protoculul I2C.

### E-Paper Connector
Circuitul E-Paper Connector este conexiunea la ecranul E-Paper. El este conectat la microcontroller prin protoculul SPI. Semnalele care sunt conectate la microcontroller sunt EPD_BUSY, EPD_RST, EPD_DC, EPD_CS, SCK si MOSI. El este conectat si la circuitul E-Paper Drive Circuit prin PREVGH, PREVGL si 3V3.

### E-Paper Drive Circuit
Circuitul E-Paper Drive "creste" semnalul pentru modelarea cernelii pentru ecranul E-Paper. El este plasat direct langa E-Paper Display Connector datorita semnalului puternic de putere (pana la 50V) pe care il transmite ecranului. Astfel, amsamblul de putere mentionat mai devreme, conectorul E-Paper si acest circuit sunt puse apropiat pentru a nu interfera cu restul PCB-ului.

### USB-C Connector
Circuitul USB-C Connector reprezinta mufa USB. Este conectat la ansamblul de putere(VBUS), circuitul ESD Protection(VBUS, DN, DP). Desi in designul PCB-ului DN si DP ar trebui sa fie trasee diferentiale, ele nu sunt. Am luat aceasta decizie datorita pozitiei apropiate a USB-C Connector cu circuitul ESD Protection. El este conectat la microcontroller cu semnalul VBUS si indirect, prin ESD Protection, cu semnalele diferentiale D+ si D-.

### ESD Protection
Circuitul ESD Protection reprezinta protectia mufei USB-C in descarcarii statice. El este conectat la USB-C Connector(VBUS, DN, DP) si microcontroller(D+, D- trasee diferentiale). In designul PCB-ului semnalele D+ si D- au aceeasi lungime.

### SWD
Circuitul SWD este folosit pentru debugging si este conectat la semnalele importante (RESET, 3V3 si GND). Poate fi conectat la JTAG.

### Haptic Driver
Circuitul Haptic Driver este cel responsabil de vibratia ceasului. El este conectat la microcontroller prin protocolul I2C si semnalul (HAPTIC_EN). In PCB el este situat departat de IMU pentru a nu interfera cu el la fel de mult in momentul in care vibreaza.

### IMU
Circuitul IMU masoara acceleratia si directia ceasului pentru a determina cati pasi a facut utilizatorul. El este amplasat departat de Haptic Driver pentru motivul mentionat mai sus si spre centrul ceasului pentru a masura cat mai precis pasii (ceasul se misca pe mana si asta poate afecta masuratorile). El este conectat la microcontroller prin I2C si semnalele IMUINT1 si IMUINT2 (intreruperi ce pot fi setate).

## Descrierea conexiunilor microcontroller-ului nRF52840
- P$AD22(SWO) - conexiune cu TP_SWO pentru debug.
- P$AC13(RESET) - conexiune cu TP_RESET si SWD pentru resetarea componentei.
- P$AD12(EPD_BUSY) - conexiune cu E-Paper Display(EPD_BUSY). Indica daca ecranul este ocupat cu afisarea sau nu.
- P$AD10(EPD_DC) - conexiune cu E-Paper Display(EPD_DC - Data/Command). Descrie daca bitul trimis este pentru date (pixeli) sau o comanda.
- P$K2(EPD_CS) - conexiune cu E-Paper Display(EPD_CS - Chip Select) pentru protocolul SPI.
- P$AD12(EPD_RST) - conexiune cu E-Paper Display(EPD_RST) pentru resetare.
- P$AC9(P0.14) - GPIO buton din mijloc.
- P$AD8(P0.13) - GPIO buton din dreapta.
- P$W24(P1.02) - GPIO buton din stanga.
- P$AD6(D+) - traseu diferential pozitiv catre ESD Protection.
- P$AD4(D+) - traseu diferential negativ catre ESD Protection.
- P$AD2(VBUS) - conexiune cu semnalul VBUS al USB-C Connector.
- P$U1(HAPTIC_EN) - conexiune cu Haptic Driver pentru enable/disable.
- P$T2(PMIC_INT) - conexiune intrerupere cu circuitul bateriei (LiPo Battery).
- P$P2(IMU_INT2) - conexiune intrerupere cu IMU.
- P$M2(SCL) - conexiune I2C intre restul componentelor care folosesc acest protocol.
- P$N1(IMU_INT1) - conexiune intrerupere cu IMU.
- P$L1(SDA) - conexiune I2C cu restul componentelor care folosesc acest protocol.
- P$F2 si P$D2 - conexiune cu ceasul de 32KiloHerti.
- P$A12(SCK) - conexiune clock cu ecranul pentru protocolul SPI.
- P$P13(MOSI) - MOSI pentru conexiunea SPI (cu ecranul)
- P$A23 si P$A24 - conexiune cu ceasul de 32 de MegaHerti.
- P$J24(ALERT) - conexiune cu alerta circuitului Fuel Gauge.
- P$Y23(P1.01) - conexiune care conduce E-Paper Drive Circuit pentru a afisa cerneala pe ecran.
- P$AA24(SWDCLK) - conexiune pentru SWD, cu scopul de debug al ceasului.
- P$AC24(SWDIO) - conexiune SWD input/output.
- P$H23, P$F23 - conexiune pentru transmiterea wireless prin antena.

## Aprobarea erorilor si alte detalii
Inafara erorilor de overlap deja aprobate la inceput (in total 6 erori), restul erorilor por fi explicate astfel:
- 6 erori de Solid Polygon Shape, Overlap, la butoane, aparute de la sincronizarea initiala a schematicului cu PCB-ul.
- 11 erori de Via-Smd sau Smd-Via, Overlap, pentru via-in-pad a pinilor de pe procesor.

### Detalii post-review
- Am mutat circuitul IMU mai sus pentru a aloca suficeint spatiu pe PCB pentru un via mai gros de la pinul 3V3 la startul POWER. Pre-review se folosea un via cu grosimea de 0.2mm direct sub componenta IMU.
- Pentru a rezolva al doilea via cu grosimea de 0.2mm pentru un traseu de putere, de la pinul P$AD23 al nRF52840 am alocat suficient spatiu pentru a avea grosimea indicata.
- La rezolvarea greselii din schematic in care am folosit componenta NORDIC_NRF_3_CAPACITOR in locul componentei GRM011R60J152KE01L pentru condensatori, a aparut problema overlap cu fire de 0.3mm datorita footprint-ului 0201 pe care il are obligatoriu noua componenta. Pentru a rezolva am variat grosimea la 0.25mm. Personal as fi pastrat componenta precedenta datorita footprint-ului 0402.
- Am mutat firul P0.14 de pe bottom pentru a nu trece sub ceasul de 32KHz al procesorului.
- In urma modificarii schematicului circuitului Haptic Driver pinul SDA era plasat in mijloc. Pentru a rezolva problema am folosit via-in-pad. De asemenea a fost nevoie sa conectez pinul GND si am folosit via catre startul GND. 
