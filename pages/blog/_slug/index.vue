<template>
  <section class="post-content-area single-post-area">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-lg-8 posts-list">
          <div class="single-post row">
            <div class="col-lg-12">
              <div class="feature-img">
                <img class="img-fluid" src="@/assets/img/blog/feature-img1.jpg" alt="">
              </div>
            </div>
            <div class="col-lg-3  col-md-3 meta-details">
              <ul class="tags">
                <li><a href="#">Food,</a></li>
                <li><a href="#">Technology,</a></li>
                <li><a href="#">Politics,</a></li>
                <li><a href="#">Lifestyle</a></li>
              </ul>
              <div class="user-details row">
                <p class="user-name col-lg-12 col-md-12 col-6"><a href="#">Mark wiens</a> <span class="lnr lnr-user"></span></p>
                <p class="date col-lg-12 col-md-12 col-6"><a href="#">12 Dec, 2017</a> <span class="lnr lnr-calendar-full"></span></p>
                <p class="view col-lg-12 col-md-12 col-6"><a href="#">1.2M Views</a> <span class="lnr lnr-eye"></span></p>
                <p class="comments col-lg-12 col-md-12 col-6"><a href="#">06 Comments</a> <span class="lnr lnr-bubble"></span></p>
                <ul class="social-links col-lg-12 col-md-12 col-6">
                  <li><a href="#"><i class="fa fa-facebook"></i></a></li>
                  <li><a href="#"><i class="fa fa-twitter"></i></a></li>
                  <li><a href="#"><i class="fa fa-github"></i></a></li>
                  <li><a href="#"><i class="fa fa-behance"></i></a></li>
                </ul>
              </div>
            </div>
            <div class="col-lg-9 col-md-9">
              <div v-html="posts[$route.params.slug]"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

</template>

<script>
  import Hello from '@/md/hello.md';
  import Diary from '@/md/diary.md';
  import LastTrip from '@/md/last-trip.md';

    export default {
        name: "BlogSingle",

      data() {
          return {
            posts: {
              hello: Hello,
              diary: Diary,
              'last-trip': LastTrip,
            }
          }
      }
    }
</script>

<style scoped>

</style>
