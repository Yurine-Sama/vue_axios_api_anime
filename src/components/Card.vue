<template>
  <div class="card">
    <b-card :img-src="image" img-alt="Card image" img-top class="my-1">
      <b-card-text>
        {{ title }}
      </b-card-text>
    </b-card>
  </div>
</template>
<script>
export default {
  props: {
    title: String,
    image: String
  }
};
</script>
