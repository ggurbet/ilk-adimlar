# İlk Adımlar
Bir işe başlarken ilk adımı atmak genelde en zorudur. Burada açık kaynak bir projeye ilk adımı atarken kolaylaştırıcı bir ortam sunmayı amaçladım.

**NOT:** Burada kullandığım ve sizin oluşturduğunuz tüm içerikler Türkçe olacaktır.

# Nasıl?
Projede çeşitli klasörler var. Bu klasörlerde de çeşitli dosyalar var. Bulunduğunuz klasörün içeriğine göre bir dosya oluşturabilirsiniz. Örneğin [algoritmalar](algoritmalar) klasörünün altındaki farklı algoritmalara istediğiniz bir algoritmayı ekleyebilirsiniz. Algoritmanın daha önce başkası tarafından yazılmış olması veya aynı programlama dilinde yazılmış olması fark etmez! İstediğiniz kodu ekleyin! Kodun ilk satırına yorum olarak adınızı, soyadınızı ve paylaşmak istediğiniz başka bilgileri ekleyebilirsiniz.

# Kolay Bir Örnek

## 1. Projeyi Çatallayın
Sağ üstteki `Fork` (Çatalla) düğmesine tıklayarak projenin kendinize ait bir kopyasını oluşturun.

![](/resimler/catalla-dugmesi.png)

### 1.1. GitHub Web Sitesi Üzerinden
Proje sayfanızdayken [KATKICILAR.md](KATKICILAR.md) dosyasına tıkladıktan sonra dosya içeriğinizin sağ üst kısmındaki kalem düğmesine tıklayarak istediğiniz değişikliği yapabilir ve sonrasında bunu yeni bir dal (branch) oluşturacak şekilde kaydedebilirsiniz. Dal adı olarak `adiniz-soyadiniz` kullanın, örneğin `gokhan-gurbetoglu`.

### 1.2. Kendi Bilgisayarınızdan

#### 1.2.1.  Git Ayarlarınızı Yapın
Hızlıca Git ayarlarınızı yapmanızda fayda var. Bundan sonraki tüm işlerde geçerli olması için şu komutları uçbirimden çalıştırabilirsiniz:
```
git config --global user.name "Adınız Soyadınız"
git config --global user.email "e-posta@adresiniz.com"
```

**Not:** Bu şekilde ayarlarınızı yaptığınızda bundan sonraki tüm Git çalışmalarınızda bu ayarlar kullanılacaktır. Bunun yerine her deponuz için ayrı ayrı tanımlama yapmak isterseniz `--global` anahtarını kaldırabilirsiniz.

#### 1.2.2. Projeyi Klonlayın
Yeni oluşturduğunuz projeyi kendi bilgisayarınızda klonlayın. Bunun için proje sayfanızda sağ üstteki `Clone or download` (Klonla ya da indir) düğmesine tıklayın ve verilen adresi kopyalayın. Bunu adresin sağındaki kopyalama düğmesine tıklayarak da yapabilirsiniz.

Bilgisayarınızda uçbirime (terminal veya konsol da denebilir) girin ve şu komutla projenizi bilgisayarınıza klonlayın:
```
git clone kopyalanan-adres
```
Proje adınızda bir klasör oluşturulacak ve projeniz bulunduğunuz klasörün altında yer alacak.

Örneğin:
```
git clone https://github.com/ggurbet/ilk-adimlar.git
```
komutuyla klonladığınızda artık projenize `ilk-adimlar` adlı klasörden erişebilirsiniz.


#### 1.2.3. Dal (Branch) Oluşturun
Uçbirimde projenizin bulunduğu klasördeyken:
```
git checkout -b dal-adi
```
komutunu çalıştırarak `dal-adi` adında bir dal oluşturun ve bu dala geçiş yapın. Örneğin bu proje için dal adı olarak kendi adınızı ve soyadınızı girebilirsiniz:
```
git checkout -b gokhan-gurbetoglu
```

**Not:** Daha sonra ana dalınıza, örneğin `main`, dönmek için `git checkout main` ya da `git switch main` komutlarını kullanabilirsiniz.

#### 1.2.4. Katkınızı Yapın (Commit)
Artık hazırız! İlk katkımız için [KATKICILAR.md](KATKICILAR.md) dosyasının içine adınızı, soyadınızı, GitHub hesabınızı ve benzeri paylaşmak istediğiniz diğer bilgilerinizi dosyanın sonuna ekleyin ve kaydedin.
```
- [Adınız Soyadınız](https://github.com/kullanici-adiniz)
```

Örneğin:
```
- [Gökhan Gurbetoğlu](https://github.com/ggurbet)
```

Değişiklikleriniz bittiğinde uçbirimden
```
git add KATKICILAR.md
```
komutunu vererek [KATKICILAR.md](KATKICILAR.md) dosyasını değişiklikleri kaydedilmek üzere bulunduğunuz dala ekleyin. Sonra uçbirimden:
```
git commit -m "Katkıcı-Adı'nı katkıcılar listesine ekle"
```
komutunu çalıştırarak yaptığınız katkıyı işleyin. Örneğin:
```
git commit -m "Gökhan Gurbetoğlu'nu katkıcılar listesine ekle"
```

#### 1.2.5. Katkınızı Gönderin (Push)
Artık katkımızı göndermeye hazırız. Uçbirimden:
```
git push origin adiniz-soyadiniz
```
girin. Burada `adiniz-soyadiniz` yerine önceden oluşturduğunuz dalın adını yazın. Değişiklikleriniz artık GitHub'da!

## 2. İncelenmesi için Değişiklikleri Gönderin
Artık GitHub üzerinde proje sayfanıza girdiğinizde sağ üstte yeşil renkli bir `Compare & pull request` (Karşılaştır ve çekme isteği oluştur) düğmesi göreceksiniz. Bu düğmeye tıklayın, gerekli bilgileri girin ve `Create pull request` (Çekme isteği oluştur) düğmesine tıklayarak isteğinizi tamamlayın.

## 3. İncelemeniz Onaylandı!
Yukarıdaki tüm işlemleri yaptıysanız ben de çekme isteğinizi inceleyip bu projeye eklenmesi için onay vereceğim. Tebrikler! İlk katkınızı yaptınız!
