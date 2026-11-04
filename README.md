# Toprak Nerede?

Toprak Aydın'da mı Fethiye'de mi? Arkadaşlar bakıyor, plan seçiyor, WhatsApp'tan yazıyor.

- `index.html`: Sitenin kendisi.
- `data.json`: Toprak'ın durumu. Site bu dosyayı okur, panelden kaydedince bu dosya güncellenir.

## Kurulum (bir kere, ~10 dakika)

### 1. Repoyu aç
1. github.com → sağ üst **+** → **New repository**
2. Repository name: `toprak-nerede`
3. **Public** seç. GitHub Pages ücretsiz planda public repo ister.
4. **Create repository**

### 2. Dosyaları yükle
Repoda **uploading an existing file** linkine tıkla. `index.html` ve `data.json` dosyalarını sürükle. Sonra **Commit changes**.

(Claude'a GitHub erişimi verdiysen bu adımı Claude da yapabilir.)

### 3. Siteyi yayına al
1. Repoda **Settings** → soldan **Pages**
2. Source: **Deploy from a branch**
3. Branch: `main`, klasör `/ (root)`, sonra **Save**
4. 1-2 dakika sonra site açılır: `https://KULLANICI-ADIN.github.io/toprak-nerede/`

Bu linki arkadaşlarına at.

### 4. Kendine düzenleme anahtarı al
1. GitHub → profil fotoğrafı → **Settings** → en altta **Developer settings**
2. **Personal access tokens** → **Fine-grained tokens** → **Generate new token**
3. Ayarlar:
   - Token name: `toprak-nerede`
   - Expiration: 1 yıl (ya da istediğin süre)
   - Repository access: **Only select repositories** → `toprak-nerede`
   - Permissions → Repository permissions → **Contents: Read and write**
4. **Generate token**. Çıkan `github_pat_…` ile başlayan anahtarı kopyala.

### 5. Telefondan giriş yap
1. Siteyi telefonda aç, en alta in.
2. **Ben Toprak'ım, düzenle** butonuna dokun, anahtarı yapıştır, **Giriş yap**.

Anahtar sadece o telefonun tarayıcısında saklanır. Artık "Aydın'dayım / Fethiye'deyim" butonları, gidiş tarihleri ve planlar sende.

İpucu: Siteyi telefonda "Ana ekrana ekle" yaparsan uygulama gibi açılır.

## Bilmen gerekenler
- Arkadaşların her zaman en güncel hali görür. Site durumu doğrudan GitHub'dan okur.
- Anahtarı kimseyle paylaşma. Bu anahtar sadece bu repoyu değiştirebilir. Telefonunu kaybedersen GitHub'dan anahtarı silip yenisini al.
- WhatsApp numaranı panelden eklersen `data.json` içinde herkese açık durur.
- Anahtarın süresi dolunca panel "anahtar geçersiz" der. 4. adımı tekrarlayıp yeni anahtarla gir.
