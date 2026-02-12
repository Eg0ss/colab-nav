<template>
  <div class="about-container">
    <div class="about-hero">
      <h1>On ne gère pas des dossiers, <br><span>mais des humains.</span></h1>
    </div>

    <div class="content-layout">
      <div class="timeline">
        <div class="checkpoint">
          <div class="dot"></div>
          <div class="text">
            <h4>2024</h4>
            <p>Naissance de l'idée : simplifier le chaos administratif.</p>
          </div>
        </div>
        <div class="checkpoint">
          <div class="dot active"></div>
          <div class="text">
            <h4>Aujourd'hui</h4>
            <p>Une plateforme robuste utilisée par des centaines de RH.</p>
          </div>
        </div>
      </div>

      <div class="pillars">
        <div class="pillar-card">
          <span class="number">01</span>
          <h3>Simplicité</h3>
          <p>Pas de manuel d'utilisation, tout est intuitif.</p>
        </div>
        <div class="pillar-card">
          <span class="number">02</span>
          <h3>Vitesse</h3>
          <p>Une interface qui répond au doigt et à l'œil.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.about-container {
  max-width: 1100px;
  margin: 0 auto;
  padding: 60px 20px;
  font-family: 'Inter', sans-serif;
}

.about-hero h1 {
  font-size: 3.5rem;
  font-weight: 800;
  color: #0f172a;
  line-height: 1.1;
  margin-bottom: 80px;
}

.about-hero h1 span {
  color: #0ea5e9;
}

.content-layout {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 100px;
}

.timeline {
  border-left: 2px solid #e2e8f0;
  padding-left: 30px;
  position: relative;
}

.checkpoint {
  position: relative;
  margin-bottom: 50px;
}

.dot {
  position: absolute;
  left: -41px;
  top: 5px;
  width: 20px;
  height: 20px;
  background: white;
  border: 4px solid #e2e8f0;
  border-radius: 50%;
}

.dot.active {
  border-color: #0ea5e9;
  box-shadow: 0 0 15px rgba(14, 165, 233, 0.4);
}

.checkpoint h4 {
  margin: 0;
  color: #0ea5e9;
  font-size: 1.2rem;
}

.checkpoint p {
  color: #64748b;
  margin-top: 5px;
}

.pillars {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.pillar-card {
  background: #ffffff;
  padding: 30px;
  border-radius: 16px;
  border: 1px solid #f1f5f9;
  position: relative;
  transition: all 0.3s ease;
}

.pillar-card:hover {
  transform: translateX(10px);
  border-color: #bae6fd;
}

.number {
  position: absolute;
  top: 20px;
  right: 20px;
  font-size: 2rem;
  font-weight: 900;
  color: #f1f5f9;
}

.pillar-card h3 {
  margin: 0 0 10px 0;
  color: #0c4a6e;
}

.pillar-card p {
  margin: 0;
  color: #64748b;
  font-size: 0.95rem;
}

@media (max-width: 768px) {
  .content-layout { grid-template-columns: 1fr; gap: 50px; }
  .about-hero h1 { font-size: 2.2rem; }
}
</style>