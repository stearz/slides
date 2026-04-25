---
theme: default
colorSchema: light
layout: cover
transition: fade-out
mdc: true
title: Lasttests für Kubernetes-Workloads
info: |
  Nachbau der IT-Tage 2025 Präsentation in Slidev.
class: text-left
fonts:
  sans: 'Arial'
---

<style>
:root {
  --brand: #0b4ea2;
  --brand-dark: #123d7a;
  --muted: #5f6b7a;
}
.slidev-layout {
  background: white;
  color: #111827;
}
h1, h2, h3 {
  color: var(--brand-dark);
}
.page-no {
  position: absolute;
  right: 18px;
  bottom: 10px;
  font-size: 12px;
  color: #6b7280;
}
.title-slide {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  min-height: 100%;
  padding-bottom: 2rem;
}
.title-slide .tag {
  position: absolute;
  right: 2rem;
  top: 1.5rem;
  font-size: 1.25rem;
  color: white;
  background: #0b0b0b;
  padding: 0.35rem 0.75rem;
}
.section-title {
  font-size: 2rem;
  font-weight: 700;
  color: var(--brand-dark);
  margin-bottom: 1.5rem;
}
.bullets {
  font-size: 1.15rem;
  line-height: 1.55;
}
.bullets li {
  margin: 0.45rem 0;
}
.note {
  color: var(--muted);
  font-size: 0.95rem;
}
.two-col {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2rem;
  align-items: start;
}
.image-frame {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
}
.image-frame img {
  max-width: 100%;
  max-height: 100%;
  object-fit: contain;
}
</style>

<div class="title-slide">
  <div class="tag">#ittage</div>
  <div class="text-5xl font-bold" style="color:#123d7a">Lasttests für Kubernetes-Workloads</div>
  <div class="text-3xl mt-4" style="color:#123d7a">Stephan Schwarz</div>
  <div class="page-no">1</div>
</div>

---
layout: default
---

<div class="section-title">about me</div>

<div class="two-col">
  <div>
    <ul class="bullets">
      <li>44 Jahre alt</li>
      <li>Verheiratet, zwei Kinder</li>
      <li>Rollen in der Vergangenheit:
        <ul>
          <li>Network Administrator</li>
          <li>Systems Engineer</li>
          <li>Cloud Engineer</li>
          <li>Infrastructure Developer</li>
          <li>Platform Engineer</li>
        </ul>
      </li>
      <li>seit 2017: Kubernetes</li>
      <li>seit 2021: Consultant</li>
    </ul>
  </div>
  <div class="text-lg leading-8 pt-40">
    <div>Stephan Schwarz</div>
    <div>Senior DevOps Engineer / Consultant</div>
    <div>iits-consulting GmbH</div>
  </div>
</div>
<div class="page-no">2</div>

---

<div class="section-title">what about you?</div>
<div class="page-no">3</div>

---

<div class="section-title">Wie das Thema zu mir kam</div>
<div class="page-no">4</div>

---

<div class="section-title">Was ist Performance?</div>

<div class="text-2xl mb-8"><strong>Performant</strong> = <strong>Erwartungen</strong> werden <strong>erfüllt</strong> an:</div>
<ul class="bullets text-xl">
  <li>Durchsatz</li>
  <li>Latenz</li>
  <li>Skalierbarkeit</li>
  <li>Ressourcenverbrauch</li>
</ul>
<div class="page-no">5</div>

---

<div class="section-title">Warum Lasttests?</div>
<ul class="bullets text-xl">
  <li>Aufdecken von <strong>Bottlenecks</strong></li>
  <li><strong>Stabiler Betrieb</strong></li>
  <li>Testen der <strong>Skalierbarkeit</strong></li>
  <li>Sicherstellung von <strong>SLAs</strong></li>
  <li>Ermittlung der benötigten <strong>Ressourcen</strong></li>
  <li>Optimierung von <strong>Kosten</strong></li>
</ul>
<div class="page-no">6</div>

---

<div class="section-title">Arten von Lasttests</div>
<div class="image-frame">
  <img src="/assets/rendered/page-07.png" alt="Arten von Lasttests" />
</div>
<div class="page-no">7</div>

---

<div class="section-title">Smoke Test</div>
<div class="image-frame">
  <img src="/assets/rendered/page-08.png" alt="Smoke Test" />
</div>
<div class="page-no">8</div>

---

<div class="section-title">Average Load Test</div>
<div class="image-frame">
  <img src="/assets/rendered/page-09.png" alt="Average Load Test" />
</div>
<div class="page-no">9</div>

---

<div class="section-title">Spike Test</div>
<div class="image-frame">
  <img src="/assets/rendered/page-10.png" alt="Spike Test" />
</div>
<div class="page-no">10</div>

---

<div class="section-title">Stress Test</div>
<div class="image-frame">
  <img src="/assets/rendered/page-11.png" alt="Stress Test" />
</div>
<div class="page-no">11</div>

---

<div class="section-title">Soak Test</div>
<div class="image-frame">
  <img src="/assets/rendered/page-12.png" alt="Soak Test" />
</div>
<div class="page-no">12</div>

---

<div class="section-title">Break Point Test</div>
<div class="image-frame">
  <img src="/assets/rendered/page-13.png" alt="Break Point Test" />
