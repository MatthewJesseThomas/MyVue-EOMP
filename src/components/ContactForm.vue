<template>
    <h2 class="display-4 text-light mt-0 kage fw-bolder" data-aos="zoom-in">Contact</h2>
    <div class="Ama-Superstar">
    <div id="contact" class="container-fluid text-center">
        <div class="container container-border-info">
            <form action="https://formspree.io/f/mdovovaj" method="POST" default class="m-2">
                <div class="myForm">
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
    border-radius: 10px;
} 
.bttn:hover{
    scale: 1.1;
    color: #638889;
    background-color: #5f3d81b2;
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
.myForm{
    width: 70rem;
}
.div, input, textarea{
    border-radius: 8px;
}
</style>