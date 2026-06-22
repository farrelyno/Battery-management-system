# 🔋 Battery Management System (BMS)

## Overview

Battery Management System (BMS) adalah sistem elektronik yang digunakan untuk memantau, melindungi, dan mengelola baterai lithium agar dapat beroperasi dengan aman, efisien, dan memiliki umur pakai yang lebih panjang.

Repository ini berisi dokumentasi teknis mengenai prinsip kerja Battery Management System, mulai dari dasar teori hingga implementasi berbagai fitur proteksi yang umum digunakan pada baterai lithium-ion.

## Kondisi Tegangan Pada Baterai
* Tegangan Nominal = Nilai tegangan rata-rata yang mewakili karakteristik baterai selama pemakaian.
* Tegangana Maksimum = Tegangan saat baterai selesai diisi penuh.
 ** Saat tegangan mencapai maksimum:
 * Pengecasan harus dihentikan untuk mencegah overcharge
* Tegangan Cutoff = Tegangan terendah yang masih diizinkan untuk digunakan.
 * Saat tegangan mencapai cutoff:
  * Beban harus diputus.
  * Baterai sebaiknya segera diisi ulang.
  * Masih ada sedikit energi tersisa, tetapi sengaja tidak digunakan untuk melindungi baterai.
  
## Features

* ⚡ Monitoring tegangan setiap sel baterai (Cell Voltage Monitoring)
* 🔌 Pengukuran arus menggunakan shunt resistor (Current Sensing)
* 🌡️ Monitoring suhu menggunakan NTC Thermistor
* 🛡️ Proteksi Overvoltage (OV)
* 🛡️ Proteksi Undervoltage (UV)
* 🛡️ Proteksi Overcurrent (OC)
* 🛡️ Proteksi Overtemperature (OT)
* 🔄 Cell Balancing
* 📊 State of Charge (SOC) Estimation
* ⚙️ Power Path Management menggunakan Back-to-Back MOSFET

## System Architecture

Secara umum BMS bekerja dalam tiga tahap utama:

1. **Sensing**

   * Mengukur tegangan sel
   * Mengukur arus baterai
   * Mengukur suhu baterai

2. **Processing**

   * Membandingkan hasil pengukuran dengan batas proteksi
   * Mengestimasi State of Charge (SOC)
   * Mengelola proses balancing

3. **Acting**

   * Mengontrol MOSFET charge/discharge
   * Mengaktifkan proteksi
   * Mengirimkan informasi status sistem

## Main Topics Covered

* Pentingnya Battery Management System
* Arsitektur BMS
* Voltage Sensing
* Current Sensing
* Temperature Sensing
* Threshold dan Hysteresis
* Power Path MOSFET
* Cell Balancing
* State of Charge (SOC)
* Pemilihan IC BMS
* Pemilihan MOSFET
* PCB Layout Guidelines
* Troubleshooting dan Design Considerations

## Applications

BMS digunakan pada berbagai aplikasi seperti:

* Electric Vehicle (EV)
* Energy Storage System (ESS)
* Solar Energy Storage
* UPS System
* E-bike dan E-motorcycle
* Portable Battery Pack
* IoT dan Embedded Systems

## Documentation

Dokumentasi lengkap tersedia pada file:

```text
BMS OVERVIEW.html
```

atau melalui GitHub Pages apabila repository telah di-deploy.

## References

* Texas Instruments Battery Management Solutions
* Analog Devices Battery Monitoring ICs
* Lithium-Ion Battery Datasheets
* IEC 62619
* IEC 62133
* IEEE Battery Management References

## License

This project is intended for educational and research purposes.
