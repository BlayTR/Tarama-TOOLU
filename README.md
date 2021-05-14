# Tarama-TOOLU
Güncel tarama toolu
import os

while True:
        os.system("pkg install figlet")
        os.system("clear")
        os.system("figlet Blay")
        print("""
Gelismis Tarama Araci

1) Site Hakkinda Genel Bilgi
2) Hizli Port Tarama
3) Versiyon Bilgi
Q) Cikis


""")

        islemno =input("İslem No giriniz: ")
        if islemno=="1":
            hedefip= input("Hedef Site Giriniz: ")
            os.system("whois "+hedefip)
        elif islemno=="2":
            hedefip= input("Hedef Site Giriniz: ")
            os.system("nmap "+hedefip)
        elif islemno=="3":
            hedefip= input("Hedef Site Giriniz: ")
            os.system("nmap -sV "+hedefip)
        elif islemno=="q" or "Q":
                quit()
        else:
                input("Hatali Giris Devam Etmek İcin Enter'e Bas!")
