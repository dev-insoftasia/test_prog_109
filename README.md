<h1 id="aplikasi-multi-tenant-e-commerce-kecil-dengan-isolasi-data-dan-ssr-incremental">Aplikasi Multi-tenant E-Commerce kecil dengan Isolasi Data dan SSR Incremental</h1>
<p>Deskripsi:</p>
<ul>
<li>Bangun prototype toko online multi-tenant (brand A dan brand B) yang memakai Next.js App Router. Tiap tenant punya katalog, tema sederhana, dan halaman checkout mock.</li>
</ul>
<p>Syarat Minimal:</p>
<ul>
<li>SSR untuk halaman katalog dengan incremental rendering untuk tiap-tenant (caching per tenant).</li>
<li>Isolasi data tenant: tidak boleh ada kemungkinan satu tenant membaca data tenant lain pada runtime.</li>
<li>Checkout fake: API route membuat &ldquo;order&rdquo; ke mock persisted store; simulasikan race condition ketika 2 request memesan stok terakhir.</li>
</ul>
<p>Teknis:</p>
<ul>
<li>Jelaskan arsitektur isolasi data dan bagaimana Anda mencegah cross-tenant leakage.</li>
<li>Tunjukkan mekanisme cache per-tenant dan skenario invalidasi.</li>
<li>Tangani race condition dengan strategi yang bisa diuji secara manual.</li>
<li>Sertakan diagram arsitektur singkat dan trade-offs keputusan Anda.</li>
</ul>
<p>Deliverable:</p>
<ul>
<li>Repo dengan README, script run, tenant demo (dua tenant), langkah reproduksi race condition, dan file arsitektur.</li>
<li>Invite github @dev-insoftasia ke repo tersebut.</li>
</ul>
