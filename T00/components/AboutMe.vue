<script setup>
const scholar = {
  citations: 17249,
  hindex: 43,
  i10index: 107,
}

const publications = [
  {
    year: 2019,
    number: 1446
  },
  {
    year: 2020,
    number: 1596
  },
  {
    year: 2021,
    number: 1714
  },
  {
    year: 2022,
    number: 1868
  },
  {
    year: 2023,
    number: 1826
  },
  {
    year: 2024,
    number: 1890
  },
  {
    year: 2025,
    number: 1900
  },
  {
    year: 2026,
    number: 1202
  }
]
</script>

<template>
  <div class="page">
    <section class="bio">
      <div class="card">
        <ul>
          <li>
            <strong>Professor</strong> of Project Engineering and Management
            at the Department of Industrial Engineering, Business Administration, 
            and Statistics at the Universidad Politécnica de Madrid (UPM) since 2009.
            Employed at three Spanish universities.
          </li>
          <li>
            <strong>Visiting academic</strong> at various acdemic institutions including INRIA (FR), 
            ESTI (FR), University of Iowa (USA), BIT (CN), École Polytechnique (FR),
            UBI (PT), DTU (DK) and Brunel (UK).
          </li>
          <li>
            <strong>Participation</strong> in more than 20 EU-funded projects, 
            and more than 100 private transfer technology contracts.
          </li>
          <li>
            <strong>Co-author</strong> of more than 150 articles and 20 books.
          </li>
          <li>
            <strong>Co-inventor</strong> in more than 10 industrial patents, 
            some under exploitation.
          </li>
          <li>
            <strong>Supervisor</strong> of more than 30 PhD theses.
          </li>
          <li>
            <strong>Consultant</strong> for over 10 years. <it>Interest 
              in improving industrial processes using data-driven models,
              process optimization, business analytics, big data analytics 
              and project management</it> => <strong style="color:red;">Industrial Management</strong>.
          </li>
        </ul>
      </div>

      <div class="research-card">
        <h3>Research Focus</h3>
        <div class="venn">
          <div class="circle left">
            Industrial<br>Management
          </div>
          <div class="circle right">
            Digital<br>Technology
          </div>
          <div class="me">
            Me
          </div>
        </div>

      </div>
    </section>

    <section class="sidebar">
      <div class="profile-name">
        Joaquín Ordieres-Meré
      </div>
      <div class="profile">
        <a href="https://biba.etsii.upm.es/jom/" target="_blank">
        <img class="profile-photo" src="/images/JOM_PERSONALIA_400.png">
        </a>
      </div>

      <div class="pub-card">
        <div class="scholar-header">
          <span>Cited by </span>
          <span>(GScholar)</span>
        </div>
        <table class="metrics-table">
          <thead>
            <tr>
              <th></th>
              <th>All</th>
              <th>Since 2021</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Citations</td>
              <td>17249</td>
              <td>10404</td>
            </tr>
            <tr>
              <td>h-index</td>
              <td>43</td>
              <td>34</td>
            </tr>
            <tr>
              <td>i10-index</td>
              <td>107</td>
              <td>73</td>
            </tr>
          </tbody>
        </table>
      </div>

      <div class="chart-card">
        <div class="chart-container">
          <div class="y-axis">
            <span>2000</span>
            <span>1500</span>
            <span>1000</span>
            <span>500</span>
            <span>0</span>
          </div>

          <div class="chart">
            <div
              v-for="pub in publications"
              :key="pub.year"
              class="bar-wrapper"
            >
              <div
                class="bar"
                :style="{
                  height: `${pub.number / 2000 * 140}px`
                }"
              >
                <span class="tooltip">
                  {{ pub.number }}
                </span>
              </div>
              <div class="year-label">
                {{ pub.year }}
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

  </div>
</template>

<style scoped>
.page{
  display:grid;
  grid-template-columns: 75% 25%;
  gap:10px;
  height:100%;
  background:white;
}

h1{
  color:#0066c0;
  font-size:2.4rem;
  font-weight:700;
  margin-bottom:10px;
}

.card,
.research-card,
.pub-card{
  background:white;
  border-radius:14px;
  box-shadow:0 4px 14px rgba(0,0,0,.08);
  padding:10px;
}

.card ul{
  margin:0;
}

.card li{
  margin-bottom:6px;
  line-height:1.0;
  font-size:0.9rem;
}

.sidebar{
  display:flex;
  flex-direction:column;
  gap:5px;
}

