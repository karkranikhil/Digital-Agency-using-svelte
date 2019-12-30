<script>
  export let footerData = {};
  export let header = "";
  const {
    DESCRIPTION,
    CONTACT_DETAILS,
    SUBSCRIBE_NEWSLETTER,
    SUBSCRIBE
  } = footerData;
  const { HEADING, ADDRESS, MOBILE, EMAIL } = CONTACT_DETAILS;
</script>

<!------------------------------------------->
<!----------------MARKUP----------------------->
<!------------------------------------------->
<section class="main-bgcolor light-color" id="footer">
  <img src="images/wave2.png" alt="" class="wave-img" />
  <div class="container">
    <div class="row section-body">
      <div class="col-md-4 footer-box">
        <div class="company_brand">{header}</div>
        <p>{DESCRIPTION}</p>
      </div>
      <div class="col-md-4 footer-box">
        <p class="footer-title">{HEADING}</p>
        <p>
          <i class="fas fa-map-marker-alt" />
          {ADDRESS}
        </p>
        <p>
          <i class="fas fa-phone" />
          {MOBILE}
        </p>
        <p>
          <i class="fas fa-envelope" />
          {EMAIL}
        </p>
      </div>
      <div class="col-md-4 footer-box">
        <p class="footer-title">{SUBSCRIBE_NEWSLETTER}</p>
        <input
          type="email"
          class="form-control round-border"
          placeholder="Your Email" />
        <button type="button" class="btn btn-outline-light round-border">
          {SUBSCRIBE}
        </button>
      </div>
    </div>
  </div>
</section>
<!------------------------------------------->
<!----------------Style----------------------->
<!------------------------------------------->
<style>
  .footer-title {
    font-weight: bold;
    text-transform: uppercase;
  }

  .footer-box button {
    margin-top: 30px;
  }

  .round-border {
    border-radius: 20px !important;
  }
  .wave-img {
    width: 100%;
    height: auto;
  }
</style>