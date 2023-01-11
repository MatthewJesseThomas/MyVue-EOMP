<template>
    <div>
        <section id="contact" class="container-fluid text-center">
        <h2 class="display-4 text-light mt-0 rounded-3 barney kage animate-charcter fw-bolder" data-aos="zoom-in">Contact</h2>
        <div class="container">
            <form action="https://formspree.io/f/mwkzbykn" method="POST">
                <div >
                    <label for="#firstname" class="fs-1 animate-charcter fw-bold">Name</label>
                    <input id="firstname" name="firstName" type="text" placeholder="Enter your name" required  class="w-100">
                </div>
                <div>
                    <label for="#firstname" class="fs-1 animate-charcter fw-bold">Surname</label>
                    <input id="surname" name="surname" type="text" placeholder="Enter your surname" required  class="w-100">
                </div>
                <div>
                    <label for="#email" class="fs-1 animate-charcter fw-bold">Email</label>
                    <input id="Email" name="Email" type="text" placeholder="Enter your Email" required class="w-100">
                </div>
                <div>
                    <label for="#Response" class="fs-1 animate-charcter fw-bold">Message</label>
                    <textarea name="message" cols="30" rows="10" placeholder="Enter your Message" required type="reset"  class="w-100"></textarea>
                </div> <br>
                <div>
                  <select class="form-select" aria-label="Default select example">
                      <option selected disabled class="fs-2 fw-bold">Gender</option>
                      <option class="fs-2" value="1">Male</option>
                      <option class="fs-2" value="2">Female</option>
                      <option class="fs-2" value="3">Other</option>
                  </select>
              </div> <br>
                <div>
                    <input id="submit" type="submit" value="submit">
                </div>
            </form>
        </div> <br>
        <ul class="list-unstyled text-light bg-dark offsite kage animate-charcter" data-aos="flip-left"
        data-aos-easing="ease-out-cubic"
        data-aos-duration="2000">
            <li><strong>Telephone:0213713910</strong></li>
            <br>
            <li><strong>Cellphone:0827294648</strong></li>
            <br>
            <li><strong>owlsaintgermain@gmail.com</strong></li>
            <br>
        </ul>
        </section>
    </div>
</template>
<script>
export default {
    name:'ContactForm'

};
</script>
<style>
#contact{
    margin-top: 9rem;
}   
</style>