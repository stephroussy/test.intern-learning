<template>
    <div class="chapman-cares">
        <HeadingText>Chapman Cares</HeadingText>

        <img
            :src="require('@/assets/cares-banner.jpg')"
            alt="Chapman Cares"
            class="banner-img"
        />
        <img
            :src="require('@/assets/making-strides.jpg')"
            alt="making strides"
            class="strides-img"
        />
        <div v-for="(event, index) in events" :key="index" class="event">
            <h3 class="event-name1">{{ event.name1 }}</h3>
            <p class="event-text1">{{ event.text1 }}</p>
        </div>
        
        <img
            :src="require('@/assets/canine-companions.jpg')"
            alt="canine companion"
            class="canine-img"
        />

        <div v-for="(event, index) in events" :key="index" class="event">
            <h3 class="event-name2">{{ event.name2 }}</h3>
            <p class="event-text2">{{ event.text2 }}</p>
        </div>
    </div>
</template>

<script>
import HeadingText from '@/components/heading-text';

export default {
    name: 'ChapmanCares',
    components: {
        HeadingText,
    },
    data() {
        return {
            events: [
                {
                    name1: 'Making Strides Against Cancer',
                    text1:
                        'Thousands of people, young and old, participated in the Making Strides Against Breast Cancer event at Tempe Beach Park. As a sponsorship partner, Chapman Auto brought the Breast Cancer Pace Car, driven by Danica Patrick. Chapman Auto employees participated in the walk, helping to raise thousands of dollars for breast cancer research.',
                },
                {
                    name2: 'Canine Companions For Independence',
                    text2:
                        'Chapman Auto has been a proud supporter of Canine Companions for Independence for more than 10 years. From sponsoring a golf tournament to puppy training, Chapman Auto employees are proud to work with CCI as they help others live happy, independent lives.',
                },
            ],
        };
    },
};
</script>

<style lang="scss" scoped>
.banner-img {
    width: 100%;
}
.canine-img {
    margin-left: 8rem;
    margin-top: 25rem;
    position: absolute;
    left: 7rem;
    max-height: 40%
}
.strides-img {
    margin-left: 8rem;
    margin-top: 20rem;
    position: absolute;
    left: 7rem;
    max-height: 40%;

}
.event-text1 {
    margin-left: 15rem;
    margin-top: 10rem;
    position: absolute;
    left: 20rem;
    padding-right: 15rem;
    line-height: 2.5rem;
   
}
.event-text2 {
    margin-left: 15rem;
    margin-top: 31rem;
    position: absolute;
    left: 20rem;
    padding-right: 15rem;
    line-height: 2.5rem;
    
}
.event-name1 {
    margin-left: 15rem;
    margin-top: 7rem;
    position: absolute;
    left: 20rem;
    
}
.event-name2 {
    margin-left: 15rem;
    margin-top: 28rem;
    position: absolute;
    left: 20rem;
    
}
</style>

