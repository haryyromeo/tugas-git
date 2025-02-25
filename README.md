# tugas-git
## 1.1. Import library pandas beri nama pd
  import pandas as pd
## 1.2. Baca data file nba terlampir simpan dengan nama dataku
  df=pd.read_csv(r"C:\Kuliah\Semester 4\Machine Learning\nba.csv")
## 1.3. Tampilkan isi dataku
  df
## 1.4. Berapa ukuran dataku (jumlah baris dataku dan jumlah kolom dataku)? 
  df.shape
## 1.5. Tampilkan informasi dari dataku (info)
  df.info()
## 1.6. Berapa banyaknya kolom dari dataku
  df.shape[1

##2.1. Tampilkan data awal dari dataku (gunakan head)
  df.head()
##2.2. Tampilkan data terakhir dari dataku (gunakan tail)
  df.tail()
##2.3. Tampilkan 20 data teratas dari dataku dari column Name
  df["Name"].head(20) 
##2.4. Tampilkan 10 data teratas dari column Name dan Age, simpan hasilnya dengan nama "
  data_teratas = df[["Name", "Age"]].head(10)

  data_teratas.to_csv("data_teratas.csv", index=False)

  print(data_teratas)

##2.5. Tampilkan 10 data terbawah dari column Name. Simpan hasilnya dalam variable "bottom10
  bottom10 = df["Name"].tail(10)

  print(bottom10)
