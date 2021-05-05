<template>

    <div class="card faq-card">
        <header class="card-header">
            <p class="card-header-title">
                Is INFINITY deflationary?
            </p>
        </header>
        <div class="card-content">
            <div class="content has-text-left">
                <p>INFINITY rebases a total of 500,000 tokens at the end of each cycle which means that 137,500 are burned perminently each cycle. The contract owner can set the number of cycles after which FOT will become 0 which means burning will cease. This is initially set to 500 cycles after which the total supply will have reduced from 100mm tokens to 31,250,000 tokens.</p>
            </div>
        </div>
        <footer class="card-footer">
            <p class="card-footer-item">
                <span class="subtitle is-6 has-text-black">INFINITY is a deflationary supply elastic protocol</span>
            </p>
        </footer>
    </div>
    <div class="card tweet-card">
        <div class="card-content">
            <p class="title is-4">
                Thank you
                @coingecko
                for the listing. As the first
                @degen_vc
                project to be listed on
                @PancakeSwap
                , we are pioneering a new frontier in store of value and Defi. Come join us in the fun!
            </p>
            <p class="subtitle">
                @infinity_proto
            </p>
        </div>
        <footer class="card-footer">
            <p class="card-footer-item">
              <span>
                View on <a href="https://twitter.com/infinity_proto/status/1389475241756225542">Twitter</a>
              </span>
            </p>
        </footer>
    </div>
    <div class="card faq-card">
        <header class="card-header">
            <p class="card-header-title">
                What is the purpose of the rebase?
            </p>
        </header>
        <div class="card-content">
            <div class="content has-text-left">
                <p>First things first. What is a rebase? A rebase is an adjustment to the balance of tokens in the wallets of everyone holding the tokens. So, if there is a 10% rebase everyone has 10% more tokens in their wallet than they had before. It is an expansion or contraction of supply therefore.</p>
                <p>At first glance, it might look like INFINITY’s burn and rebase is about reducing supply to affect price. But, historically, token burns for most projects don’t make much impact on price — that is to say price can tend to be insensitive to burns — and in the case of INFINITY the max burn before rebase is less than 1% of supply so it is not dramatic.</p>
                <p>No, its not about stimulating price. The purpose of the INFINITY rebase is to redistribute INFINITY to longer term holders.</p>
                <p>A person who supports the INFINITY model could plan in hodl INFINITY for an extended period of time. And by “extended” we mean more than a year (Yes, such people do exist even in DeFi). This person benefits from continuous top-ups of tokens to their wallet via the rebase mechanism.</p>
            </div>
        </div>
        <footer class="card-footer">
            <p class="card-footer-item">
                <span class="subtitle is-6 has-text-black">Essentially, de facto farming by hodl</span>
            </p>
        </footer>
    </div>

    <div class="card">
        <div class="card-image">
            <figure class="image is-5by3">
                <a href="https://medium.com/infinitywin/infinity-protocol-ec2e3b84e988"><img src="../assets/medium-header.png"></a>
            </figure>
        </div>
        <div class="card-content">
            <div class="media">
                <div class="media-content">
                    <p class="title is-4"><a href="https://medium.com/infinitywin/infinity-protocol-ec2e3b84e988" class="has-text-black">Infinity Protocol</a></p>
                </div>
            </div>

            <div class="content">
                The problem with DeFi’s store-of-value economic experiments (Core, Axion, Safemoon, Lighting etc) is that they are all predicated on the same idea that their innovation represents the ultimate innovation. But only one thing holds true for innovation — innovation is always trumped by better innovation.
            </div>
        </div>
        <footer class="card-footer">
            <p class="card-footer-item">
              <span>
                <a href="https://medium.com/infinitywin/infinity-protocol-ec2e3b84e988">Read More</a>
              </span>
            </p>
        </footer>
    </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    type: String,
    name: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .card {
        margin: 1em;
        height: fit-content;
        opacity: 0.75;
        min-width: 360px;
    }
    .card:hover {
        opacity: 1;
    }
    .faq-card {
        min-width: 500px;
    }
</style>
