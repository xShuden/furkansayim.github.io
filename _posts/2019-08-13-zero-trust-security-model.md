---
layout: post
title:  "Zero Trust Güvenlik Modeli Nedir?"
categories: "Docker"
description: "Zero Trust Güvenlik Modeli'ni anlamak"
---

Zero Trust güvenlik, John Kindervag ve Forrester Research Inc. tarafından 2009 yılında geliştirilen bir kavramdır. ([Forrester](http://www.virtualstarmedia.com/downloads/Forrester_zero_trust_DNA.pdf))

Zero Trust ağ mimarisi olarak da adlandırılan Zero Trust güvenliği fikri, son yirmi, otuz yıl boyunca geleneksel "çevre temelli (perimeter-based)" güvenlik mimarisine tamamen zıt bir bakış açısıdır. Son kimlik ihlalleriyle birlikte sağlayıcılar ve analistler, Zero Trust güvenlik modelinin taviz vermeden çalışıp çalışmayacağını merak ediyorlar.

BT kuruluşları, ağları etrafında bir "Sur" oluşturur ve sonrasında bilgisayar korsanlarının üstesinden gelmek, onlarla mücadele etmek için güvenlik katmanları oluştururlar. Ağın merkezi en kritik varlıklara sahip olmalı (veriler, uygulamalar vs.) ve teoride derinlemesine savunma yaklaşımı, bilgisayar korsanlarının onlara ulaşmasını zorlaştıracaktır. Bu güvenlik yaklaşımı, yalnızca çevre katmanlara değil, aynı zamanda merkezin içinde çalışan kullanıcılara da açıkca güvenmemeyi içerir.

Modern çağda, bilgisayar korsanları her yerdeler ve geleneksel güvenlik yöntemleri onları durdurmaya yetmiyor. Giderek daha fazla bilgisayar korsanı oluşuyor ve bu kişiler hem içeriden hem de dışarıdan ağlara saldırıyorlar. Forrester’ın Zero Trust güvenlik modelinin geliştirilmesi konusunda 2011-2012 yılları arasında yayınlanmış olan [NIST raporunda](https://www.nist.gov/sites/default/files/documents/2017/06/05/040813_forrester_research.pdf) en yaygın güvenlik ihlali kaynaklarını göstermektedir. Bu saldırıların neredeyse %50'si bir kuruluşun içinden kaynaklanırken, yalnızca %25'i dış kaynaklardan kaynaklanıyor. Başka bir deyişle, bugün dünya üzerinde yer alan bir kuruluş içerisinde, kuruluşun dışına kıyasla daha fazla güvenlik tehdidi bulunuyor. 

*Akıllardaki diğer bir soruyu sormanın vakti geldi. Bu gerçeklere rağmen geleneksel çevre tabanlı (perimeter-based) güvenlik modeli halen işe yarıyor mu?*

Standart bir ağda en dışta yer alan güvenlik önlemleri kritik noktaları koruma konusunda işini tam olarak yapamazlar. Fakat Zero Trust güvenlik modeli en dışta yer alan güvenlik önlemlerine dayanmaz. Zero Trust güvenliğinin ardındaki zihniyet, hem harici hem de dahili tüm ağ trafiği kaynaklarını potansiyel saldırı vektörleri olarak görür. Bu nedenle, tüm kullanıcılar ve kaynaklar doğrulanmalıdır. Sistem verileri toplanmalı ve analiz edilmelidir. Ağ erişimi ve trafiği sınırlı tutulmalı ve izlenmelidir. 

Mimari biraz paranoyakca görünebilir. Zero Trust güvenliği bulut çağının gerçeklerinden kaynaklanıyor. 

Günümüzde veri ve uygulamalar, SaaS sağlayıcıları ve bulut altyapısı ile doğrudan internette saklanmaktadır. Kullanıcılar dünyanın her yerinde bulunur ve BT kaynaklarına erişebilmeleri gerekir. Şirket içi ağlar, geçmişe göre daha çok WiFi'si bulunan internet kafelere benziyorlar. Hackerların artık güvenlik önlemi katmanları arasına adım atmasına gerek yok. Bunun yerine, hedefli doğrudan seçebiliyorlar. 

BT organizasyonları, özellikle kullanıcı kimliklerini doğrulamak konusunda koruma yolları düşünüyorlar. Son zamanlarda, tüm ihlallerin %81'inden fazlasının kimlik ihlallerinden ([CSO](https://www.cso.com.au/mediareleases/29642/hacked-passwords-cause-81-of-data-breaches/)) kaynaklandığı bildirildi. Bu yüzden, tamamen güvensizlik dediğimiz bir şey olsaydı bu kimlikler(hesaplar) olurdu. Ancak sadece kimlikleri ortadan kaldıramayız. Gerekli olan her türlü BT kaynağına erişmek için hepimizin kimlik bilgilerine ihtiyacımız var. Öyleyse, Zero Trust güvenlik modeli, en çok sızma yöntemi olarak kabul edilen kimlik ihlali gerçeğine karşı nasıl çalışıyor?

BT güvenlik uzmanları, bu sorunu çözebilecek bir dizi kimlik güvenliği uygulaması geliştirmektedir. Kimlik doğrulamanın en basit ve en güçlü yolu, çok faktörlü bir kimlik doğrulama (MFA(2FA) yaklaşımından yararlanmaktır. Makinelerin yanı sıra uygulamalar için ikinci bir faktör gerekmesi, yalnızca sızan kimlik bilgilerinin erişim sağlamak için yeterli olmayacağından emin olarak büyük bir risk seviyesini ortadan kaldırıyor.

MFA yeteneklerini güçlü şifreler ve SSH anahtarları ile güçlendirdiğinizde, kimlik ihlali olasılığını azaltabilirsiniz. Kimlik doğrulamada önemli adımlar atmanın yanı sıra keskin bir internet politikasına sahip BT kuruluşları, Zero Trust güvenlik modelini benimseyip kimlik yönetimine uygulayabilirler. 

### Kaynaklar

* [CSO](https://www.cso.com.au/mediareleases/29642/hacked-passwords-cause-81-of-data-breaches/)
* [PaloAltoNetworks](https://www.paloaltonetworks.com/cyberpedia/what-is-a-zero-trust-architecture)
* [Cloudflare](https://www.cloudflare.com/learning/security/glossary/what-is-zero-trust/)
* [Centrify](https://www.centrify.com/education/what-is-zero-trust-privilege/)
* [Forcepoint](https://www.forcepoint.com/cyber-edu/zero-trust)