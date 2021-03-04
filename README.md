[![Netlify Status](https://api.netlify.com/api/v1/badges/9a01b648-edcb-4792-bf7a-b487f6cc44f2/deploy-status)](https://app.netlify.com/sites/blog-apeven/deploys)

### This hugo theme was created by using Narative's Novella theme ported by Forestry to Hugo, translated to Turkish.

-[Visit Narative](narative.co)
-[Visit Forestry](forestry.io)

### Bu hugo teması Narative'in Novella temasının Forestry tarafından Hugo'ya portunun Türkçe'ye çevirilmesiyle oluşturulmuştur.

-[Narative'yi ziyaret et](narative.co)
-[Forestry'i ziyaret et](forestry.io)

# blog.apeven.me

Forestry'nin [Hugo Novela](https://github.com/forestryio/hugo-theme-novela) portunun geliştirilmiş ve Türkçe'ye çevrilmiş versiyonu.

## Gereksinimler

Bu  site [Hugo Module](https://gohugo.io/hugo-modules/) kullanarak yapılmıştır.

- Go versiyonu > 1.12
- Hugo versiyonu > 0.65.0 

## İçerik Yönetimi

Bu sitede [Forestry](https://forestry.io) kullanarak içeriklerinizi rahatça yönetebillirsiniz  ✨.

Sitenizde yapacağınız herhangi bir değişiklik anında git reponuza kaydolacaktır.

## Deploy on Netlify

Reponuzu [Netlify](https://netlify.com)'a aktarın

1. Netlify'da yeni bir site yaratın ve reponuzu içeri aktarın.
2. build command'ı yandaki gibi yazın: `hugo --gc --minify`
3. publish directory'i yandaki gibi yazın: `public`
4. `GO_VERSION`'u `1.12` ve üstüne ayarlayın
4. `HUGO_VERSION`'u `0.65.3` ve üstüne ayarlayın

Artık Forestry'den yaptığınız her düzenleme otomatik olarak sitenizde yayınlanacak.

## Geliştirme

```bash
# clone your repository
# cd in your project directory
# Start local server
hugo server
```

Daha fazla bilgi için :[Hugo Başlangıç Sayfası (ingilizce)](https://gohugo.io/getting-started/).

## Özelleştirme

### Logo

Preojenizin layout konumuna logonuzun SVG dosyasını ekleyin:
`/layouts/icons/ui/logo.html`

### Sosyal Hesaplar

Forestry'den sosyal hesapları düzenleyebilmek için temanın `config/_default/social.yaml` dosyasını projenize kopyalayın.

### Yazarlar

Yazarlarınızı taxonomy olarak projenizin `config.yaml` dosyasına eklemeniz gerekli.

```yaml
taxonomies:
  author: authors
```

#### Yazar profili oluşturma

Buna benzer bir dosyayı content klasörünüze ve de Front Matter'a ekleyin.

```yaml
# /content/authors/firstname-lastname/_index.md
---
title: Dennis Brotzky
bio: |
  Written by You. This is where your author bio lives. Share your work, your
  joys and of course, your Twitter handle.
avatar: /images/dennis-brotzky.jpg
featured: true
social:
  - title: github
    url: https://github.com
  - title: twitter
    url: https://twitter.com
  - title: instagram
    url: https://instagram.com
  - title: dribbble
    url: https://dribbble.com
  - title: unsplash
    url: https://unsplash.com
---
```

#### Yazarları içeriğinize ekleme

Yazarın adını "authors" kısmına ekleyin:

```yaml
authors:
  - Dennis Brotzky
  - Thiago Costa
```
### E-posta için bültene kaydolma

Bu tema, herhangi bir sayfaya ekleyebileceğiniz bir haber bülteni açıklama formu için bir kısa kod içerir.
Bu tema [formspree.io](//formspree.io/) sitesini gerçek maili göndermek için bir proxy olarak kullanıyor. Her ay ziyaretçileriniz size kendi maillerini herhangi bir ücret olmadan bin adet gönderebiliyorlar. Formspree e-postanızı aşağıdaki gibi kısa kodunuza eklemek için Formspree sitesini ziyaret edin.

```
{{< subscribe email="your@email.com" >}}
```


## LICENSE

MIT
