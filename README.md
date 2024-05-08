## Tutorial 1 Module 10

### 1.2 Understanding how it works
![alt text](images/1_2.png)
Pada gambar tersebut, terliath bahwa `println!("Zuhdy's Computer: hey hey!");` langsung dieksekusi langsung setelah spawner.spawn dipanggil. Jl ini menunjukkan bahwa statement tersebut bukan merupakan sebuah async, sehingga tidak perlu menunggu hasil dari async task untuk dieksekusi.

Sedangkan disisi lain, async block akan dijalankan secara async, tetapi menunggu `println!("Zuhdy's Computer: hey hey!");` selesai dieksekusi dikarenakan block tersebut dieksekusi secara langsung.