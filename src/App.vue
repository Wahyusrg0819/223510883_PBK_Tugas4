<script setup>
import { ref } from 'vue';
import ArticleCardList from './components/ArticleCardList.vue';
import ArticleCard from './components/ArticleCard.vue';
import ArticleModal from './components/ArticleModal.vue';
import FooterArticle from './components/FooterArticle.vue';


const articles = ref([
  {
    id: 1,
    title: 'Studi Baru Mengungkap Kehidupan Rahasia Kucing: Mengapa Mereka Pilih Menjaga Jarak dengan Manusia?',
    image: 'https://cdn.pixabay.com/photo/2024/02/28/07/42/european-shorthair-8601492_1280.jpg',
    summary: 'Penelitian terbaru dari Universitas Catlandia menunjukkan bahwa kucing cenderung menjaga jarak dengan manusia ketika merasa tidak nyaman. Temuan ini mengubah pandangan tentang hubungan kucing-manusia dan menyoroti kompleksitas perilaku hewan peliharaan.',
    content: `
    Dalam sebuah penelitian revolusioner yang dilakukan oleh para ilmuwan di Universitas Catlandia, sebuah temuan mengejutkan telah mengungkapkan pola perilaku yang menarik dari kucing domestik. Penelitian ini, yang berlangsung selama lima tahun, bertujuan untuk memahami dinamika interaksi antara kucing dan manusia. 
    Hasil studi tersebut menunjukkan bahwa kucing memiliki preferensi yang kuat untuk menjaga jarak dengan manusia dalam beberapa situasi tertentu. Para peneliti menyimpulkan bahwa hal ini tidak semata-mata karena sikap kucing yang cenderung independen, tetapi ada faktor-faktor lain yang memengaruhi perilaku mereka. 
    Salah satu penemuan menarik adalah bahwa kucing cenderung menjaga jarak ketika mereka merasa terganggu atau tidak nyaman dengan keberadaan manusia di sekitar mereka. 
    Hal ini menunjukkan bahwa kucing memiliki tingkat sensitivitas yang lebih tinggi daripada yang sebelumnya diyakini oleh banyak orang. Dr. Whiskers, salah seorang peneliti utama dalam studi ini, menjelaskan bahwa "Kucing tidak selalu menunjukkan perasaan mereka secara terbuka seperti anjing. Mereka memiliki cara tersendiri untuk mengungkapkan ketidaknyamanan atau stres, dan menjaga jarak dengan manusia adalah salah satu mekanisme pertahanan yang mereka gunakan." 
    Penemuan ini mengubah pandangan kita tentang hubungan antara kucing dan manusia, serta memberikan pemahaman yang lebih dalam tentang kompleksitas perilaku hewan peliharaan.
     Meskipun masih banyak yang harus dipelajari, penelitian ini menjadi langkah awal yang penting untuk menjembatani kesenjangan antara manusia dan kucing dalam pemahaman saling memahami satu sama lain.
    `
  },
  {
    id: 2,
    title: 'Mengungkap Misteri Seni Bonsai: Lebih dari Sekedar Tanaman Miniatur',
    image: 'https://upload.wikimedia.org/wikipedia/commons/thumb/b/b1/Bonsai_IMG_6412.jpg/360px-Bonsai_IMG_6412.jpg',
    summary: `
    Seni bonsai telah menarik minat banyak orang selama berabad-abad dengan keindahan dan kesederhanaannya yang memikat. Namun, di balik kecantikan yang terlihat, terdapat filosofi dan teknik yang kompleks yang melibatkan pemangkasan akar dan cabang serta perawatan yang cermat. Bonsai bukan hanya tentang menciptakan pohon miniatur, tetapi juga tentang menciptakan representasi alam yang harmonis dalam pot kecil.
    `,
    content: `
    Seni bonsai telah menarik minat banyak orang selama berabad-abad dengan keindahan dan kesederhanaannya yang memikat. Namun, di balik kecantikan yang terlihat, terdapat filosofi dan teknik yang kompleks yang melibatkan pemangkasan akar dan cabang serta perawatan yang cermat. Bonsai bukan hanya tentang menciptakan pohon miniatur, tetapi juga tentang menciptakan representasi alam yang harmonis dalam pot kecil.
    Di Jepang, tempat asal bonsai, seni ini dianggap sebagai bentuk meditasi yang membantu menghubungkan manusia dengan alam. Proses pembentukan bonsai membutuhkan kesabaran dan ketelitian yang tinggi, mengajarkan kesadaran terhadap waktu dan alam semesta. Setiap gerakan pemangkasan atau perawatan memiliki makna mendalam, mencerminkan filosofi Shinto yang menghargai keseimbangan dan harmoni.
    Bonsai tidak hanya sekadar hobi, tetapi juga cara untuk menyatukan jiwa dengan alam melalui penciptaan keindahan yang abadi. Meskipun membutuhkan dedikasi dan keterampilan yang tinggi, hasil akhirnya adalah karya seni yang membawa kedamaian dan keindahan bagi para pengamatnya.
    `
  },
  {
    id: 3,
    title: 'Mitos dan Fakta tentang Diet Ketogenik: Apa yang Sebenarnya Perlu Anda Ketahui?',
    image: 'https://d1vbn70lmn1nqe.cloudfront.net/prod/wp-content/uploads/2023/05/04085347/Kategori-Diet-Keto.jpg.webp',
    summary: `
    Diet ketogenik telah menjadi perbincangan hangat dalam dunia kesehatan dan kebugaran, namun masih ada banyak kesalahpahaman seputar konsep ini. 
    Sementara beberapa klaim tentang manfaat kesehatan dan penurunan berat badan telah diperdebatkan, ada fakta ilmiah yang perlu dipahami sebelum memulai diet ini.
    `,
    content:`
    Diet ketogenik telah menjadi perbincangan hangat dalam dunia kesehatan dan kebugaran, namun masih ada banyak kesalahpahaman seputar konsep ini. Sementara beberapa klaim tentang manfaat kesehatan dan penurunan berat badan telah diperdebatkan, ada fakta ilmiah yang perlu dipahami sebelum memulai diet ini.
    Meskipun diketahui dapat membantu menurunkan berat badan dengan cepat, diet ketogenik juga dapat memengaruhi kesehatan jangka panjang seseorang, terutama pada aspek keseimbangan gizi dan fungsi ginjal. Oleh karena itu, penting untuk berkonsultasi dengan profesional medis sebelum memulai diet ini, terutama bagi individu dengan kondisi kesehatan yang sudah ada.
    Dengan memahami mitos dan fakta seputar diet ketogenik, individu dapat membuat keputusan yang lebih terinformasi tentang apakah ini adalah pilihan yang tepat untuk tujuan kesehatan dan kebugaran mereka.
    `
  },
  {
    id: 4,
    title: 'Mengungkap Rahasia Kecerdasan Buatan: Bagaimana Algoritma Belajar Mesin Mengubah Dunia?',
    image: 'https://mediaedukasi.id/wp-content/uploads/2023/11/artificial-intelligence-new-technology-science-futuristic-abstract-human-brain-ai-technology-cpu-central-processor-unit-chipset-big-data-machine-learning-cyber-mind-domination-generative-ai-scaled-1.jpg',
    summary: `
    Kecerdasan Buatan (AI) telah menjadi pusat perhatian dalam beberapa dekade terakhir dengan kemampuannya untuk memecahkan masalah kompleks dan melakukan tugas yang sebelumnya hanya dapat dilakukan oleh manusia. 
    Salah satu komponen kunci di balik keberhasilan AI adalah algoritma pembelajaran mesin, yang memungkinkan sistem untuk belajar dari data tanpa perlu pemrograman langsung.
    `,
    content: `
    Kecerdasan Buatan (AI) telah menjadi pusat perhatian dalam beberapa dekade terakhir dengan kemampuannya untuk memecahkan masalah kompleks dan melakukan tugas yang sebelumnya hanya dapat dilakukan oleh manusia. Salah satu komponen kunci di balik keberhasilan AI adalah algoritma pembelajaran mesin, yang memungkinkan sistem untuk belajar dari data tanpa perlu pemrograman langsung.
    Algoritma pembelajaran mesin dapat diklasifikasikan menjadi beberapa jenis, termasuk pembelajaran terawasi, tidak terawasi, dan penguatan, masing-masing dengan pendekatan yang unik dalam memproses informasi. Dengan adanya teknik-teknik ini, AI dapat mengenali pola, membuat prediksi, dan mengambil keputusan dengan tingkat akurasi yang semakin tinggi.
    Penerapan AI dengan algoritma pembelajaran mesin telah menyentuh hampir semua aspek kehidupan manusia, mulai dari pengenalan wajah di media sosial hingga pengoptimalan rantai pasokan di industri manufaktur. Dengan terus berkembangnya teknologi ini, ada potensi besar untuk menciptakan solusi inovatif yang dapat memecahkan masalah kompleks di masa depan.
    `
  },
  {
    id: 5,
    title: 'Eksplorasi Terakhir: Mengungkap Misteri Lautan Dalam',
    image: 'https://thumb.viva.co.id/media/frontend/thumbs3/2010/03/09/86317_lapisan_gas_mirip_sungai_di_dalam_laut__cenote_angelita__mexico_1265_711.jpg',
    summary: `
    Lautan Dalam masih menjadi salah satu wilayah paling misterius dan kurang dipahami di Bumi. 
    Penelitian terbaru mengungkapkan kehidupan yang luar biasa di kedalaman yang belum pernah dijangkau oleh mata manusia sebelumnya. 
    Dengan teknologi baru seperti kapal selam otonom dan kamera beresolusi tinggi, para ilmuwan dapat mempelajari ekosistem yang kaya dan unik di kedalaman laut yang gelap dan tekanan tinggi ini.
    `,
    content: `
    Lautan Dalam masih menjadi salah satu wilayah paling misterius dan kurang dipahami di Bumi. Penelitian terbaru mengungkapkan kehidupan yang luar biasa di kedalaman yang belum pernah dijangkau oleh mata manusia sebelumnya. Dengan teknologi baru seperti kapal selam otonom dan kamera beresolusi tinggi, para ilmuwan dapat mempelajari ekosistem yang kaya dan unik di kedalaman laut yang gelap dan tekanan tinggi ini.
    Penemuan baru-baru ini termasuk spesies baru, fitoplankton bioluminesen, dan formasi geologis yang spektakuler, yang semuanya memberikan wawasan baru tentang evolusi kehidupan dan geologi bumi. Namun, tantangan dalam menjelajahi Lautan Dalam termasuk tekanan yang sangat tinggi, suhu yang rendah, dan kurangnya cahaya matahari, yang semuanya mengharuskan para peneliti untuk mengandalkan teknologi canggih untuk mengeksplorasi dan memahami lingkungan ini.
    Eksplorasi Lautan Dalam bukan hanya tentang memahami kehidupan di kedalaman, tetapi juga tentang memahami bagaimana ekosistem ini berinteraksi dengan laut yang lebih dangkal dan lingkungan global secara keseluruhan. Dengan pemahaman yang lebih baik tentang Lautan Dalam, kita dapat mengembangkan strategi perlindungan yang lebih efektif untuk menjaga keberlanjutan dan keberagaman hayati di seluruh planet ini.
    `
  },
  {
    id: 6,
    title: 'Menjelajahi Potensi Energi Alternatif: Arus Laut sebagai Sumber Energi Masa Depan',
    image: 'https://sunenergy.id/cfind/source/thumb/images/blog/cover_w880_h478_content-mengapa-kita-memerlukan-energi-alternatif-simak-alasannya-di-sini.jpg',
    summary: `
    Dengan meningkatnya kesadaran akan pentingnya energi terbarukan, arus laut telah muncul sebagai salah satu sumber energi yang menjanjikan untuk masa depan. 
    Dibandingkan dengan sumber energi konvensional, arus laut menawarkan keunggulan karena dapat diandalkan, tidak memancarkan gas rumah kaca, dan tersedia secara konsisten di sebagian besar wilayah pesisir.
    `,
    content: `
    Dengan meningkatnya kesadaran akan pentingnya energi terbarukan, arus laut telah muncul sebagai salah satu sumber energi yang menjanjikan untuk masa depan. Dibandingkan dengan sumber energi konvensional, arus laut menawarkan keunggulan karena dapat diandalkan, tidak memancarkan gas rumah kaca, dan tersedia secara konsisten di sebagian besar wilayah pesisir.
    Teknologi pembangkit listrik tenaga arus laut (PLTAA) terus berkembang dengan cepat, dari turbin arus laut hingga perangkat pengumpul energi kinetik. Meskipun masih dalam tahap pengembangan, potensi energi yang dapat dihasilkan dari arus laut sangat besar dan dapat berkontribusi signifikan dalam memenuhi kebutuhan energi global.
    Namun, ada beberapa tantangan yang perlu diatasi, termasuk biaya tinggi, dampak lingkungan, dan keterbatasan teknologi saat ini. Dengan penelitian dan investasi yang lebih lanjut, arus laut memiliki potensi untuk menjadi salah satu sumber energi utama yang membantu mengurangi ketergantungan pada bahan bakar fosil dan mengurangi jejak karbon global.
    `
  },
  {
    id: 7,
    title: 'Perubahan Iklim di Kepulauan: Adaptasi dan Ketahanan Masyarakat Pesisir',
    image: 'https://awsimages.detik.net.id/community/media/visual/2023/06/22/1379073342.jpeg?w=1254',
    summary: `
    Kepulauan sering kali menjadi pusat perhatian dalam diskusi tentang perubahan iklim, karena mereka rentan terhadap ancaman seperti kenaikan permukaan laut, badai tropis, dan erosi pantai. 
    Masyarakat pesisir yang tinggal di pulau-pulau ini harus menghadapi tantangan besar dalam menyesuaikan diri dengan dampak perubahan iklim yang semakin nyata.
    `,
    content: `
    Kepulauan sering kali menjadi pusat perhatian dalam diskusi tentang perubahan iklim, karena mereka rentan terhadap ancaman seperti kenaikan permukaan laut, badai tropis, dan erosi pantai. Masyarakat pesisir yang tinggal di pulau-pulau ini harus menghadapi tantangan besar dalam menyesuaikan diri dengan dampak perubahan iklim yang semakin nyata.
    Adaptasi menjadi kunci untuk meningkatkan ketahanan masyarakat pesisir. Inisiatif seperti pengembangan infrastruktur tangguh, sistem peringatan dini, dan rencana evakuasi darurat menjadi penting untuk melindungi penduduk dan aset mereka dari ancaman cuaca ekstrem. Selain itu, pendekatan berbasis masyarakat yang melibatkan pengetahuan lokal dan partisipasi aktif dari komunitas dapat meningkatkan kemampuan mereka untuk menghadapi perubahan iklim.
    Namun, tantangan utama tetaplah kompleksitas perubahan iklim itu sendiri, yang sering kali tidak terduga dan sulit diprediksi. Oleh karena itu, kerja sama lintas sektoral dan internasional menjadi kunci dalam membangun ketahanan masyarakat pesisir di kepulauan. Dengan upaya bersama, masyarakat pesisir dapat membangun masa depan yang lebih berkelanjutan dan tangguh di tengah tantangan perubahan iklim yang terus meningkat.
    `
  },
  {
    id: 8,
    title: 'Judul Artikel Kedua',
    image: 'https://via.placeholder.com/150/56a8c2',
    summary: 'Ringkasan artikel kedua...',
    content: 'Konten lengkap artikel kedua...'
  },
  
]);


