# dic-info - Doğa İçin Çal Bilgileri

### Doğa İçin Çal Nedir ? 

> Fırat Çavaş direktörlüğünde yapılan doğa için bir farkındalık oluşturma amacı güden bir projedir.
> Bu farkındalığı yapabildikleri en iyi ve en güzel şeyle, müzikle yapıyorlar.

### dic-info Nedir ?

> Doğa İçin Çal projesinde yer alan tüm sanatçıların düzgün bir şekilde kayıt altına alınmasını sağlayan bir projedir.

### Kullanım

> dic-info.json dosyasında tüm bilgiler yer almaktadır.
> İstediğiniz yerde, istediğiniz şekilde kullanabilirsiniz.

### Json Veri Yapısı

```c#
// Artist Class
public class Artist
{
    public string name { get; set; }
    public string country { get; set; }
    public string city { get; set; }
    public List<string> project { get; set; }
}

// Dic Class
public class Dic
{
    public string code { get; set; }
    public string name { get; set; }
    public List<string> song { get; set; }
    public string year { get; set; }
    public string director { get; set; }
    public List<Artist> artist { get; set; }
}

// Root Class
public class RootObject
{
    public List<Dic> dic { get; set; }
}
```