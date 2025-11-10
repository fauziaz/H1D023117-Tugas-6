# Flutter Passing Data

Nama: Fauzia Azahra Depriani  
NIM: H1D023117  
Shift Lama: D  
Shift Baru: F  

---

## ⚙️ Cara Kerja Parsing Data
1. **User mengisi form** di `form_data.dart`
   - Data nama, nim, umur diambil dari `TextEditingController`
   - Umur dihitung otomatis:  
     ```dart
     int umur = DateTime.now().year - tahunLahir;
     ```

2. **Navigasi ke halaman tampil data**
   - Data dikirim lewat constructor ke `TampilDataPage`:
     ```dart
     Navigator.push(
       context,
       MaterialPageRoute(
         builder: (context) => TampilDataPage(
           nama: nama,
           nim: nim,
           umur: umur,
         ),
       ),
     );
     ```

3. **Halaman `tampil_data.dart` menerima data**
   - Data ditampilkan dalam bentuk teks:
     ```dart
     Text('Nama saya $nama, NIM $nim, dan umur saya adalah $umur tahun');
     ```

---

## 📸 Screenshot
<p align="center">
   <img src="https://github.com/user-attachments/assets/1811e3f3-4d72-44a2-8d2f-b7fa6123ed79" width="250" style="margin:15px;">
   <img src="https://github.com/user-attachments/assets/f0dfdcd7-abc1-427f-9deb-c984cdfea2f6" width="250" style="margin:15px;">
</p>

---

## 🎥 Demo Aplikasi
https://github.com/user-attachments/assets/084869aa-82c9-4a66-8162-b33d6f07ebcc
