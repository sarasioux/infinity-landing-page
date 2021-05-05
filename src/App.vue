<template>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@0.9.2/css/bulma.min.css">

    <div class="container">
        <section class="header-section section">

        </section>
        <section class="logo-section section">
            <div class="columns is-centered is-vcentered">
                <div class="column is-2">
                    <Network
                            name="Ethereum Chain"
                            logo="ethereum"
                            link="https://ethereum.infinityprotocol.io/"
                    />
                </div>
                <div class="column">
                    <br />
                    <Logo/>
                    <br />
                </div>
                <div class="column is-2">
                    <Network
                            name="Binance Chain"
                            logo="ethereum"
                            link="https://bsc.infinityprotocol.io/"
                    />
                </div>
            </div>
        </section>
        <section class="title-section section">
            <LogoTitle />
        </section>
        <section class="icons-section section">
            <IconLink v-for="icon in getIconLinks()" :key="icon.icon"
                      :icon="icon.icon"
                      :link="icon.link"
                      :alt="icon.alt"
            />
        </section>
        <section class="cards-section section is-clearfix">
            <InfiniteCards />
        </section>
    </div>
</template>

<script>

import Logo from './components/Logo.vue'
import LogoTitle from './components/LogoTitle.vue'
import Network from './components/Network.vue'
import InfiniteCards from './components/InfiniteCards.vue'
import IconLink from './components/IconLink.vue'

export default {
  name: 'App',
  components: {
    Logo, LogoTitle, Network, InfiniteCards, IconLink
  },
  methods: {
    getIconLinks: () => {
      return [
        {
          icon: 'twitter',
          link: 'https://twitter.com/infinity_proto',
          alt: 'View our Twitter feed!'
        },
        {
          icon: 'github',
          link: 'https://github.com/degen-vc/infinity-contracts',
          alt: 'Check out the code!'
        },
        {
          icon: 'medium',
          link: 'https://medium.com/infinitywin',
          alt: 'Read the whitepaper!'
        },
        {
          icon: 'telegram',
          link: 'https://t.me/infinityprotocol',
          alt: 'Join us on Telegram!'
        },
        {
          icon: 'discord',
          link: '#',
          alt: 'Join us on Discord!'
        }
        /*
        ,
        {
          icon: 'uniswap',
          link: '#',
          alt: 'View our Twitter feed!'
        },
        {
          icon: 'dext',
          link: '#',
          alt: 'View our Twitter feed!'
        },
        */
      ]
    }
  }
}
</script>

<style>
    #app {
      font-family: Avenir, Helvetica, Arial, sans-serif;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      text-align: center;
      color: #2c3e50;
    }

    html, body {
        /* height: 100%; */
    }

    body {
        background-image: url("assets/background.png");
        background-size: cover;
        background-position: 50%;
        background-repeat: no-repeat;
        background-attachment: fixed;
    }


</style>
