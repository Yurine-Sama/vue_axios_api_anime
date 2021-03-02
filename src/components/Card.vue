<template>
  <div class="card bg-warning text-center">
    <b-card
      style="color:Salmon"
      :img-src="image"
      img-alt="Card image"
      img-height="550px"
      img-width="250px"
      img-top
    >
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
