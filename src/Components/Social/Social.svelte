<script>
  export let socialData = {};
  const { IMAGES_LIST, HEADING } = socialData;
</script>

<style>
  .social-icons img {
    width: 75px;
    transition: 0.5s;
  }
  .social-icons a:hover img {
    transform: translateY(-10px);
  }
  a:hover {
    text-decoration: none;
  }
</style>

<!------------------------------------------->
<!----------------MARKUP----------------------->
<!------------------------------------------->
<section id="social-media" class="section grey-bgcolor">
  <div class="container text-center">
    <h2 class="title text-center">{HEADING}</h2>
    <div class="social-icons section-body">
      {#each IMAGES_LIST as list}
        <a
          href="https://www.linkedin.com/in/nikhil-karkra-73a15319/"
          target="_blank">
          <img src={list} alt="Social media {list}" />
        </a>
      {/each}
    </div>
  </div>
</section>
<!------------------------------------------->
<!----------------STYLE----------------------->
<!------------------------------------------->
