# Week3Assignment

---

## Symfony kullanmanın avantajları nedir?

- Hızlı uygulama geliştirme
- Yeniden Kullanılabilir Bileşenlerin (Components) kullanımı
- Symfony, geliştiricilerin yenilik yapmasına yardımcı olur
- Önbellek (Caching) yönetimi
- Açık kaynak ve bol kaynaklı bir framework

---

## Symfony ile environment (ortam) ayarlaması nasıl yapılır?

- Kullanacağımız symfony 5.4 versiyonu için gereken ortamı:
  - `PHP 7.2.5` versiyonu ya da daha yüksek bir bir versiyon, sistemde yüklediğin `PHP` versiyonu (`Ctype`, `iconv`, `JSON`, `PCRE`, `Session`, `SimpleXML`, ve `Tokenizer`) bulundurması gerekiyor.
  - Sistemde `composer` yüklü olmalı, `PHP` paketleri yüklemek için kullanılır
  - `Symfony CLI` de yüklemek gerekir.
  ```
  scoop install symfony-cli
  ```
  Sistemde symfony ortamını kontrol etmek için
  ```
  symfony check:requirements
  ```
  ve sonra `symfony` veya `composer` ile proje oluşturabilir.

---

## Yeni bir Symfony projesi oluşturmak için kullanılan composer komutu nedir? Alternatif bir komutla Symfony projesi oluşturabilir miyiz?

- Symfoni 5.4 versiyonu projesi `composer` ya da `symfony new` ile oluşturabiliriz

```
// composer ile geleneksel web tabanlı proje oluşturmak
$ composer create-project symfony/skeleton:"^5.4" my_project_directory
$ cd my_project_directory
$ composer require webapp

// Eğer microservice, console uygulaması ya da API oluşturmak istiyorsan aşağıdakı komut ile yapılır
$ composer create-project symfony/skeleton:"^5.4" my_project_directory


// symfony ile yeni proje oluşturmak
// geleneksel web tabanı projesi
$ symfony new my_project_directory --version=5.4 --webapp

// microservice, console uygulaması veya API
$ symfony new my_project_directory --version=5.4

```

---

## Laravel framework ve Symfony framework arasındaki temel farklardan iki tanesini yazınız.

- `Laravel` ve `Symfony` framework'ler ikisi yazılım dili olarak `PHP` kullanılır.
- `Laravel` MVC kullanılır bu ise daha az enseklik yapar, `Symfony` bileşenleri kullanabilirliği kolay olduğu için kodun düzenlemesi kolaydır.
- `Laravel` şablon (template) olarak `Blade` kullanılır, `Symfony` ise `Twig`. `Blade` kod kullanabilirliğini izin verir, `Twig` ise vermiyor.