const showContactModal = ref(false);
const showArticleModal = ref(false);

const selectedMenu = ref('');
const selectedArticle = ref(null);


const openContactModal = () => {
  selectedMenu.value = 'contact';
  showContactModal.value = true;
};

const closeContactModal = () => {
  selectedMenu.value = '';
  showContactModal.value = false;
};

const openArticleModal = (article) => {
  selectedArticle.value = article;
  showArticleModal.value = true;
};

const closeArticleModal = () => {
  selectedArticle.value = null;
  showArticleModal.value = false;
};

import ContactModal from './components/contactModal.vue';
</script>

<template  >
  <header>
    <h1 class="h2">Article Card Wahyu</h1>
    <nav>
      <button to="/about">About</button>
      <button @click="openContactModal" :class="{'active': selectedMenu === 'contact'}">Contact</button>
    </nav>
  </header>

  <div>
    <ContactModal v-if="showContactModal && selectedMenu === 'contact'" @click="closeContactModal" />
      
  
  </div>

  <ul class="example-2">
    <li class="icon-content">
      <a href="https://www.instagram.com/wahyu_shiregaru/" aria-label="Instagram" data-social="instagram">
        <div class="filled"></div>
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-instagram" viewBox="0 0 16 16" xml:space="preserve">
          <path d="M8 0C5.829 0 5.556.01 4.703.048 3.85.088 3.269.222 2.76.42a3.9 3.9 0 0 0-1.417.923A3.9 3.9 0 0 0 .42 2.76C.222 3.268.087 3.85.048 4.7.01 5.555 0 5.827 0 8.001c0 2.172.01 2.444.048 3.297.04.852.174 1.433.372 1.942.205.526.478.972.923 1.417.444.445.89.719 1.416.923.51.198 1.09.333 1.942.372C5.555 15.99 5.827 16 8 16s2.444-.01 3.298-.048c.851-.04 1.434-.174 1.943-.372a3.9 3.9 0 0 0 1.416-.923c.445-.445.718-.891.923-1.417.197-.509.332-1.09.372-1.942C15.99 10.445 16 10.173 16 8s-.01-2.445-.048-3.299c-.04-.851-.175-1.433-.372-1.941a3.9 3.9 0 0 0-.923-1.417A3.9 3.9 0 0 0 13.24.42c-.51-.198-1.092-.333-1.943-.372C10.443.01 10.172 0 7.998 0zm-.717 1.442h.718c2.136 0 2.389.007 3.232.046.78.035 1.204.166 1.486.275.373.145.64.319.92.599s.453.546.598.92c.11.281.24.705.275 1.485.039.843.047 1.096.047 3.231s-.008 2.389-.047 3.232c-.035.78-.166 1.203-.275 1.485a2.5 2.5 0 0 1-.599.919c-.28.28-.546.453-.92.598-.28.11-.704.24-1.485.276-.843.038-1.096.047-3.232.047s-2.39-.009-3.233-.047c-.78-.036-1.203-.166-1.485-.276a2.5 2.5 0 0 1-.92-.598 2.5 2.5 0 0 1-.6-.92c-.109-.281-.24-.705-.275-1.485-.038-.843-.046-1.096-.046-3.233s.008-2.388.046-3.231c.036-.78.166-1.204.276-1.486.145-.373.319-.64.599-.92s.546-.453.92-.598c.282-.11.705-.24 1.485-.276.738-.034 1.024-.044 2.515-.045zm4.988 1.328a.96.96 0 1 0 0 1.92.96.96 0 0 0 0-1.92m-4.27 1.122a4.109 4.109 0 1 0 0 8.217 4.109 4.109 0 0 0 0-8.217m0 1.441a2.667 2.667 0 1 1 0 5.334 2.667 2.667 0 0 1 0-5.334" fill="currentColor"></path>
        </svg>
      </a>
      <div class="tooltip">Instagram</div>
    </li>
  </ul>

  <div id="app">
    <ArticleCardList>
      
      <ArticleCard
        v-for="article in articles"
        :key="article.id"
        :article="article"
        @click="openArticleModal(article)"
      />
    </ArticleCardList>

    <ArticleModal
      :article="selectedArticle"
      :showModal="showArticleModal"
      @close="closeArticleModal"
    />
  </div>
     
  <FooterArticle>
    <template v-slot:footer>
    <p>&copy; Wahyu Siregar 2024</p>
    </template>
  </FooterArticle>
  
    
    
