<!DOCTYPE html>
<html lang="az">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Əlaqə - Kiber Təhlükəsizlik</title>
  <link rel="stylesheet" href="style.css">
  <link rel="stylesheet" href="../dil-secim.css">
  <script src="../translations.js" defer></script>
  <script src="script.js" defer></script>
</head>
<body>
  <nav class="navbar">
    <div class="nav-logo">
      <span class="logo-icon"><svg viewBox="0 0 24 24" fill="none" stroke="royalblue" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg></span>
      <div>
        <p class="logo-kiber" data-tr="logo_kiber">Kibertəhlükəsizlik</p>
        <p class="logo-kafedra" data-tr="logo_kafedra">Kafedrası</p>
      </div>
    </div>
    <div class="nav-right">
    <ul class="nav-links">
      <li><a href="../index.html" data-tr="nav_ana">Ana səhifə</a></li>
      <li><a href="../Haqqimizda_Mehrac/index.html" data-tr="nav_haqqimizda">Haqqımızda</a></li>
      <li><a href="../Emekdaslar_Senan/index.html" data-tr="nav_emekdaslar">Əməkdaşlar</a></li>
      <li><a href="../Meqaleler_Senan_Mehrac/index.html" data-tr="nav_meqaleler">Məqalələr</a></li>
      <li><a href="../Fenler_Yusif/index.html" data-tr="nav_fenler">Fənlər</a></li>
      <li><a href="#" class="active" data-tr="nav_elaqe">Əlaqə</a></li>
    </ul>
    <div class="dil-secim">
      <button data-dil="az" onclick="dilDeyish('az')">AZ</button>
      <button data-dil="en" onclick="dilDeyish('en')">EN</button>
      <button data-dil="ru" onclick="dilDeyish('ru')">RU</button>
    </div>
    </div>
  </nav>

  <!-- sehife bashligi -->
  <section class="page-top">
    <div class="page-top-text">
      <h1 data-tr="el_h1">Əlaqə</h1>
      <p data-tr="el_sub">Bizimlə əlaqə saxlayın - hər zaman köməyə hazırıq</p>
    </div>
  </section>

  <!-- form ve elaqe melumatlari -->
  <section class="elaqe-main">
    <div class="elaqe-grid">
      <!-- sol terefde form -->
      <div class="form-box">
        <h2 data-tr="el_form_h">Mesaj Göndərin</h2>
        <form id="elaqeForm">
          <div class="form-group">
            <label for="ad"><span data-tr="el_label_ad">Ad və Soyad</span> <span>*</span></label>
            <input type="text" id="ad" data-tr-ph="el_ph_ad" placeholder="Ad və Soyadınız" required>
          </div>

          <div class="form-group">
            <label for="email"><span data-tr="el_label_email">E-mail</span> <span>*</span></label>
            <input type="email" id="email" placeholder="email@example.com" required>
          </div>

          <div class="form-group">
            <label for="movzu"><span data-tr="el_label_movzu">Mövzu</span> <span>*</span></label>
            <select id="movzu" required>
              <option value="" data-tr="el_opt_sec">Mövzu seçin</option>
              <option value="qebul" data-tr="el_opt_qebul">Qəbul prosesi</option>
              <option value="tehsil" data-tr="el_opt_tehsil">Tədris haqqında</option>
              <option value="emekdaslik" data-tr="el_opt_emek">Əməkdaşlıq</option>
              <option value="diger" data-tr="el_opt_diger">Digər</option>
            </select>
          </div>

          <div class="form-group">
            <label for="mesaj"><span data-tr="el_label_mesaj">Mesaj</span> <span>*</span></label>
            <textarea id="mesaj" rows="6" data-tr-ph="el_ph_mesaj" placeholder="Mesajınızı yazın..." required></textarea>
          </div>

          <button type="submit" class="btn-submit">
            <span class="send-icon">✈️</span> <span data-tr="el_btn_gonder">Göndər</span>
          </button>
        </form>

        <!-- gondrildikden sonra gorunecek -->
        <div class="success-msg" id="successMsg">
          <span>✓</span>
          <h3>Mesajınız göndərildi!</h3>
          <p>Tezliklə sizinlə əlaqə saxlayacağıq.</p>
        </div>
      </div>

      <!-- sag terefde elaqe melumatlari -->
      <div class="contact-info">
        <h2 data-tr="el_info_h">Əlaqə Məlumatları</h2>

        <div class="info-item">
          <div class="info-icon-box">📍</div>
          <div class="info-text">
            <h3 data-tr="el_info_unvan_h">Ünvan</h3>
            <p data-tr="el_info_unvan_p1">Azərbaycan Dövlət Universiteti</p>
            <p data-tr="el_info_unvan_p2">Kibertəhlükəsizlik Kafedrası</p>
            <p data-tr="el_info_unvan_p3">Bakı, Azərbaycan</p>
          </div>
        </div>

        <div class="info-item">
          <div class="info-icon-box">✉️</div>
          <div class="info-text">
            <h3 data-tr="el_info_email_h">E-mail</h3>
            <a href="mailto:info@cybersec.edu.az">info@cybersec.edu.az</a>
            <a href="mailto:admission@cybersec.edu.az">admission@cybersec.edu.az</a>
          </div>
        </div>

        <div class="info-item">
          <div class="info-icon-box">📞</div>
          <div class="info-text">
            <h3 data-tr="el_info_tel_h">Telefon</h3>
            <p>+994 12 123 45 67</p>
            <p>+994 12 123 45 68</p>
          </div>
        </div>

        <div class="info-item">
          <div class="info-icon-box">🕐</div>
          <div class="info-text">
            <h3 data-tr="el_info_saat_h">İş saatları</h3>
            <p data-tr="el_info_saat_p1">Bazar ertəsi - Cümə: 09:00 - 18:00</p>
            <p data-tr="el_info_saat_p2">Şənbə - Bazar: Bağlı</p>
          </div>
        </div>

        <!-- komanda shekli -->
        <div class="team-photo">
          <img src="komanda.jpg" alt="Komandamız" onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';">
          <div class="photo-placeholder">
            <span>👥</span>
            <p>Komandamız</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- FAQ - tez-tez verilen suallar -->
  <section class="faq-section">
    <h2 data-tr="el_faq_h">Tez-tez Verilən Suallar</h2>

    <div class="faq-grid">
      <div class="faq-card">
        <h3 data-tr="el_faq1_h">Qəbul şərtləri hansılardır?</h3>
        <p data-tr="el_faq1_p">Qəbul şərtləri haqqında ətraflı məlumat üçün admission@cybersec.edu.az ünvanına müraciət edə bilərsiniz.</p>
      </div>

      <div class="faq-card">
        <h3 data-tr="el_faq2_h">Təhsil haqqı nə qədərdir?</h3>
        <p data-tr="el_faq2_p">Təhsil haqqı illik olaraq müəyyən edilir və hər il yenilənir. Cari məlumat üçün bizimlə əlaqə saxlayın.</p>
      </div>

      <div class="faq-card">
        <h3 data-tr="el_faq3_h">Beynəlxalq sertifikatlar əldə edə bilərəmmi?</h3>
        <p data-tr="el_faq3_p">Bəli, tələbələrimiz CompTIA, CEH, CISSP kimi beynəlxalq sertifikatlar üçün hazırlıq görə bilərlər.</p>
      </div>

      <div class="faq-card">
        <h3 data-tr="el_faq4_h">Magistratura qəbulu necə həyata keçirilir?</h3>
        <p data-tr="el_faq4_p">Magistratura qəbulu üçün bakalavr dərəcəsi və qəbul imtahanı tələb olunur. Ətraflı məlumat üçün əlaqə saxlayın.</p>
      </div>
    </div>
  </section>

  <!-- gizli surpriz duymesi -->
  <div class="surpriz-bolme">
    <button class="surpriz-btn" data-tr="el_surpriz_btn" onclick="acSurpriz()">⭐ Müəllim üçün</button>
  </div>

  <!-- surpriz modal -->
  <div class="surpriz-modal" id="surprizModal">
    <div class="surpriz-content">
      <button class="surpriz-close" onclick="baglaSurpriz()">✕</button>
      <div class="surpriz-icon">🏆</div>
      <h2 data-tr="el_surpriz_h">Hörmətli müəllim!</h2>
      <p class="surpriz-text"><span data-tr="el_surpriz_text_pre">Bizim qrupa</span> <span class="bal" data-tr="el_surpriz_bal">10 bal</span> <span data-tr="el_surpriz_text_suf">verirsiniz</span></p>
      <p class="surpriz-sub" data-tr="el_surpriz_sub">Çox sağ olun! 🎉</p>
    </div>
  </div>

  <!-- footer -->
  <footer class="footer">
    <div class="footer-inner">
      <div class="footer-brand">
        <p class="footer-logo"><svg viewBox="0 0 24 24" fill="none" stroke="cornflowerblue" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" width="20" height="20" style="vertical-align: middle; margin-right: 6px;"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>Kibertəhlükəsizlik Kafedrası</p>
        <p data-tr="footer_slogan">Rəqəmsal dünyada təhlükəsizlik – gələcəyin əsası</p>
      </div>
      <div class="footer-links">
        <h4 data-tr="footer_kecidler">Keçidlər</h4>
        <a href="../Haqqimizda_Mehrac/index.html" data-tr="nav_haqqimizda">Haqqımızda</a>
        <a href="../Fenler_Yusif/index.html" data-tr="nav_fenler">Fənlər</a>
        <a href="../Meqaleler_Senan_Mehrac/index.html" data-tr="nav_meqaleler">Məqalələr</a>
      </div>
      <div class="footer-contact">
        <h4 data-tr="footer_elaqe_bash">Əlaqə</h4>
        <p>Email: info@cybersec.edu.az</p>
        <p>Tel: +994 12 123 45 67</p>
        <p>Ünvan: Bakı, Azərbaycan</p>
      </div>
    </div>
    <div class="footer-bottom">
      <p data-tr="footer_copyright">© 2026 Kibertəhlükəsizlik Kafedrası. Bütün hüquqlar qorunur.</p>
    </div>
  </footer>
</body>
</html>
