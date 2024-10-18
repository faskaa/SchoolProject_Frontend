# Məktəb Tanıtım Veb Saytı Texniki Tapşırığı

## 1. Layihənin Məqsədi
Məktəb haqqında məlumatları təqdim edən, istifadəçi dostu və informativ bir veb sayt yaratmaq.

## 2. Funksional Tələblər

### 2.1 Ana Səhifə
- Məktəbin qısa təqdimatı
- Xəbərlər və elanlar bölməsi
- Qalereya (şəkillər və videolar)

### 2.2 Haqqımızda
- Məktəbin tarixi
- Missiya və vizyon
- Rəhbərlik və müəllim heyəti

### 2.3 Təhsil Proqramları
- Təklif olunan proqramların siyahısı
- Hər proqram üçün ətraflı məlumat

### 2.4 Tələbə Həyatı
- Dərsdənkənar fəaliyyətlər
- Tələbə klubları
- İdman imkanları

### 2.5 Qəbul
- Qəbul prosesi haqqında məlumat
- Online müraciət forması
- Tez-tez verilən suallar (FAQ)

### 2.6 Əlaqə
- Əlaqə məlumatları
- Xəritə
- Əlaqə forması

### 2.7 İnzibati Panel
İnzibati panel, sayt administratoruna veb saytın bütün məzmununu və funksiyalarını idarə etmək imkanı verən mərkəzləşdirilmiş bir idarəetmə sistemidir.

#### 2.7.1 Admin Girişi və Təhlükəsizlik
- Təhlükəsiz giriş sistemi (istifadəçi adı və güclü şifrə tələbi)
- İkifaktorlu autentifikasiya (2FA)
- Şifrə sıfırlama və yeniləmə funksiyası
- Giriş cəhdlərinin jurnalı və şübhəli fəaliyyətlərin izlənməsi
- Avtomatik çıxış (session timeout) funksiyası

#### 2.7.2 Məzmun İdarəetməsi
- Xəbərlər və elanların yaradılması, redaktəsi və silinməsi
- Statik səhifə məzmununun redaktəsi (məsələn, "Haqqımızda", "Təhsil Proqramları")
- Qalereya idarəetməsi: şəkil və videoların yüklənməsi, təşkili və silinməsi
- Faylların idarə edilməsi: sənədlərin, təqdimatların yüklənməsi və təşkili

#### 2.7.3 Tədris Proqramı İdarəetməsi
- Təhsil proqramlarının əlavə edilməsi, redaktəsi və silinməsi
- Müəllim məlumatlarının idarə edilməsi (ad, soyad, fənn, qısa bio)
- Dərs cədvəllərinin əlavə edilməsi və yenilənməsi

#### 2.7.4 Tələbə Həyatı Bölməsi İdarəetməsi
- Dərsdənkənar fəaliyyətlərin əlavə edilməsi və yenilənməsi
- Tələbə klublarının siyahisinin idarə edilməsi
- İdman tədbirlərinin və nailiyyətlərin paylaşılması

#### 2.7.5 Qəbul Prosesi İdarəetməsi
- Online müraciət formasının redaktə edilməsi
- Daxil olan müraciətlərin siyahısının görüntülənməsi və idarə edilməsi
- Qəbul statistikalarının izlənməsi

#### 2.7.6 Əlaqə və Sorğu İdarəetməsi
- Əlaqə forması vasitəsilə gələn sorğuların görüntülənməsi və idarə edilməsi
- Cavablanmış və cavablanmamış sorğuların filtrlənməsi

#### 2.7.7 SEO və Analitika
- Səhifələr üçün meta teqlərin və açar sözlərin idarə edilməsi
- Google Analytics hesabatlarının inteqrasiyası və görüntülənməsi
- Sayt xəritəsinin (sitemap) yenilənməsi

#### 2.7.8 Sistem Parametrləri
- Saytın ümumi parametrlərinin idarə edilməsi (sayt adı, logo, əlaqə məlumatları)
- Backup yaratma və sistem bərpası funksiyaları

#### 2.7.9 Hesabat və Audit
- Admin fəaliyyətlərinin jurnalı
- Məzmun dəyişikliklərinin tarixçəsi
- Sistem performansı və ziyarətçi statistikaları haqqında hesabatlar

## 3. Qeyri-Funksional Tələblər

### 3.1 Dizayn və İstifadəçi İnterfeysi
- Responsiv dizayn (mobil, tablet və desktop uyğunluğu)
- Məktəbin korporativ kimliyi ilə uyğunlaşdırılmış rəng sxemi

### 3.2 Performans
- Səhifə yüklənmə müddəti: maksimum 3 saniyə
- Eyni anda ən azı 1000 istifadəçini dəstəkləmək

### 3.3 Təhlükəsizlik
- HTTPS protokolunun istifadəsi
- SQL injection və XSS hücumlarına qarşı qorunma
- Admin giriş məlumatlarının güclü şifrələnməsi
- Mütəmadi təhlükəsizlik auditləri və yeniləmələri
- Giriş cəhdlərinin məhdudlaşdırılması (rate limiting)

### 3.4 Uyğunluq
- GDPR tələblərinə uyğunluq
- Əlilliyi olan istifadəçilər üçün əlçatanlıq (WCAG 2.1 standartları)

## 4. Texniki Spesifikasiyalar

### 4.1 Front-end
- HTML5, CSS3, JavaScript
- Responsive framework (məsələn, Bootstrap)

### 4.2 Back-end
- C# proqramlaşdırma dili
- .NET Core framework
- Entity Framework Core (ORM)
- ASP.NET Core MVC

### 4.3 Verilənlər Bazası
- Microsoft SQL Server

### 4.4 Hosting
- Microsoft Azure və ya Amazon Web Services (AWS)
- Yüksək əlçatanlıq və avtomatik miqyaslandırma konfiqurasiyası
- CDN (Content Delivery Network) inteqrasiyası

### 4.5 Versiya İdarəetmə və CI/CD
- Git (GitHub və ya Azure DevOps)
- Avtomatlaşdırılmış build və deployment prosesləri
- Continuous Integration və Continuous Deployment (CI/CD) pipelines

## 5. Test və Keyfiyyət Təminatı
- Unit testlər
- İnteqrasiya testləri
- İstifadəçi qəbul testləri (UAT)

## 6. Təhvil və Dəstək
- Mərhələli təhvil planı
- İstifadəçi təlimatları və sənədləşdirmə
- 6 ay texniki dəstək və xidmət müqaviləsi

## 7. Layihə Strukturu

### Frontend

- `FrontEndSource/`
  - `Admin/`
    - `homepage.html`: İnzibati panel ana səhifəsi
    - `assets/`: CSS, JavaScript və şəkil faylları
  - `Public/`: İctimai istifadəçilər üçün səhifələr

### Backend

- `BackEndSource/`
  - `Controllers/`
  - `Models/`
  - `Views/`
  - `Services/`

## 8. Əlavə Qeydlər

- İnzibati panel ana səhifəsi (`homepage.html`) hazırlanmışdır və dashboard funksionallığını əks etdirir.
- Növbəti addımlar digər inzibati panel səhifələrinin və ictimai istifadəçi interfeyslərinin hazırlanmasını əhatə edəcək.
