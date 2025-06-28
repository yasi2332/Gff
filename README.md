from docx import Document

# ایجاد مجدد فایل Word با لوگو Coldwell Banker برای لیست سوالات جلسه Hyatt پس از ریست شدن محیط

doc = Document()
doc.add_heading('Hyatt + 30 Rezidans Satın Alma Görüşme Soruları', level=1)

questions = [
    "1. Bu 30 rezidans ünitesinin her birinin tapusu ayrı mı?",
    "2. Tapu kayıtları üzerinde ipotek, haciz veya satış kısıtlaması var mı?",
    "3. Tapular tek tek benim adıma mı devredilecek yoksa bir şirket yapısı üzerinden mi aktarılacak?",
    "4. Rezidans tapularında kat irtifakı mı var yoksa kat mülkiyeti mi?",
    "5. Bu 180 milyon € fiyatlandırma, SPK değerleme raporuna göre mi belirlendi?",
    "6. SPK raporunda otel ve rezidanslar ayrı mı yoksa tek proje olarak mı değerlendirilmiş?",
    "7. Rezidansların ortalama metrekare fiyatı nedir ve toplam metrekare dağılımı nasıl?",
    "8. Bu fiyat neden proje piyasa ortalamasından daha düşük belirlenmiş? (gerekçesi)",
    "9. Daha önce bu rezidanslardan satılmış olan veya satışa çıkmış ünite var mı?",
    "10. Eğer var ise, kaç ünite satıldı ve şu anki sahipleri kimler?",
    "11. Rezidanslar Hyatt markası altında mı yönetiliyor yoksa bağımsız kullanım mı söz konusu?",
    "12. Mevcut franchise / management anlaşması rezidansları da kapsıyor mu yoksa sadece otel operasyonunu mu?",
    "13. Satın alma sonrası Hyatt yönetimi ile yeni bir sözleşme imzalamam gerekiyor mu?",
    "14. Satın alma sırasında KDV oranı nedir ve tapu harçları nasıl hesaplanıyor?",
    "15. Ödeme planında kapora ne kadar, escrow hesabı kullanılacak mı?",
    "16. Tapu devir işlemi sırasında tüm ödemeler nasıl yapılandırılacak?",
    "17. Otelin son 3 yıllık ADR, occupancy ve net kar verileri nedir?",
    "18. Rezidanslardan kira veya yönetim geliri elde ediliyor mu yoksa boş mu duruyorlar?",
    "19. Hyatt markası altında rezidans kiralamak için aylık yönetim ücreti veya marka bedeli nedir?"
]

for q in questions:
    doc.add_paragraph(q)

doc.add_paragraph("\nSaygılarımla,\nAshkan Kohanpoolaad\nBroker Associate\nColdwell Banker\n📞 +1 818-445-6211\n✉️ salongmustachen@hotmail.com\n🌐 www.coldwellbanker.com")

output_path = "/mnt/data/Hyatt_Rezidans_Satin_Alma_Sorular.docx"
doc.save(output_path)

output_path
