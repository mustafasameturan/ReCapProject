# RentACarProject

## ☑️Teşekkür 
Öncelikle bana bu projeyi yazmamda büyük desteği olan, bana çok değerli bilgiler katan Engin Demiroğ Hocama teşekkür ediyorum. Ayrıca bu yolda bana destek olan arkadaşlarıma ve aileme de teşekkürlerimi iletiyorum.

## ☑️Amaç
Projeyi yazmamdaki amacımdan bahsetmek istiyorum çünkü bunu projeyi daha anlamlı kılacak bir unsur olarak görüyorum. Başlıca amacım C# dilini, .NET dünyasını tanımak, bu yolda uzmanlaşmaktır. Yazdığım bu proje kendimi geliştirmeme vesile oluyor. Ayrıca bu proje ile birlikte SOLID yazılım tekniklerini öğreniyorum. Yazılım Geliştirici olma yolunda ilerlerken temelimi sağlam atmaya çalışıyorum ve sadece kendi penceremden değil, bu projeyi okuyacak, üstünde çalışacak insanların penceresinden de bakarak çalışmalarıma devam ediyorum.

## ☑️Tanıtım
Projem adından da anlaşılacağı üzere bir araba kiralama sistemidir. Projemde, kendi oluşturduğum database üzerinden gelen bilgileri yönlendirerek;<br>

• Araba Ekle/Sil/Güncelle/Listele<br>
• Araba Gücü(HP) Ekle/Sil/Güncelle/Listele<br>
• Marka Ekle/Sil/Güncelle/Listele<br>
• Renk Ekle/Sil/Güncelle/Listele<br>
• Kullanıcı Ekle/Sil/Güncelle/Listele<br>
• Müşteri Ekle/Sil/Güncelle/Listele<br>
• Araba Kiralama Özelliği<br>

gibi imkanlar mevcuttur. Ayrıca projem bir katmanlı mimaridir. Projemin katmanlı mimarisi sayesinde kodun anlaşılabilirliği yüksektir. Tüm yazılan kodlar bir düzen içerisinde çalışmaktadır. Projemde kullandığım teknolojilerden bahsedeceğim fakat öncesinde sizden talep edilen farklı bir teknoloji kullanmak istediğinizde, projem herhangi bir zorluk yaratmayacaktır. Tamamen "Plug and Play" prensipi göz önüne alınarak tasarlanmıştır. WebAPI arabirimi kullanılmıştır ve IoC Contanier tekniği kullanılmıştır.

![Katmanlı Mimari](https://user-images.githubusercontent.com/77546366/108605441-21567d80-73c5-11eb-9536-fa39515740d4.PNG) 

## ☑️Kullanılan Teknolojiler
• Database → SQL
• Köprü → EntityFramework
• IoC Container → Autofac
• Arabirim → WebAPI
• Katmanlar → Business,DataAccess,Entity,Core,ConsoleUI

![Katmanlar](https://user-images.githubusercontent.com/77546366/108605460-3df2b580-73c5-11eb-9180-1cd05041a560.PNG)

## ☑️SQL Tables

<table>
  <tr>
    <td>Cars</td>
     <td>Brands</td>
     <td>Colors</td>
     <td>Powers</td>
  </tr>
  <tr>
    <td>

Variable Name | Data Type
------------ | -------------
CarId | int
BrandId | int
ColorId | int
ModelYear | nchar(10)
DailyPrice | decimal
Description | nvchar(30)
Model | nchar(20)
   
   </td>
    <td>

Variable Name | Data Type
------------ | -------------
ColorId | int
ColorName | nchar(10)
   
   </td>
    <td>

Variable Name | Data Type
------------ | -------------
BrandId | int
BrandName | nchar(12)
   
   </td>
   <td>
  
Variable Name | Data Type
--------------|--------------
PowerId | int
BrandId | int
CarId | int
HorsePower | nchar(4)  
  
   </td>
  </tr>
 </table>
 
 <table>
  <tr>
    <td>Customers</td>
     <td>Rentals</td>
     <td>Users</td>
  </tr>
  <tr>
    <td>

Variable Name | Data Type
------------ | -------------
CustomerId | int
UserId | int
CompanyName | nchar(40)
   
   </td>
    <td>

Variable Name | Data Type
------------ | -------------
RentalId | int
CarId | int
CustomerId | int
RentDate | datetime
ReturnDate | datetime

   </td>
    <td>

Variable Name | Data Type
------------ | -------------
UserId | int
FirstName | nchar(25)
LastName | nchar(20)
Email | nchar(50)
Password | nchar(20)

   </td>
  </tr>
 </table>

## ☑️Son Güncellemeler
• Autofac Desteği eklendi.

