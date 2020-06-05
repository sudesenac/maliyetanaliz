#!/usr/bin/python
# -*- coding: utf-8 -*-

adet = int(input("Lütfen Adet Giriniz: "))
malzemeGideri = int(input("Lütfen Malzeme Giderini Giriniz: "))
iscilikGideri = int(input("Lütfen İşçilik Giderini Giriniz: "))
degiskenGUG = int(input("Lütfen Değişen Genel Üretim Giderleri Giriniz: "))
sabitGugDirekt = int(input("Lütfen Sabit Dİrekt Genel Üretim Giderleri Giriniz: "))
sabitGugOrtak = int(input("Lütfen Sabit Ortal Genel Üretim Giderleri Giriniz: "))
satinAlinma = int(input("Lütfen Satın Alınma Fiyatını Giriniz: "))


def hesaplama(adet, malzemeGideri, iscilikGideri, degiskenGUG, sabitGugDirekt, sabitGugOrtak, satinAlinma):
toplam = (adet*malzemeGideri) + (adet*iscilikGideri) + (adet*degiskenGUG) + (adet*sabitGugDirekt) + (adet*sabitGugOrtak)
if toplam>satinAlinma:
print("Malzemeyi dışarıdan satın alın")
else:
print("Malzemeyi işletmede üretin")


hesaplama(adet, malzemeGideri, iscilikGideri, degiskenGUG, sabitGugDirekt, sabitGugOrtak, satinAlinma)
