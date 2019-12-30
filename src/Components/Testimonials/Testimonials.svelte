<script>
  export let testimonialData = {};
  const { HEADING, TESTIMONIAL_LIST } = testimonialData;
</script>
<!------------------------------------------->
<!----------------MARKUP----------------------->
<!------------------------------------------->

<section id="testimonials" class="section">
  <div class="container">
    <h2 class="title text-center">{HEADING}</h2>
    <div class="row offset-1 section-body">
      {#each TESTIMONIAL_LIST as list}
        <div class="col-md-5 testimonial">
          <p>{list.DESCRIPTION}</p>
          <img src={list.IMAGE_URL} alt="" />
          <p class="user-details">
            <b>{list.NAME}</b>
            <br />
            {list.DESIGNATION}
          </p>
        </div>
      {/each}
    </div>
  </div>
</section>
<!------------------------------------------->
<!----------------STYLE----------------------->
<!------------------------------------------->
<style>
  .testimonial {
    border-left: 4px solid #0072ff80;
    margin-top: 10px;
    margin-bottom: 10px;
  }

  .testimonial img {
    height: 60px;
    width: 60px;
    border-radius: 50%;
    margin: 0 10px;
  }

  .user-details {
    display: inline-block;
    font-size: 12px;
  }
</style>