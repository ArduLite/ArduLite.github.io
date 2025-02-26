# 🎨 ArduLite - Arduino Versi Lite ⚡️

## 📌 Tentang ArduLite

**ArduLite** adalah library/framework ringan untuk **C++** yang dirancang khusus untuk board **Arduino dengan memori terbatas**, seperti:

- 🎯 Arduino Uno
- 🎯 Arduino Nano
- 🎯 Board berbasis **ATMega8**

Tujuan utama dari **ArduLite** adalah **menghemat penggunaan memori** dibandingkan dengan framework Arduino standar, sehingga memungkinkan aplikasi berjalan lebih efisien di perangkat dengan sumber daya terbatas.

## 🚀 Mengapa ArduLite?

✨ **Lebih Hemat Memori** → Program "blink" standar pada Arduino memakan **924 bytes**, sementara dengan **ArduLite hanya 190 bytes** saja!  
🎨 **Desain Kode Lebih Elegan** → Struktur kode tetap mirip dengan Arduino asli, sehingga tetap mudah dipahami.  
🛠 **Cocok untuk Board Low-Memory** → Dirancang khusus untuk board dengan **SRAM & Flash kecil**.

## 🔧 Cara Instalasi

1. **🛠 Melalui Library Manager Arduino IDE**:
   - Buka **Arduino IDE**
   - Masuk ke menu **Sketch > Include Library > Manage Libraries**
   - Cari **ArduLite**
   - Klik **Install**

2. **📥 Alternatif: Install Manual dari GitHub**:
   - Clone repository dengan perintah:
     ```bash
     git clone https://github.com/ArduLite.git
     ```
   - Tambahkan ke **Arduino IDE**:
     - Buka **Arduino IDE**
     - Masuk ke menu **Sketch > Include Library > Add .ZIP Library**
     - Pilih folder **ArduLite**

3. **📝 Gunakan di Sketch Arduino**:
   ```cpp
   #include "ArduLite.h"

   int main() {
      Digital led(13, OUT);

      while(1){
         led.on();
         wait(300);
         led.off();
         wait(300);
      }
   }
   ```

## 💡 Contoh Perbandingan Memori

📊 **Hasil Pengujian Penggunaan Memori**

| Library | Flash Memory Usage |
|---------|--------------------|
| **Arduino**  | 924 bytes |
| **ArduLite** | 190 bytes |

Dengan ArduLite, Anda bisa menghemat **lebih dari 79% memori!**

## 🎭 Uji Coba di Wokwi

Penasaran ingin mencoba sebelum install? Cek langsung di Wokwi:

🎨 [🔗 Coba ArduLite di Wokwi](https://wokwi.com/projects/411835205072828417)

## 📖 Dokumentasi & Pengembangan

ArduLite masih dalam tahap pengembangan, namun Anda bisa melihat source code awalnya di:

🔗 **GitHub Repository**: [https://github.com/ArduLite](https://github.com/ArduLite)

Jika ingin berkontribusi, silakan fork, buat pull request, atau beri ide di **Issues**! 🚀

## 🏆 Dukungan

💖 Bantu proyek ini berkembang dengan cara:

- ⭐ **Berikan Star** di GitHub!
- 🛠️ **Bantu kembangkan kode** (kontribusi selalu diterima!)
- 📢 **Bagikan ke teman-teman yang butuh library ringan untuk Arduino!**

Terima kasih sudah mendukung ArduLite! ✨🎨
