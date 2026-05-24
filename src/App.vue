<script setup>
</script>

<template>
  <div class="app-shell">
    <section class="hero">
      <div class="hero-copy">
        <p class="eyebrow">Aplikasi Bahan Ajar UT</p>
        <h1>Kelola stok secara cepat dan pantau delivery order dengan mudah</h1>
        <p>
          Mulai dari manajemen stok bahan ajar sampai tracking DO, semua tersedia dalam satu tampilan.
          Pilih tombol berikut untuk melanjutkan.
        </p>
      </div>

      <div class="hero-actions">
        <a class="action-card primary" href="/stok.html">
          <span>Stok Bahan Ajar</span>
          <p>Masuk ke dashboard stok dan update data bahan ajar.</p>
        </a>

        <a class="action-card secondary" href="/tracking.html">
          <span>Tracking DO</span>
          <p>Lacak status pengiriman DO mahasiswa secara real time.</p>
        </a>
      </div>
    </section>
  </div>
</template>

<style scoped>
.app-shell {
  min-height: calc(100vh - 4rem);
  display: grid;
  place-items: center;
  padding: 2rem;
  background: linear-gradient(180deg, #f7fcfb 0%, #e8f5f0 100%);
}

.hero {
  width: min(100%, 980px);
  display: grid;
  gap: 2rem;
  padding: 2.5rem;
  border-radius: 28px;
  background: #ffffff;
  box-shadow: 0 28px 80px rgba(15, 23, 42, 0.08);
}

.hero-copy {
  max-width: 640px;
}

.eyebrow {
  margin: 0 0 1rem;
  color: #2d7a5a;
  font-size: 0.95rem;
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

.hero h1 {
  margin: 0;
  font-size: clamp(2rem, 2.5vw, 3.4rem);
  line-height: 1.05;
  color: #0f3f2b;
}

.hero p {
  margin: 1.2rem 0 0;
  font-size: 1rem;
  max-width: 680px;
  line-height: 1.85;
  color: #334a48;
}

.hero-actions {
  display: grid;
  gap: 1rem;
}

.action-card {
  display: block;
  padding: 1.6rem 1.8rem;
  border-radius: 22px;
  text-decoration: none;
  transition: transform 0.24s ease, box-shadow 0.24s ease, background 0.24s ease;
  box-shadow: 0 18px 45px rgba(15, 23, 42, 0.08);
}

.action-card span {
  display: block;
  font-size: 1.25rem;
  font-weight: 700;
  margin-bottom: 0.6rem;
}

.action-card p {
  margin: 0;
  color: #4c5753;
  line-height: 1.7;
}

.action-card:hover {
  transform: translateY(-4px);
}

.primary {
  background: linear-gradient(135deg, #1c7b5c 0%, #41b78a 100%);
  color: white;
}

.secondary {
  background: linear-gradient(135deg, #285d8f 0%, #57a0df 100%);
  color: white;
}

@media (min-width: 720px) {
  .hero-actions {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }
}
</style>
