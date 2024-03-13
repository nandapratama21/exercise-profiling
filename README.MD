<h1> MODUL 5 </h1>

Nama : Muhammad Nanda Pratama
NPM : 2206081654  
Kelas : Pemrograman Lanjut A


Reflection (sesuai dengan 7 nomor di soal)
---


1. Perbedaan cara pendekatan _performance_ JMeter dengan Intellij Profiler yaitu:  
- JMeter mengukur _performance_ aplikasi dengan mensimulasikan banyak pengguna yang menggunakan aplikasi tersebut.
- Intellij Profiler mengukur _performance_ aplikasi dengan menemukan _bottleneck_ pada program aplikasi yang menyebabkan aplikasi berjalan lebih lambat.

2. Proses _profiling_ ini sangat membantu saya untuk mengidentifikasi bagian kode apa yang membuat aplikasi berjalan lebih lambat. Dari hal tersebut, saya bisa melihat penggunaan _resource_ yang digunakan seperti CPU Usage, _concurrency_, dan aktivitas dari _garbage collector).    
  
3. Menurut saya, IntelliJ Profiler sangat efektif untuk mengidentifikasi bagian kode apa yang membuat aplikasi berjalan lebih lambat dan bagian yang _bottleneck_.IntelliJ Profiler terdapat grafik yang menunjukkan aktivitas _hardware_ selama program berjalan, contohnya seperti CPU Time.
4. Tantangan saya dalam melakukan _performance testing_ dan _profilling_ adalah saya harus memahami mengapa bagian kode yang _bottleneck_ tersebut bisa terjadi, dan saya pun memikirkan bagaimana cara mengatasi solusi dari permasalahan tersebut, salah satunya yaitu dengan menggunakan _refactoring_.
5. Manfaat utama yang saya dapatkan setelah menggunakan IntelliJ Profiler adalah saya bisa menganalisis performa aplikasi secara _runtime_ dan melihat bagian kode apa yang paling berpengaruh terhadap performa aplikasi.
6. Selama saya menggunakan dua aplikasi tersebut, saya tidak menemukan adanya inkonsistensi pada hasil yang diberikan. Namun, jika hal tersebut terjadi, saya akan menganalisis lebih lanjut mengapa hal tersebut bisa terjadi, melalui pencarian di _website_ yang memiliki ahli dalam bidang tersebut.
7. Strategi saya dalam mengoptimisasi kode setelah melihat hasil dari JMeter dan IntelliJ Profiler adalah dengan menggunakan pendekatan Query pada method findStudentWithHighestGpa, menggunakan StringBuilder pada method joinStudentNames, dan menggunakan pendekatan HashMap dan mengurangi kompleksitas loop pada method getAllStudentsWithCourses.

<h1>Hasil Analisis Performance</h1>

<h2>Endpoint /all-student </h2>

Jmeter Result:
![Screenshot 2024-03-13 at 11.24.38.png](screenshot%2FAfter%20Refactor%2FScreenshot%202024-03-13%20at%2011.24.38.png)

Before Optimized:
![Screenshot 2024-03-13 at 00.20.39.png](screenshot%2FBefore%20Refactor%2FScreenshot%202024-03-13%20at%2000.20.39.png)

After Optimized:
![Screenshot 2024-03-13 at 10.47.12.png](screenshot%2FAfter%20Refactor%2FScreenshot%202024-03-13%20at%2010.47.12.png)

Dapat dilihat bahwa setelah di optimized, status warning berbuah menjadi Success

<h2>Endpoint /all-student-name </h2>

Jmeter Result:
![Screenshot 2024-03-13 at 11.24.12.png](screenshot%2FAfter%20Refactor%2FScreenshot%202024-03-13%20at%2011.24.12.png)

Before Optimized:
![Screenshot 2024-03-13 at 00.22.40.png](screenshot%2FBefore%20Refactor%2FScreenshot%202024-03-13%20at%2000.22.40.png)

After Optimized:
![Screenshot 2024-03-13 at 10.48.24.png](screenshot%2FAfter%20Refactor%2FScreenshot%202024-03-13%20at%2010.48.24.png)

Dapat dilihat bahwa setelah di optimized, status warning berbuah menjadi Success

<h2>Endpoint /highest-gpa </h2>

Jmeter Result:
![Screenshot 2024-03-13 at 11.25.23.png](screenshot%2FAfter%20Refactor%2FScreenshot%202024-03-13%20at%2011.25.23.png)

Before Optimized:
![Screenshot 2024-03-13 at 00.23.37.png](screenshot%2FBefore%20Refactor%2FScreenshot%202024-03-13%20at%2000.23.37.png)

After Optimized:
![Screenshot 2024-03-13 at 10.47.56.png](screenshot%2FAfter%20Refactor%2FScreenshot%202024-03-13%20at%2010.47.56.png)

Dapat dilihat bahwa setelah di optimized, status warning berbuah menjadi Success

