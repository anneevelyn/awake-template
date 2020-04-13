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
          <ol>
            <li>Learn basic words and grammar</li>
            <li>Input: Listening and Reading</li>
            <li>Output: Speaking and Writing</li>
            <li>Regular Practice</li>
          </ol>
          <p>
            <strong>Read full post to learn more about the Elevate Method</strong> 
          </p>
          <br />
          <article class="tile is-child box">
            <p class="title">
              About Anne
            </p>
            <p class="subtitle">
              BA Psychology, University of British Colombia
            </p>
            <img src="../assets/uploads/contact.jpg" height="500" />
          </article>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="subtitle">
                I grew up in Seattle, in the United States. After high school I moved to Vancouver, Canada to study Psychology. I've loved traveling and learning languages since I was young. I got my certificate in Teaching English as a Foreign Language (TEFL) after graduation, and started traveling the world while teaching English. Six months ago I moved to France. I studied French in high school, but I didn't feel like I learned the language well with only grammar and vocabulary. Instead, I improved my French naturally by listening to podcasts, watching YouTube videos and TV shows, and by talking to new friends French, even though it was scary at first. I want to help my English students in the same way. Even if they can't move to an English speaking country, my podcasts, YouTube channel, and blog posts can help them learn English naturally at home.
              </p>
            </article>
          </div>
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