</div>
<div class="page-no">13</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-14.png" alt="Load Generatoren" />
</div>
<div class="page-no">14</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-15.png" alt="Load Generatoren markiert" />
</div>
<div class="page-no">15</div>

---

<div class="section-title">Was wird getestet?</div>
<div class="text-2xl mb-6">End-to-end</div>
<ul class="bullets text-xl">
  <li>Realitätsnah</li>
  <li>Kundenperspektive</li>
  <li>Testet komplette Infrastruktur</li>
  <li>Abhängige Services werden mitgetestet</li>
</ul>
<div class="page-no">16</div>

---

<div class="section-title">Was wird getestet?</div>
<div class="text-2xl mb-6">Labor Test</div>
<ul class="bullets text-xl">
  <li>z.B. <strong>Single Pod</strong> Perspektive</li>
  <li>Ermittlung der <strong>Resource Usage</strong></li>
  <li>Experimentieren mit Werten für <strong>requests</strong> und <strong>limits</strong></li>
  <li>Abhängige Services und Infrastruktur werden nur bei Notwendigkeit mitgetestet</li>
</ul>
<div class="page-no">17</div>

---

<div class="section-title">Wie funktioniert ein Load Generator?</div>
<div class="image-frame">
  <img src="/assets/rendered/page-18.png" alt="Wie funktioniert ein Load Generator" />
</div>
<div class="page-no">18</div>

---

<div class="section-title">Wie funktioniert ein Load Generator?</div>
<div class="text-xl mb-8">Stages:</div>
<ul class="bullets text-xl">
  <li>Ramp-up</li>
  <li>Main test</li>
  <li>Ramp-down</li>
</ul>
<div class="text-xl mt-8 mb-4">Target Virtual Users:</div>
<ul class="bullets text-xl">
  <li>Parallele Ausführungen</li>
</ul>
<div class="page-no">19</div>

---

<div class="section-title">Wie funktioniert ein Load Generator?</div>
<div class="text-xl mb-8">Stages:</div>
<ul class="bullets text-xl">
  <li>Ramp-up</li>
  <li>Main test</li>
  <li>Ramp-down</li>
</ul>
<div class="text-xl mt-8 mb-4">Target Virtual Users:</div>
<ul class="bullets text-xl">
  <li>Parallele Ausführungen</li>
</ul>
<div class="text-xl mt-8">Die eigentlichen Tests</div>
<div class="page-no">20</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-21.png" alt="Visual slide 21" />
</div>
<div class="page-no">21</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-22.png" alt="Visual slide 22" />
</div>
<div class="page-no">22</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-23.png" alt="Visual slide 23" />
</div>
<div class="page-no">23</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-24.png" alt="Visual slide 24" />
</div>
<div class="page-no">24</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-25.png" alt="Visual slide 25" />
</div>
<div class="page-no">25</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-26.png" alt="Visual slide 26" />
</div>
<div class="page-no">26</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-27.png" alt="Visual slide 27" />
</div>
<div class="page-no">27</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-28.png" alt="Visual slide 28" />
</div>
<div class="page-no">28</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-29.png" alt="Visual slide 29" />
</div>
<div class="page-no">29</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-30.png" alt="Visual slide 30" />
</div>
<div class="page-no">30</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-31.png" alt="Visual slide 31" />
</div>
<div class="page-no">31</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-32.png" alt="Visual slide 32" />
</div>
<div class="page-no">32</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-33.png" alt="Visual slide 33" />
</div>
<div class="page-no">33</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-34.png" alt="Visual slide 34" />
</div>
<div class="page-no">34</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-35.png" alt="Visual slide 35" />
</div>
<div class="page-no">35</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-36.png" alt="Visual slide 36" />
</div>
<div class="page-no">36</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-37.png" alt="429 Too Many Requests" />
</div>
<div class="page-no">37</div>

---

<div class="section-title">Gelernte Lektionen (1 / 2)</div>
<div class="text-xl mb-6">Zugriff auf weitere Systeme notwendig:</div>
<ul class="bullets text-xl">
  <li>Monitoring</li>
  <li>Metriken</li>
  <li>Traces</li>
  <li>Logs</li>
</ul>
<div class="page-no">38</div>

---

<div class="section-title">Gelernte Lektionen (2 / 2)</div>
<ul class="bullets text-xl">
  <li>Lasttest vorher <strong>kommunizieren</strong> (relevante Abteilungen / Dienstleister)</li>
  <li>Nie mehr als <strong>eine Änderung</strong> gleichzeitig</li>
  <li>Veränderung und Ergebnis <strong>dokumentieren</strong></li>
  <li>Tests <strong>wiederholen</strong>, um zufällige äußere Faktoren aufzudecken</li>
  <li>Wenn etwas bricht, <strong>Ursache(n) finden</strong></li>
  <li>Dinge werden kaputt gehen</li>
</ul>
<div class="page-no">39</div>

---

<div class="image-frame">
  <img src="/assets/rendered/page-40.png" alt="Closing visual" />
</div>
<div class="page-no">40</div>

---
layout: center
class: text-center
---

<div class="text-4xl font-semibold mb-6" style="color:#123d7a">Vielen Dank</div>
<div class="text-xl">Stephan Schwarz</div>
<div class="text-lg mt-2">stephan.schwarz@iits-consulting.de</div>
<div class="page-no">41</div>