.stats{
  display:grid;
  grid-template-columns:1fr;
  gap:10px;
}

.stat{
  background:linear-gradient(
    135deg,
    #005fb8,
    #2c87ff
  );
  color:white;
  border-radius:14px;
  padding:16px;
  text-align:center;
}

.stat span{
  display:block;
  font-size:2rem;
  font-weight:700;
}

.pub h3{
  margin-bottom:12px;
}

.pub{
  display:flex;
  gap:12px;
  margin-bottom:12px;
}

.year{
  min-width:55px;
  font-weight:700;
  color:#0066c0;
}

.title{
  font-size:.88rem;
  font-weight:600;
}

.venue{
  color:#666;
  font-size:.75rem;
}

.venn{
  position:relative;
  height:260px;
}

.circle{
  position:absolute;
  width:180px;
  height:160px;
  border-radius:50%;
  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;
  font-weight:700;
}

.left{
  left:60px;
  background:#00A7DCBB;
  color:white;
  justify-content:flex-start;
  padding-left:20px;
}

.right{
  left:190px;
  background:#EFD470CC;
  color:#0f4ea8;
  justify-content:flex-start;
  padding-left:70px;
}

.me{
  position:absolute;
  left:195px;
  top:10px;
  background:#e53935;
  color:white;
  padding:4px 6px;
  border-radius:8px;
  font-weight:600;
}

.scholar-header{
  display:flex;
  justify-content:space-between;
  align-items:center;

  margin-bottom:4px;

  font-size:0.75rem;
  font-weight:500;
}

.scholar-header a{
  color:#2d2dbe;
  font-size:0.8rem;
  text-decoration:none;
}

.metrics-table{
  width:100%;
  border-collapse:collapse;
  margin-bottom:6px;
  font-size:0.65rem;
}

.metrics-table th{
  font-weight:600;
  text-align:right;
  padding:2px 4px;
}

.metrics-table td{
  padding:2px 4px;
}

.metrics-table td:first-child{
  text-align:left;
}

.metrics-table td:not(:first-child){
  text-align:right;
}

.y-axis{
  width:35px;

  display:flex;
  flex-direction:column;
  justify-content:space-between;

  text-align:right;

  font-size:0.5rem;
  color:#666;
}

.chart{
  flex:1;

  display:flex;
  align-items:flex-end;
  gap:1px;

  position:relative;

  border-left:1px solid #bbb;
  border-bottom:1px solid #bbb;
  padding-left:4px;
}

.chart-container{
  display:flex;
  gap:8px;
  height:180px;
}

.chart::before{
  content:'';

  position:absolute;
  inset:0;

  background:
    repeating-linear-gradient(
      to top,
      #e5e5e5 0px,
      #e5e5e5 1px,
      transparent 1px,
      transparent 25%
    );

  pointer-events:none;
}

.bar-wrapper{
  width:22px;
  flex:none;

  display:flex;
  flex-direction:column;
  align-items:center;
  justify-content:flex-end;

  height:100%;
}

.bar{
  width:80%;
  background:#8c8c8c;
  border-radius:3px 3px 0 0;
  position:relative;
  cursor:pointer;
  transition:.2s;
}

.bar:hover{
  background:#5d5d5d;
}

.year-label{
  margin-top:6px;
  font-size:0.45rem;
  color:#666;
}

.profile{
  display:flex;
  justify-content:center;
  margin-bottom:6px;
}

.profile-photo{
  width:auto;
  max-width:90px;
  height:100px;
  border-radius:10px;
  border:1px solid #ddd;
  box-shadow:0 2px 8px rgba(0,0,0,.15);
}

.profile-name{
  text-align:center;
  font-size:0.80rem;
  font-weight:600;
  margin-bottom:2px;
}

.profile-link{
  text-align:center;
  font-size:0.65rem;
  color:#666;
  margin-bottom:8px;
}

.profile-photo:hover{
  transform:scale(1.03);
  box-shadow:
    0 6px 16px rgba(0,0,0,.25);
}

.tooltip{
  position:absolute;
  top:-30px;
  left:50%;
  transform:translateX(-50%);
  background:#222;
  color:white;
  padding:3px 6px;
  font-size:.45rem;
  border-radius:4px;
  white-space:nowrap;
  opacity:0;
  pointer-events:none;
  transition:.2s;
}

.bar:hover .tooltip{
  opacity:1;
}


</style>


