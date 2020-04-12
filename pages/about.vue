<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About Us"
      image="/uploads/home.png"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>How can I learn to actually <i>speak<i> English?</h3>
          <p>
            Hi, I'm Anne. I created Elevate English after hundreds of students asked me this question. I can read, write and understand English, but I always feel blocked when speaking. What should I do? I developed a method to help English learners at all levels improve their speaking and overall language skills. This method is based on theories from psycholinguistics, learning psychology, and my experience as an ESL teacher.
          </p>
          <h3>The Elevate Method</h3>
          <p>
            1.Learn basic words and grammar
            2.Input: Listening and Reading
            3.Output: Speaking and Writing
            4.Regular Practice
          </p>
          <p>
            <strong>Read full post to learn more about the Elevate Method</strong> 
          </p>
          <h3>About Anne</h3>
           <p>
            <strong>
              BA Psychology, University of British Colombia
            </strong>
          </p>
          <p>
            I grew up in Seattle, in the United States. After high school I moved to Vancouver, Canada to study Psychology. I've loved traveling and learning languages since I was young. I got my certificate in Teaching English as a Foreign Language (TEFL) after graduation, and started traveling the world while teaching English. Six months ago I moved to France. I studied French in high school, but I didn't feel like I learned the language well with only grammar and vocabulary. Instead, I improved my French naturally by listening to podcasts, watching YouTube videos and TV shows, and by talking to new friends French, even though it was scary at first. I want to help my English students in the same way. Even if they can't move to an English speaking country, my podcasts, YouTube channel, and blog posts can help them learn English naturally at home.
          </p>
          <quote-card />
        </div>

        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Elevate English Podcast
              </p>
              <p class="subtitle">
               Interesting topics (slow or fast speaking speed) with full transcripts
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Elevate English on YouTube
              </p>
              <p class="subtitle">
                Watch videos about helpful language learning tips from Anne
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Elevate English Blog
              </p>
              <p class="subtitle">
                Read full length posts on interesting topics and language learning strategies
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
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
