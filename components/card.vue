<template>
  <div class="card-card card">
    <div class="card-header">
      <img alt="image" :src="Icon" class="card-icon" />
      <svg viewBox="0 0 950.8571428571428 1024" class="card-icon1">
        <path
          d="M920.571 554.857c0 19.429-8 37.714-21.143 51.429l-42.857 42.857c-13.714 13.714-32.571 21.714-52 21.714s-38.286-8-51.429-21.714l-168-167.429v402.286c0 41.143-34.286 66.857-73.143 66.857h-73.143c-38.857 0-73.143-25.714-73.143-66.857v-402.286l-168 167.429c-13.143 13.714-32 21.714-51.429 21.714s-38.286-8-51.429-21.714l-42.857-42.857c-13.714-13.714-21.714-32-21.714-51.429s8-38.286 21.714-52l372-372c13.143-13.714 32-21.143 51.429-21.143s38.286 7.429 52 21.143l372 372c13.143 13.714 21.143 32.571 21.143 52z"
        ></path>
      </svg>
      <h3 class="card-heading">{{ Title }}</h3>
    </div>
    <p class="card-text">{{ Description }}</p>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    Icon: {
      type: String,
      default: '/group 1642.svg',
    },
    Title: {
      type: String,
      default: 'Accelerate your growth',
    },
    Description: {
      type: String,
      default: 'We use data to help you make better decisions, faster.',
    },
  },
}
</script>

<style scoped>
.card-card {
  position: relative;
}
.card-header {
  gap: var(--dl-space-space-oneandhalfunits);
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}
.card-icon {
  height: 50px;
  object-fit: cover;
}
.card-icon1 {
  width: 24px;
  height: 24px;
}
.card-heading {
  color: rgb(18, 40, 33);
  font-size: 24px;
  max-width: 600px;
  font-style: normal;
  font-weight: 500;
}
.card-text {
  color: rgb(18, 40, 33);
  max-width: 600px;
  font-family: Lato;
  line-height: 24px;
}
</style>
