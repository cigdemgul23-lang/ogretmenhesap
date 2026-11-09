# ��retmen Hesab�m

�i�dem G�l Aslan i�in ��retmen ve ��rencilerin ayr� hesaplarla kulland��� T�rk�e �al��ma alan�.

## �zellikler

- Supabase e-posta/�ifre giri�i, e-posta do�rulama, �ifre yenileme.
- Ki�isel profil, g�nl�k g�revler, tamamlanma durumu, tarihli ders program�, �zel notlar.
- ��retmenin olu�turdu�u �devler, duyurular ve kaynak ba�lant�lar�; ��rencinin �dev tamamlanma takibi.
- Masa�st� ve telefona uyumlu aray�z.

## Yay�n

GitHub Pages: `main` dal�, `/ (root)` klas�r�. Statik dosyalar do�rudan yay�mlan�r; derleme gerekmez.

## Yetkiler ve veri

Veri Supabase'de saklan�r. Taray�c�daki anahtar public/publishable anahtard�r; sunucu anahtar� kullan�lmaz. T�m uygulama tablolar�nda sat�r d�zeyi g�venlik aktiftir. Kullan�c� profili, ajanda ve tamamlanma durumu yaln�zca sahibine a��kt�r. Payla��mlar b�t�n kay�tl� kullan�c�lar taraf�ndan okunabilir; s�n�f etiketleri eri�im k�s�t� de�ildir. Yaln�zca `app_private.teachers` tablosunda tan�ml� hesaplar payla��m olu�turabilir.

��retmen yetkisi y�netici taraf�ndan do�rulanan hesaba verilir; kullan�c�lar kendilerine ��retmen rol� atayamaz. Yeni hesaplar ��renci olarak a��l�r. ��retmen rol� verilince ��k�� yap�p yeniden giri� yapmak veya sayfay� yenilemek yeterlidir.

Supabase Auth URL Configuration b�l�m�nde Site URL ve izin verilen y�nlendirme URL'si yay�n adresiyle e�le�melidir. �ifre s�f�rlama ve kay�t do�rulama ba�lant�lar� ayn� uygulamaya d�ner.

## Geli�tirme

Bir statik HTTP sunucusuyla klas�r� sunun. `app.js`, sabitlenmi� s�r�ml� Supabase JS istemcisini esm.sh'den kullan�r. Google Fonts y�klenemezse sistem yaz� tipleri devreye girer. Veritaban� yap�s� `schema.sql` i�indedir; yeniden uygulamak i�in tasarlanmam��t�r.

