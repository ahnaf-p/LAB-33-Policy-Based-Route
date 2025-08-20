# LAB-33-Policy-Based-Route
Rabu 20 Agustus 2025  
  
# Policy Based Route
  PBR merupakan fitur yang berfungsi memetakan jalur. Kita bisa memetakan berdasarkan alamat IP tujuan, IP asal, bisa juga kita buat yang lebih spesifik lagi berdasarkan koneksi (port dan protokol). Biasanya digunakan jika kita memiliki lebih dari 1 link menuju provider agar lebih efisien. Tujuan utamaknya adalah untuk memisahkan service, layanan atau jaringan tertentu agar mengunakan jalur ISP yang berbeda. Dan pemetaan jalur ini bisa disesuaikan dengan kondisi yang ada dilapangan. Agar lebih efisien dan tidak ada down time di jaringan, PBR bisa di kombinasikan dengan failover. Yang berfungsi saat salah saru link atau ISP putus maka bisa mengunakan jalur atau link yang masih tersedia. Penggunaan PBR ini tidak terbatas hanya dengan 2 link menuju ISP, tetapi bisa saja lebih banyak lagi.  
  
# Konfigurasi PBR  
  1. Pastikan kita sudah melakukan basic config (IP Address, DNS, NAT, dll). Kemudian kita bisa coba untuk lakukan konfigurasi PBR. Pada kasus ini kita akan konfigurasi PBR1 menggunakan Route Rules.
  2. Sekarang pergi ke **IP > Route** lalu kita **add**, untuk alamat ip asalnya (src. Address) kita bisa isi dengan alamat IP dari LAN A **10.1.1.0/24**, dan actionnya **lookup**.  
![](IMAGES/)  
  3. Lalu buat lagi untuk IP **10.2.2.0/24**.  
![](IMAGES/)
  4. 
