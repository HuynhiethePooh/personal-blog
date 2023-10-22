<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About Me"
      subtitle="Why does this page exist?"
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Going through your 20's in the modern world</h3>
          <p>
            I have always loved going to random longform blogs and just reading
            even though it's a much less sexy alternative to quick videos and social
            media. There is something about finding these little nooks and crannies 
            where people write about what they love regardless of the view counts. Primarily
            growing up a STEM kid and not being great at English or writing, I've found an 
            appreciation for the art of writing and would love to have my own little corner of the
            internet to do so.
          </p>

          <h3>What is the point of my website?</h3>
          <p>
            Honestly, I don't know! I have so many passions just like everyone else growing up in such 
            a fast paced world, but they still feel special to me. Being able to see the special even if
            none of us are really that unique feels so human. I plan on writing about food, travels, books and
            whatever else I obsess with at the moment. Maybe the one person who somehow finds my corner of the internet
            feels connected to me for a moment too!
          </p>
        </div>

        <!-- <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Cool Stuff We Do
              </p>
              <p class="subtitle">
                Sooo Cool
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Other Cool Things
              </p>
              <p class="subtitle">
                Just as cool
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                All the cool
              </p>
              <p class="subtitle">
                that is all
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
        </div> -->
      </template>

      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest Posts
        </h3>
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
