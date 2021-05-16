<template>
  <section class="discover">
    <img src="../assets/analytics.svg" alt="analytics" class="icon-big" />
    <h1><strong>DISCOVER</strong></h1>
    <p>BOOKED TOOL</p>
    <img v-if="data === 'A'" src="../assets/img1.webp" alt="analytics-img" />
    <img
      v-else-if="data === 'B'"
      src="../assets/img2.webp"
      alt="analytics-img"
    />
    <img
      v-else-if="data === 'C'"
      src="../assets/img3.webp"
      alt="analytics-img"
    />
    <img
      v-else-if="data === 'D'"
      src="../assets/img4.webp"
      alt="analytics-img"
    />
    <div class="discover__options">
      <div
        class="discover__option"
        v-bind:class="[data == 'A' ? ' discover__option__active' : '']"
        @click="handleClick"
        ref="A"
      >
        Discover A
      </div>
      <div
        class="discover__option"
        v-bind:class="[data == 'B' ? ' discover__option__active' : '']"
        @click="handleClick"
        ref="B"
      >
        Discover B
      </div>
      <div
        class="discover__option"
        v-bind:class="[data == 'C' ? ' discover__option__active' : '']"
        @click="handleClick"
        ref="C"
      >
        Discover C
      </div>
      <div
        class="discover__option"
        v-bind:class="[data == 'D' ? ' discover__option__active' : '']"
        @click="handleClick"
        ref="D"
      >
        Discover D
      </div>
    </div>
    <p class="discover__text" v-if="data === 'A'">
      <strong>Discover A</strong> Lorem ipsum dolor sit amet consectetur
      adipisicing elit. Ducimus vel omnis nemo iste eos quia voluptatem delectus
      consectetur beatae eveniet!
    </p>
    <p class="discover__text" v-else-if="data === 'B'">
      <strong>Discover B</strong> Lorem ipsum dolor, sit amet consectetur
      adipisicing elit. Itaque, molestias.
    </p>
    <p class="discover__text" v-else-if="data === 'C'">
      <strong>Discover C</strong> Lorem ipsum dolor sit amet consectetur
      adipisicing elit. Voluptates quis nihil odio fugit, natus quod quasi
      deleniti cumque dicta, numquam recusandae hic perspiciatis tenetur
      possimus? Necessitatibus autem vero perspiciatis fugiat!
    </p>
    <p class="discover__text" v-else-if="data === 'D'">
      <strong>Discover D</strong> Lorem ipsum dolor sit amet, consectetur
      adipisicing elit. Quis reiciendis, libero quam voluptatem sequi, sint,
      voluptate minus non quo odio perspiciatis velit asperiores beatae
      dignissimos molestias. Inventore cumque quia atque, ratione nam fuga
      repudiandae consectetur delectus, nostrum, tenetur ea quo.
    </p>
  </section>
</template>
<script>
export default {
  data() {
    return {
      data: "A",
    };
  },
  methods: {
    handleClick(e) {
      switch (e.target.innerText) {
        case "Discover A":
          this.data = "A";
          break;
        case "Discover B":
          this.data = "B";
          break;
        case "Discover C":
          this.data = "C";
          break;
        case "Discover D":
          this.data = "D";
          break;
      }
    },
  },
};
</script>
