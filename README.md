
# Spot ROS - Proyek Spot Robot dengan ROS

Proyek ini mengimplementasikan antarmuka untuk mengendalikan robot Spot dari Boston Dynamics menggunakan Robot Operating System (ROS). Tujuan dari proyek ini adalah untuk menyediakan cara sederhana bagi pengguna ROS untuk mengontrol dan mengintegrasikan Spot ke dalam lingkungan robotik mereka.

## Fitur
- **Teleop**: Mengendalikan Spot secara manual dengan menggunakan joystick atau antarmuka ROS lainnya.
- **Autonomy**: Menyediakan API untuk menjalankan misi otonom dengan Spot, seperti navigasi otomatis dan penjelajahan.
- **Visualisasi**: Memungkinkan pengguna untuk melihat data sensor Spot dan informasi status di Rviz, sebuah alat visualisasi untuk ROS.
- **Kompatibilitas**: Mendukung berbagai versi ROS dan sistem operasi, serta dapat diintegrasikan dengan sistem robotik lainnya.

## Prasyarat
- **ROS**: Pastikan Anda memiliki instalasi ROS yang berfungsi. Proyek ini diuji dengan ROS Noetic dan ROS Melodic.
- **Spot SDK**: Anda harus memiliki SDK resmi dari Boston Dynamics untuk berinteraksi dengan robot Spot.
- **Python 3**: Digunakan untuk menjalankan skrip dan komunikasi dengan ROS.

## Instalasi
1. Clone repositori ini ke dalam workspace ROS Anda:
    ```
    git clone https://github.com/heuristicus/spot_ros.git
    ```
2. Instal semua dependensi yang diperlukan:
    ```
    rosdep install --from-paths src --ignore-src -r -y
    ```
3. Build workspace Anda:
    ```
    catkin_make
    ```
4. Sumberkan setup file:
    ```
    source devel/setup.bash
    ```

## Penggunaan
Untuk menjalankan kontrol manual Spot:
```
roslaunch spot_driver teleop.launch
```
Untuk menjalankan misi otonom dengan Spot:
```
roslaunch spot_autonomy autonomy.launch
```

## Kontribusi
Jika Anda ingin berkontribusi, silakan fork repositori ini dan buat pull request dengan perubahan atau peningkatan yang ingin Anda tambahkan. Pastikan Anda mengikuti pedoman pengkodean yang ada dan menambahkan dokumentasi yang sesuai.

## Lisensi
Proyek ini dilisensikan di bawah lisensi MIT. Lihat file `LICENSE` untuk informasi lebih lanjut.

## Kredit
Proyek ini dikembangkan oleh komunitas ROS dengan kontribusi dari berbagai pengembang yang tertarik untuk mengintegrasikan Spot dengan ROS. 

## Source
https://github.com/heuristicus/spot_ros/blob/master/README.md