</template>


<style scoped>

nav {
  display: flex;
  justify-content:space-around;
  align-items: left ;
  margin: 1px;
}

button {
  padding: 1.3em 3em;
  font-size: 12px;
  text-transform: uppercase;
  letter-spacing: 2.5px;
  font-weight: 500;
  color: #000;
  background-color: #fff;
  border: none;
  border-radius: 45px;
  box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease 0s;
  cursor: pointer;
  outline: none;
  margin-top: 3%;
  margin-bottom: 3%;
}

button:hover {
  background-color: #23c483;
  box-shadow: 0px 15px 20px rgba(46, 229, 157, 0.4);
  color: #fff;
  transform: translateY(-7px);
}

button:active {
  transform: translateY(-1px);
}

footer {
  position:relative;
  width: 100%;
  height: 100%;
  background-color: black;
  color: white;
  text-align: center;
  padding: 10px;
}

header {
  text-align: center;
  padding:10px;
  margin-left:0px;
  border-bottom-left-radius: 10px;
  border-bottom-right-radius: 10px;
  
  width: 100%;
  height: 100%;
  --s: 200px; 
  --c1: #1d1d1d;
  --c2: #4e4f51;
  --c3: #3c3c3c;

  background: repeating-conic-gradient(
        from 30deg,
        #0000 0 120deg,
        var(--c3) 0 180deg
      )
      calc(0.5 * var(--s)) calc(0.5 * var(--s) * 0.577),
    repeating-conic-gradient(
      from 30deg,
      var(--c1) 0 60deg,
      var(--c2) 0 120deg,
      var(--c3) 0 180deg
    );
  background-size: var(--s) calc(var(--s) * 0.577);
}

