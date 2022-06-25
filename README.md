# this is my process of learning, installation and settings and figuring out how to use it 
Proses Installation Firewall And Setting Rule Snort And Proses Monitoring much more

* For more details, you can visit my portfolio, [Portfolio](https://marifrizkiii.github.io/documentation-project-installation/)

# IDS dan IPS
Apa itu Snort? Snort adalah Sistem Pencegahan Intrusi Sumber Terbuka (IPS) terkemuka di dunia. Snort IPS menggunakan serangkaian aturan yang membantu menentukan aktivitas jaringan berbahaya dan menggunakan aturan tersebut untuk menemukan paket yang cocok dengannya dan menghasilkan peringatan bagi pengguna. Snort juga dapat digunakan secara inline untuk menghentikan paket-paket ini. Snort memiliki tiga kegunaan utama: Sebagai sniffer paket seperti tcpdump, sebagai pencatat paket — yang berguna untuk debugging lalu lintas jaringan, atau dapat digunakan sebagai sistem pencegahan intrusi jaringan yang lengkap. Snort dapat diunduh dan dikonfigurasi untuk penggunaan pribadi dan bisnis.

Apa saja pilihan saya untuk membeli dan menggunakan Snort? Setelah diunduh dan dikonfigurasi, aturan Snort didistribusikan dalam dua set: “Community Ruleset” dan “Snort Subscriber Ruleset.” Aturan Pelanggan Snort dikembangkan, diuji, dan disetujui oleh Cisco Talos. Pelanggan Snort Subscriber Ruleset akan menerima ruleset secara real-time saat dirilis ke pelanggan Cisco. Anda dapat mengunduh aturan dan menerapkannya di jaringan Anda melalui situs web Snort.org. Aturan Komunitas dikembangkan oleh komunitas Snort dan QAed oleh Cisco Talos. Ini tersedia secara bebas untuk semua pengguna.

Untuk informasi lebih lanjut tentang Aturan Pelanggan Snort yang tersedia untuk dibeli, silakan kunjungi halaman produk Snort.

* [Install Snort Dan Cara Menulis Rules](https://marifrizkiii.github.io/documentation-project-installation/#Installation_Snort)

# Snowl - Snort Gui
Apa itu Snowl? Snowl adalah GUI (antarmuka pengguna grafis) berbasis web modern untuk snort. Snort adalah open source IDS/IPS (sistem deteksi/pencegahan intrusi). Ini adalah alat baris perintah dan tidak memiliki antarmuka grafis sendiri. Oleh karena itu, kami memutuskan untuk membuat Snowl sehingga pengaturan snort menjadi otomatis dan dapat dimengerti, dan analisis ancaman senyaman mungkin.

* [Installation Snowl Snort Gui](https://marifrizkiii.github.io/documentation-project-installation/#Installation_Snowl_Snort_GUI)

# Rkhunter
Salah satu kekhawatiran potensial adalah rootkit. Rootkit adalah perangkat lunak yang dipasang secara diam-diam oleh penyusup jahat yang memungkinkan pengguna tersebut untuk melanjutkan akses ke server setelah keamanan dilanggar. Ini adalah masalah yang sangat berbahaya, karena bahkan setelah entri vektor yang awalnya digunakan pengguna untuk mendapatkan akses permanen, mereka dapat terus masuk ke server menggunakan rootkit yang mereka instal. Salah satu alat yang dapat membantu Anda melindungi sistem Anda dari masalah seperti ini adalah rkhunter. Perangkat lunak ini memeriksa sistem Anda terhadap database rootkit yang dikenal. Juga, itu dapat memeriksa file sistem lain untuk memastikan mereka cocok dengan properti dan nilai yang diharapkan.

* [Install RKHunter Dan Cara Menggunakan](https://marifrizkiii.github.io/documentation-project-installation/#Installation_Rkhunter)

# NaGIOS
Nagios adalah sistem pemantauan sumber terbuka yang populer. Nagios menyimpan inventaris server Anda dan memantaunya sehingga Anda tahu bahwa layanan penting Anda aktif dan berjalan. Menggunakan sistem pemantauan seperti Nagios adalah alat penting untuk lingkungan produksi apa pun, karena dengan memantau waktu aktif, penggunaan CPU, atau ruang disk, Anda dapat mencegah masalah sebelum terjadi, atau sebelum pengguna menghubungi Anda. Di sini kita akan menginstal Nagios 4 dan mengkonfigurasinya sehingga kita dapat memantau sumber daya host di antarmuka web Nagios. Kami juga akan menyiapkan Nagios Remote Plugin Executor (NRPE), yang akan berjalan sebagai agen host jarak jauh sehingga kami dapat memantau sumber dayanya.

# Membutuhkan
* Dua server Ubuntu 20.04 dengan hak istimewa pengguna root. Firewall dengan ufw.
* Server dengan Nagios akan disebut server Nagios.
* Server tanpa Nagios akan disebut server Ubuntu.
* Server Nagios akan menjalankan Apache dan PHP.
* Server Nagios biasanya dijalankan di belakang Firewall atau VPN. Jika Anda menjalankannya di IP Publik, Anda harus lebih serius menginstal TLS/SSL dll. Tutorial ini mengasumsikan, server Nagios berada di belakang Firewall.

* [Installation Nagios 4 dan Memantau Server di Ubuntu 20.04](https://marifrizkiii.github.io/documentation-project-installation/#Installation_Nagios)

# Zabbix
Zabbix dirancang terutama sebagai alat pemantauan infrastruktur TI. Fitur baru umumnya dirilis setiap enam bulan untuk versi utama dan setiap 1,5 tahun untuk versi LTS. Dirilis di bawah ketentuan GNU General Public License versi 2, Zabbix adalah perangkat lunak gratis yang tidak memerlukan lisensi untuk menggunakan fitur-fiturnya. Meskipun Zabbix adalah perangkat lunak sumber terbuka, ini adalah produk perangkat lunak pengembangan tertutup, yang dikembangkan oleh Zabbix LLC yang berbasis di Riga Latvia.

# Use
1. Pilih platform
* ZABBIX VERSION > 6.0 LTS
* OS DISTRIBUTION > Ubuntu
* OS VERSION > 20.04
* WEB SERVER > NGINX
* [Installation Zabbix dan Monitoring Website di Ubuntu 20.04](https://marifrizkiii.github.io/documentation-project-installation/#Installation_Zabbix)

# Open VPN IPv4
OpenVPN adalah sistem jaringan pribadi virtual (VPN) yang menerapkan teknik untuk membuat koneksi point-to-point atau situs-ke-situs yang aman dalam konfigurasi yang dirutekan atau dijembatani dan fasilitas akses jarak jauh. Ini mengimplementasikan aplikasi klien dan server.

OpenVPN memungkinkan rekan untuk mengotentikasi satu sama lain menggunakan kunci rahasia, sertifikat, atau nama pengguna/kata sandi yang dibagikan sebelumnya. Ketika digunakan dalam konfigurasi multiclient-server, memungkinkan server untuk merilis sertifikat otentikasi untuk setiap klien, menggunakan tanda tangan dan otoritas sertifikat.

Ini menggunakan perpustakaan enkripsi OpenSSL secara ekstensif, serta protokol TLS, dan berisi banyak fitur keamanan dan kontrol. Ini menggunakan protokol keamanan khusus[11] yang menggunakan SSL/TLS untuk pertukaran kunci. Ia mampu melintasi penerjemah alamat jaringan (NAT) dan firewall.

OpenVPN telah di-porting dan disematkan ke beberapa sistem. Misalnya, DD-WRT memiliki fungsi server OpenVPN. SoftEther VPN, server VPN multi-protokol, juga memiliki implementasi protokol OpenVPN.

Itu ditulis oleh James Yonan dan merupakan perangkat lunak bebas, dirilis di bawah ketentuan GNU General Public License versi 2 (GPLv2). [12] Selain itu, lisensi komersial juga tersedia.

* [Install Open VPN Dan Menggunakan](https://marifrizkiii.github.io/documentation-project-installation/#Open_VPN_IPv4)
