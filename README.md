# Unstructured Data by J.COp
Note: Ini adalah **part kedua** dari belajar dasar-dasar machine learning dari nol.

Setelah kita selesai mempelajari [Course 1 hingga Course 3](https://www.github.com/wiradkp/supervised_learning), sekarang kita masuk ke Course 4, yaitu bagaimana memproses data yang sifatnya tidak terstruktur / unstructured data.

# Starter Guide
Note: Apabila sudah memiliki environment jcopml seperti di [Course 1 - 3](https://www.github.com/wiradkp/supervised_learning), hanya perlu mengikuti step 1 (download materi) dan bisa langsung belajar.

## Step 1: Download materi
- Klik disini untuk [Download ZIP](https://codeload.github.com/WiraDKP/unstructured_data/zip/master), atau
- Bagi yang familiar dengan git, boleh menggunakan clone
    ```
    git clone https://github.com/WiraDKP/unstructured_data.git
    ```

## Step 2: Instalasi Miniconda
### **Windows user**
- Download miniconda untuk Python 3.7
    - Klik link ini untuk download: [Miniconda Windows 64-bit](https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86_64.exe)
    - Note: skip step ini apabila kamu sudah menggunakan Anaconda sebelumnya. Walau demikian, saya akan jelaskan alasan kenapa kamu sebaiknya menggunakan miniconda nanti di course ini.

- Install miniconda
    - Ketika ada pilihan `install for`, pilih `Just Me (recommended)`
    - Untuk `Advanced Options`, silahkan centang `Register Anaconda as my default Python 3.7`
    - Tunggu hingga instalasi selesai

- Jalankan `Anaconda Prompt`

### **Mac user**
- Download miniconda untuk Python 3.7
    - Klik link ini untuk download: [Miniconda Mac OS X 64-bit](https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.pkg)
    - Note: skip step ini apabila kamu sudah menggunakan Anaconda sebelumnya. Walau demikian, saya akan jelaskan alasan kenapa kamu sebaiknya menggunakan miniconda nanti di course ini.

- Install miniconda
    - Install tanpa mengubah opsi apapun
    - Tunggu hingga instalasi selesai

- Jalankan terminal

### **Linux user**
- Download miniconda untuk Python 3.7
    - Klik link ini untuk download: [Miniconda Linux 64-bit](https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh)
    - Note: skip step ini apabila kamu sudah menggunakan Anaconda sebelumnya. Walau demikian, saya akan jelaskan alasan kenapa kamu sebaiknya menggunakan miniconda nanti di course ini.
    
- Install miniconda
    - jalankan terminal
    - Install miniconda menggunakan command berikut
        ```
        bash Miniconda3-latest-Linux-x86_64.sh
        ```
    - Ketik `yes` untuk agree dengan license nya, kemudian `yes` lagi untuk `prepend miniconda install location to PATH`
    - Tunggu hingga instalasi selesai
    
- hanya untuk memastikan, tutup dan buka terminal lagi

## Step 3: Instalasi Jupyter 
- Kita akan install 2 hal di base environment
    ```
    conda install --name base jupyter nb_conda_kernels
    ```

## Step 4: Instalasi Environment
- Change directory `cd` ke folder kerja ini
    ```
    cd unstructured_data/
    ```
- Jalankan command ini untuk menginstall environment `jcop_ud`
    ```
    conda env create -f env_jcop_ud.yml
    ```

## Step 5: Memastikan environment terinstall dengan baik
- Jalankan command berikut untuk mengecek instalasi dan ikuti instruksi yang dihasilkan
    ```
    python check_installation.py
    ```
- Jika sudah aman, maka akan muncul keterangan berikut, dan kita bisa mulai belajar. Semangat!
    ```
    ✓ jupyter telah terinstall dengan baik
    ✓ nb_conda_kernels telah terinstall dengan baik
    ✓ Environment jcop_ud terdeteksi
    ✓ Package telah terinstall dengan baik di dalam environment jcop_ud
    ✓ Instalasi berjalan dengan baik. Selamat belajar!
    ```