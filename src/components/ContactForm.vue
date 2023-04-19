<template>
    <h2 class="display-4 text-light mt-0 kage fw-bolder" data-aos="zoom-in">Contact</h2>
    <div class="Ama-Superstar">
    <div id="contact" class="container-fluid text-center">
        <div class="container container-border">
            <form action="https://formspree.io/f/mdovovaj" method="POST" default class="m-2">
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
                    <input id="Email" name="Email" type="email" placeholder="Enter your Email" required class="w-100">
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
                <button class="bttn" id="submit" type="submit" value="submit">submit</button>
            </form>
        </div> 
        <br>
    </div>
    <div class="Contact-Info text-dark  kage animate-charcter w-50">
        <div class="Contact-Info-Name">
            <h1>Name</h1>
            <h2>Matthew Jesse Thomas</h2>
        </div>
        <br>
        <br>
        <br>
        <div class="Contact-Info-Email">
            <h1>Email</h1>
            <h2>owlsaintgermain@gmail.com</h2>
        </div>
        <br>
        <br>
        <br>
        <div class="Contact-Info-Phone">
            <h1>Phone Number</h1>
            <h2>0827294648</h2>
        </div>
        <br>
        <br>
        <br>
        <div class="Contact-Info-Address">
            <h1>Address</h1>
            <h3>South Africa</h3>
            <h3>Western Cape</h3>
            <h3>Cape Town</h3>
            <h3>Mitchell's Plain</h3>
        </div>
    </div>
</div>
</template>
<script>
export default {
    name:'ContactForm'

};
</script>
<style>
#contact{
    margin-top: 5rem;
    z-index: 1;
    position: relative;
}
.Contact-Info{
    margin-top: 7rem;
    margin-right: 5rem;
    z-index: 1;
    position: relative;
}
.bttn{
    width: 15rem;
    height: 3rem;
    border-radius: 2rem;
} 
.bttn:hover{
    scale: 1.1;
    color: #638889;
    background-color: #663399;
} 
.container{
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
} 

.Ama-Superstar{
    margin: auto;
    justify-content: space-between;
    display: flex;
    background-color: #63888951;
}
</style>