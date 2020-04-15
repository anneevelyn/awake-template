<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Podcast"
      image="/uploads/podcast.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Elevate English Podcast</h3>
          <p>
            <strong>This podcast is for intermediate English learners who want something interesting to listen to.</strong>
          </p>
          <p>
            I noticed that there are a lot of apps, books, and exercises for beginners, for people who are just starting to learn English. And for people who have an advanced level, they can read, watch, or listen to English content for native speakers, like American TV shows or British newspapers, because they can already understand it. 
          </p>
          <p>
            But between those two groups, there are people who have an intermediate level who can’t always understand traditional English media. They find that native speakers talk too fast for example, or they use complicated words and expressions. This podcast will help you learn English through listening to lots of different interesting subjects. We won’t learn grammar rules or memorize lists of words. Instead, I will simply speak to you about things like travel, culture, history, and psychology, my favorite subject. 
          </p>
          <p>
            I want your opinions! If there is a topic you want me to make an episode about, use the <a href="/contact"> Contact</a> form on my website to let me know. Put "Podcast Idea" as the subject tell me about your ideas.
          </p>
         <quote-card />
        </div>

        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Podcast
              </p>
              <p class="subtitle">
               Interesting topics (choose slow or fast speaking speed) with full transcripts
              </p>
              <img src="../assets/uploads/podcast-tile.png" />
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                YouTube
              </p>
              <p class="subtitle">
                Language learning tips, idiomatic expressions, and other fun English content
              </p>
              <img src="../assets/uploads/youtube-tile.png" /> 
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Blog
              </p>
              <p class="subtitle">
                Read full length posts on interesting topics and language learning strategies
              </p>
              <img src="../assets/uploads/blog-tile.png" />
            </article>
          </div>
        </div>
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
import QuoteCard from '~/components/cards/QuoteCardTwo'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
