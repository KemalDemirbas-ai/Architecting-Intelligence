# 💳 Project #03: Credit Risk Assessment Engine
## 📊 Kategori: 1-Tabular-Models (Endüstriyel Sınıflandırma Serisi)

**Durum:** Tamamlandı ✅ | **Performans:** 0.8120 Global Accuracy 🚀

### 🎯 Endüstriyel Hedef
**Credit Risk Assessment Engine**, bir bankanın kredi kartı temerrüt (ödeme yapamama) riskini minimize etmek için tasarlanmış otonom bir risk puanlama sistemidir. Bu proje, "Sınıf Dengesizliği" (Class Imbalance) yönetimi, finansal veri temizliği ve bankacılık standartlarında **Recall** odaklı modelleme üzerine bir "Masterclass" çalışmasıdır.

---

### 🧠 10 Adımlık Mühendislik Hattı (Pipeline)
Bu proje, **Architecting-Intelligence** çekirdek felsefesine sadık kalarak 10 adımda inşa edilmiştir:

1.  **Hedef Tanımı:** Bankanın donuk alacaklarını (NPL) azaltmak için gelecek ayki ödeme riskini tahmin etmek.
2.  **Veri Girişi & EDA:** UCI Credit Card veri seti analiz edildi; 6 aylık ödeme geçmişindeki kritik sinyaller belirlendi.
3.  **Özellik Seçimi:** Modelin ezberlemesini önlemek için `ID` sütunu kaldırıldı ve hedef değişken izole edildi.
4.  **Kategorik Dönüşüm:** Eğitim ve medeni durum gibi kategorilerdeki gürültüler temizlendi ve stratejik olarak eşlendi.
5.  **Veri Manipülasyonu:** Boş değer analizi yapıldı ve medyan tamamlama stratejileriyle veri bütünlüğü sağlandı.
6.  **Gelişmiş Özellik Mühendisliği:** Müşterinin finansal stres seviyesini ölçen **'PAY_RATIO_1'** (Ödeme/Borç Oranı) metriği üretildi.
7.  **Ölçeklendirme (Scaling):** Kredi limiti gibi büyük rakamlar ile kategorik kodları uyumlu hale getirmek için **StandardScaler** uygulandı.
8.  **Stratified Splitting:** Verideki %22'lik risk oranını korumak için katmanlı bölme (80/20) uygulandı.
9.  **Model Eğitimi:** Karmaşık risk kararlarını simüle etmek için **Random Forest Classifier** ($n\_estimators=100$) eğitildi.
10. **Değerlendirme:** **%81.2 Accuracy** değerine ulaşıldı; düşük riskli müşterilerde %84 hassasiyet (Precision) sağlandı.

---

### 🚀 Canlı Endüstriyel Dağıtım
Risk motoru, gerçek zamanlı bir ekspertiz paneli ve "Cyber-Neon" arayüzü ile Hugging Face Spaces üzerinde yayındadır.

👉 **[Launch Live Credit Risk Engine](https://huggingface.co/spaces/Ironside35/Credit-Risk-Assessment-Engine)** 💳

---

### ⚙️ Teknoloji Yığını
- **Motor:** Python | Scikit-Learn | Random Forest
- **Veri İşleme:** Pandas | NumPy
- **Görselleştirme:** Seaborn | Matplotlib
- **Dağıtım:** Streamlit | Hugging Face Spaces

---

**Mimar:** Kemal Demirbaş  
