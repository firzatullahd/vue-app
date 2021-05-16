<template>
  <section class="contact">
    <img src="../assets/contact-form.svg" class="icon-big" />
    <h2><strong>Get in touch</strong></h2>
    <p>
      Want to get in touch? We'd love to hear from you. Here's how you can reach
      us..
    </p>
    <div class="input-container">
      <img src="../assets/search.svg" alt="search" class="icon" />
      <input type="text" placeholder="Search..." />
    </div>
    <div class="contact__content">
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d15829.94274050131!2d112.69453971977539!3d-7.299201349999992!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x914612d509cc37f6!2sShangri-La%20Hotel%2C%20Surabaya!5e0!3m2!1sen!2sid!4v1620798469474!5m2!1sen!2sid"
        class="contact__content__maps"
        style="border: 0"
        loading="lazy"
      ></iframe>
      <form class="feedback-form">
        <h3>Feedback</h3>
        <div class="contact__content__name">
          <input type="text" placeholder="First" />
          <input type="text" placeholder="Last" />
        </div>
        <input type="email" placeholder="Email" />
        <textarea rows="4" cols="30" placeholder="Message"></textarea>
        <button>Send</button>
      </form>
    </div>
  </section>
</template>
