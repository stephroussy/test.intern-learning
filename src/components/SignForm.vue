<template>
    <div>
        <h2 class = headingText>SHIFT YOUR CAREER INTO OVERDRIVE!</h2>
        <h4 class="formInfo">{{ formInfo }}</h4>
        <img
            :src="require('@/assets/interested.jpg')"
            alt="interested"
            class="interested-img"
        />
        <form>
            <label class="name">Name (required) </label> <br>
            <input class = "name" type="text" required> <br>
            <label class="phone">Phone:</label> <br>
            <input class = "phone" type="text"> <br>
            <button>I'm Interested!</button>
        </form>
    </div>
</template>

<script>
export default {
    data() {
        return{
            text: "",
            formInfo: "We're seeking friendly, happy individuals up for the challenge to change the way people view the automotive industry. If you agree that a customer's time is valuable and positive human interaction is important, then we want to hear from you!"
                
            
        }
    }
}

</script>

<style lang="scss" scoped>

.formInfo {
    margin-left: 8rem;
    margin-top: .2rem;
    position: absolute;
    left: 7rem;
    right: 44rem;}

form {
    margin-left: 8rem;
    margin-top: 7rem;
    position: absolute;
    left: 7rem;
    max-height: 40%;
    font-weight: bold;
    line-height: 2.5rem;
    font-size: 1.5rem;}

button {
    height: 4rem;
    width: 30rem;
    font-size: 1.7rem;
    background-color: #ffd900;
    font-weight: bold;
    margin-top: 1rem;
    margin-bottom: 3rem;
}

.headingText {  
    margin-top: 45rem;
    border-bottom: 6px solid var(--color-highlight);
    font-size: 44px;
    text-transform: uppercase;
}

input {
    width: 30rem;
    height: 2.5rem;
}

.interested-img {
    margin-left: 33rem;
    margin-top: .7rem;
    position: absolute;
    max-height: 40%;
    width: 30%;
    height: 60%;
    margin-right: 5rem;
}

</style>
