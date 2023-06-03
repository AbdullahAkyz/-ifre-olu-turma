# -sifre-olusturma
# random modülünü içe aktarmak için
import random

# Şifrede kullanılacak karakterleri içeren bir karakter dizisi tanımlamak için
karakterler = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!@#$%^&*"

# Şifrenin uzunluğunu belirlemek için
uzunluk = 8

# Rastgele karakterler seçerek şifreyi oluşturmak için
sifre = ""
for i in range(uzunluk):
    sifre += random.choice(karakterler)

# Şifreyi ekrana yazdırmak için
print("Oluşturulan şifre:", sifre)

# Şifreyi bir dosyaya kaydetmek için
dosya = open("sifre.txt", "w")
dosya.write(sifre)
dosya.close()

