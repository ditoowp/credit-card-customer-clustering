# **Credit Card Customer** : Clustering/Segmentation

By [Dito Wicaksana P.](https://github.com/ditoowp) | Data Resource: Google BigQuery

<center><img src="https://s28126.pcdn.co/blogs/ask-experian/wp-content/uploads/4-Types-of-Cards-Everyone-Should-Have-in-Their-Wallet-1400x933-1-900x600.jpg.optimal.jpg"/></center>

---

## Introduction 

Dalam industri jasa keuangan yang kompetitif, memahami perilaku dan preferensi *customer* sangat penting untuk mengembangkan strategi pemasaran yang efektif, meningkatkan kepuasan *customer*, dan memperbaiki kinerja bisnis secara keseluruhan. Salah satu teknik yang ampuh untuk mencapai pemahaman ini adalah melalui segmentasi *customer*, yang melibatkan pembagian basis *customer* menjadi kelompok-kelompok yang berbeda dengan karakteristik dan perilaku serupa. Proyek ini berfokus pada segmentasi *customer* kartu kredit menggunakan teknik *unsupervised learning*, khususnya *clustering*.

--- 

## Objective
Objektif utama dari proyek segmentasi *customer* kartu kredit ini adalah untuk membagi *customer* kartu kredit menjadi beberapa segmen yang berbeda berdasarkan pola transaksi dan karakteristik mereka. Tujuan ini dipecah menjadi beberapa sub-objektif sebagai berikut:

1. **Mengidentifikasi segmen *customer* yang berbeda:**
    - Menggunakan teknik clustering untuk menemukan kelompok-kelompok *customer* yang memiliki perilaku dan karakteristik serupa.
    - Mengidentifikasi atribut-atribut utama yang membedakan satu segmen dari segmen lainnya.
2. **Memahami pola pengeluaran dan perilaku *customer*:**
    - Menganalisis pola transaksi dan kebiasaan pengeluaran setiap segmen untuk memahami perilaku belanja mereka.
    - Menggunakan wawasan ini untuk mengidentifikasi segmen *customer* dengan nilai tinggi dan segment yang mungkin berisiko tinggi.
3. **Meningkatkan strategi pemasaran dan penjualan:**
    - Mengembangkan strategi pemasaran yang lebih terarah dan efektif berdasarkan karakteristik dan kebutuhan spesifik dari setiap segmen.
    - Meningkatkan retensi *customer* dengan menawarkan promosi dan layanan yang sesuai dengan preferensi setiap segmen.
4. **Meningkatkan pengembangan produk dan layanan:**
    - Mengidentifikasi kebutuhan spesifik dari setiap segmen untuk mengembangkan produk dan layanan yang lebih sesuai.
    - Menciptakan produk dan layanan baru yang dapat menarik segmen *customer* yang berbeda dan meningkatkan kepuasan *customer* secara keseluruhan.
5. **Optimasi *risk management*:**
    - Mengidentifikasi segmen *customer* yang berisiko tinggi untuk mengimplementasikan strategi manajemen risiko yang lebih efektif.
    - Mengurangi potensi kerugian dengan mengawasi dan mengelola *customer* yang termasuk dalam segmen berisiko tinggi.

Dengan mencapai objektif-objektif ini, proyek ini diharapkan dapat memberikan wawasan yang mendalam dan actionable insights yang dapat membantu lembaga keuangan dalam pengambilan keputusan yang lebih baik dan perencanaan strategis yang lebih efektif.

---

## Conclusion

* **EDA Before Clustering**

Berdasarkan EDA, pengguna kartu kredit lebih banyak yang memiliki *balance* yang sedikit namun mereka sering melakukan *update* terhadap jumlah *balance* yang mereka miliki. Pengguna kartu kredit lebih cenderung melakukan *purchases* dengan harga yang *moderate*. Selain itu, mereka jarang menggunakan *cash advance*, kalaupun ada yang menggunakan *cash advance* itu hanya dengan jumlah yang relatif kecil. Ini mungkin dikarenakan terdapat *limit* pada penggunaan *cash advance*.

* **Business Implication For Each Cluster**
    - **Cluster 0,**
        Memfokuskan pada penawaran produk bernilai tinggi yang disesuaikan, melakukan promosi *cash advance* yang ditargetkan, serta layanan konsultasi keuangan pribadi, sambil memantau *credit risk*.
    - **Cluster 1,**
        Mengembangkan program *daily rewards*, mempromosikan *rewards* transaksi rutin, dan mempertimbangkan opsi pembiayaan dengan bunga yang rendah, dengan fokus pada retensi dan peningkatan.
    - **Cluster 2,**
        Menawarkan atau menyediakan produk premium, penawaran khusus untuk pengeluaran yang tergolong *luxury*, layanan *cash advance* yang lebih baik, dan program loyalitas dinamis, sambil memantau pola pengeluaran dengan cermat.

* **Model Analysis**

`K-Means` digunakan disini dikarenakan dataset semua merupakan numerikal. Untuk *cluster* yang dipilih sendiri itu adalah 3 *cluster*. Jumlah ini diambil berdasarkan evaluasi dari **Silhoutte Score**.
