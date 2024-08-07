<template>
  <section class="container" id="about">
    <h1>About</h1>
    <div class="row gx-5">
      <figure class="col-md-6">
        <img src="../assets/images/profile.jpg" alt="">
        <figcaption>About Euicheol Choi</figcaption>
      </figure>
      <p class="col-md-6">Lorem ipsum dolor sit amet conse</p>
    </div>
    <article class="row py-5">
      <h2>Skills</h2>
      <dl>
        <template v-for="item in skills">
          <dt class="lead">{{ item.name }}</dt>
          <dd>
            <div class="progress" role="progressbar">
              <div 
                class="progress-bar text-end pe-3" 
                :style="{ width: item.point }"
              >{{ item.point }}</div>
            </div> 
          </dd> 
        </template>
      </dl>
    </article>
  </section>
</template>
<script setup>
  const skills = [
    { name: 'HTML', point: '90%'},
    { name: 'CSS', point: '80%'},
    { name: 'JavaScript', point: '50%'},
    { name: 'Vue', point: '75%'},
  ]
</script>
<style lang="scss">
figure {
  img {width: 100%;}
}
</style>