<template>
  <div>
    <div class="row-12">
      <button @click="Like()" class="btn btn-outline-info">
        <i class="bi bi-emoji-laughing-fill" aria-hidden="true"></i> Like
      </button>
      <button @click="Dislike()" class="btn btn-outline-info">
        <i class="bi bi-emoji-frown-fill" aria-hidden="true"></i> Dislike
      </button>
      <button @click="Love()" class="btn btn-outline-info">
        <i class="bi bi-suit-heart-fill" aria-hidden="true"></i> Love
      </button>
      <button @click="Sad()" class="btn btn-outline-info">
        <i class="bi bi-emoji-expressionless-fill"></i> Sad
      </button>
      <button @click="reset()" class="btn btn-outline-info">
        <i class="bi bi-x-circle-fill" aria-hidden="true"></i> reset
      </button>
      <br />
      <br />
      <p v-bind:style="{fontSize: fonts + 'px' }">{{ counter }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data: function () {
    return {
      counter: 0,
      fonts: 50,
    };
  },
  methods: {
    Like: function () {
      this.counter += 1;
      console.log(this.counter);
    },
    Dislike: function () {
      this.counter -= 5;
      console.log(this.counter);
    },
    Love: function () {
      this.counter += 5;
      console.log(this.counter);
    },
    Sad: function () {
      this.counter -= 1;
      console.log(this.counter);
    },
    reset: function () {
      this.counter = 0;
      console.log(this.counter);
    },
  }, 
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
