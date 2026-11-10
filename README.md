import random
digits = "+-/*!&$#?=@abcdefghijklnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890"
parola = ""
while True:
    parola_uzunl = int(input("Parola uzunluğunu girin:   "))
    person = int(input("Kaç tane şifre lazım?"))
    parola = ""
    if parola_uzunl == 0:
        print("Sıfır karakterli bir şifre olamaz!")
    for b in range(person):

        for i in range(parola_uzunl):
            harf = random.choice(digits)
            parola += harf
        print(str(b + 1) + ". Parola " + str(parola))
        parola = ""
        
