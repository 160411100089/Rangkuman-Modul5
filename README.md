# Rangkuman-Modul5

Recursif
Rekursif ini sebenarnya merupakan sebuah perulangan di dalam sebuah program
namun, perulangan ini sangat berbeda dengan perulangan pada umumnya
seperti while dan for, Walaupun fungsinya sama yaitu perulangan atau looping.
Letak perbedaannya adalah dari cara kerjanya, jika for dan while merupakan sebuah perulangan yang menggunakan sebuah kondisi atau boolean,
maka pada rekursif ini terjadi pada sebuah fungsi atau metode yang memanggil dirinya sendiri.

Iteratif
merupakan penyelesaian permasalahan dengan perulangan, menggunakan syntax for atau while (pada Python). 

Pada code ini, terdapat iterasi while, yang menghitung perkalian, mulai dari nn, sampai dengan 2.
Contoh kode:

      def factorialIteratif(bilangan):
          if bilangan <=1:
              return(1)
          else:
              temp=bilangan
              hasil=1
              while temp>1:
                  hasil=hasil*temp
                  temp=temp-1
              return(hasil)
              
      print(factorialIteratif(4))
24


Berikut adalah code untuk perhitungan faktorial dengan cara rekursif

      def factorialRekursif(bilangan):
          if bilangan <=1:
              return(1)
          else:
              return(bilangan * factorialRekursif(bilangan-1))
              
      data=factorialRekursif(4)
      print(data)
24

Dari fungsi tersebut dapat dilihat bahwa teknik pemrograman rekursif ini melibatkan pemanggilan fungsinya itu sendiri dengan argument
atau parameter yang berukuran lebih kecil. Berikut beberapa aturan dalam teknik pemrograman rekursif:
  1. Fungsi rekursif harus memiliki base case, base case inilah yang berfungsi untuk menghentikan pemanggilan terus menerus fungsi
     rekursif
  2. fungsi rekursif harus memiliki sintaks yang dapat merubah state dari permasalahan, sehingga semakin lama solusi permasalahan
     menuju base case yang sudah dibuat
  3. Fungsi rekursif harus memanggil dirinya sendiri
  
  
Implementasi Rekursif
Banyak permasalahan yang dapat diselesaikan dengan teknik pemrograman rekursif ini, berikut saya lampirkan contoh 
kode programnya:

code untuk menghitung triangular numbers melalui teknik iteratif

      def triangularNumbers1(n):
          total=0
          temp=n
          while temp>=1:
              total+=temp
              temp-=1
          return(total)
          
      print(triangularNumbers1(2))
  3


Untuk mencari deret ke-nn dari triangular numbers, dapat juga digunakan fungsi rekursif seperti permasalahan perhitungan faktorial
sebelumnya. Base case dari triangular numbers ini adalah ketika deret ke-1 yang bernilai 1.
Berikut fungsi rekursif dari triangular numbers.

      def triangularNumbers2(n):
          if n==1:
              return(1)
          else:
              return (n + triangularNumbrs2(n-1))
              
print(triangularNumbers1(8))



Konversi Bilangan
suatu proses dimana satu system bilangan dengan basis tertentu akan dijadikan bilangan dengan basis yang lain.