.h2 {
  color:white;
  margin-bottom: 0px;
  text-shadow: #171d25;
  
   
}


.logo { 
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}

ul {
  list-style: none;
  
}

.example-2 {
  display: flex;
  justify-content: inherit;
  align-items: center;
}
.example-2 .icon-content {
  margin: 0 10px;
  position: relative;
}
.example-2 .icon-content .tooltip {
  position: absolute;
  top: -30px;
  left: 50%;
  transform: translateX(-50%);
  color: #fff;
  padding: 6px 10px;
  border-radius: 5px;
  opacity: 0;
  visibility: hidden;
  font-size: 14px;
  transition: all 0.3s ease;
}
.example-2 .icon-content:hover .tooltip {
  opacity: 1;
  visibility: visible;
  top: -50px;
}
.example-2 .icon-content a {
  position: relative;
  overflow: hidden;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  color: #4d4d4d;
  background-color: #fff;
  transition: all 0.3s ease-in-out;
}
.example-2 .icon-content a:hover {
  box-shadow: 3px 2px 45px 0px rgb(0 0 0 / 12%);
}
.example-2 .icon-content a svg {
  position: relative;
  z-index: 1;
  width: 30px;
  height: 30px;
}
.example-2 .icon-content a:hover {
  color: white;
}
.example-2 .icon-content a .filled {
  position: absolute;
  top: auto;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 0;
  background-color: #000;
  transition: all 0.3s ease-in-out;
}
.example-2 .icon-content a:hover .filled {
  height: 100%;
}

.example-2 .icon-content a[data-social="discord"] .filled,
.example-2 .icon-content a[data-social="discord"] ~ .tooltip {
  background-color: #7289da;
}

.example-2 .icon-content a[data-social="steam"] .filled,
.example-2 .icon-content a[data-social="steam"] ~ .tooltip {
  background-color: #171d25;
}
.example-2 .icon-content a[data-social="instagram"] .filled,
.example-2 .icon-content a[data-social="instagram"] ~ .tooltip {
  background: linear-gradient(
    45deg,
    #405de6,
    #5b51db,
    #b33ab4,
    #c135b4,
    #e1306c,
    #fd1f1f
  );
}
.example-2 .icon-content a[data-social="youtube"] .filled,
.example-2 .icon-content a[data-social="youtube"] ~ .tooltip {
  background-color: #ff0000;
}

</style>
