<template>
    <div class="cards-wrapper is-clearfix">
        <div class="cards is-clearfix">
            <Card />
            <Card />
            <Card />
            <Card />
            <Card />
            <Card />
            <Card />
        </div>
    </div>
</template>

<script>
  import Card from './Card.vue'

export default {
  name: 'InfiniteCards',
  components: {
    Card
  },
  data: function() {
    return {
      cards: []
    }
  },
  mounted: function() {
    this.cards = [
      "Read our awesome Medium article!",
      "Latest updates from Twitter",
      "Don't miss our whitepaper",
      "This shit is bomb",
      "It totally should be working",
      "Read our awesome Medium article!",
      "Latest updates from Twitter",
      "Don't miss our whitepaper",
      "This shit is bomb",
      "It totally should be working"
    ]

  }
}
</script>

<style scoped>
    .cards-wrapper {
        min-height: 500px;
        height: fit-content;
    }
    .cards {
        display: flex;
        position: relative;
        animation: cards-revolving 40s linear infinite both;
    }
    .cards:hover {
        animation-play-state: paused;
    }
    @keyframes cards-revolving {
        0% {
            transform: translateX(-20%)
        }

        to {
            transform: translateX(-300%)
        }
    }
</style>
