<template>
<div class="link-container">

    <div class="contact-us">
        <h1>Contact Us</h1>
        <div v-for="(parameter, index) in ContactList" :key="index" class="link">
            <i :class="` ${parameter.icon} `"></i>
            <a href="#"> {{parameter.text}} </a>
        </div>
    </div>


    <div class="support-us">
        <h1>Support Us</h1>
        <div v-for="(parameter, index) in SupportList" :key="index" class="link">
            <i class="fas fa-chevron-right"></i>
            <a href="#"> {{parameter}} </a>
        </div>
    </div>

    <div class="explore">
        <h1>explore</h1>
        <div v-for="(parameter, index) in ExploreList" :key="index" class="link">
            <i class="fas fa-chevron-right"></i>
            <a href="#"> {{parameter}} </a>
        </div>
    </div>

    <div class="visit">
        <h1>visit</h1>
        <div v-for="(parameter, index) in VistList" :key="index" class="link">
            <i class="fas fa-chevron-right"></i>
            <a href="#"> {{parameter}} </a>
        </div>
    </div>

</div>
</template>

<script>
export default {
    name : 'UsefulLinks',
    data() {
        return {
            ContactList : [
                {
                    icon : 'fas fa-map-marker-alt',
                    text : '900 Wood Street, MI New York 48607',
                },
                {
                    icon : 'fas fa-phone-square-alt',
                    text : '+56 345 678 000-09',
                },
                {
                    icon : 'fas fa-envelope',
                    text : 'info@example.com',
                },
            ],
            SupportList : [
                'privacy',
                'terms',
                'Coockie policy',
                'sitemap',
            ],
            ExploreList : [
                'accommodation',
                'arts academics',
                'central services',
                'conferences and events',
                'food and drink',
            ],
            VistList : [
                'admission',
                'contact us',
                'FAQs',
                'request information',
                'privacy notice',
            ],
        }
    }
}
</script>

<style scoped lang='scss'>
.link-container {
    display: flex;
    
    .contact-us,
    .support-us,
    .explore,
    .visit {
        width: 25%;
        .link {
            display: flex;
            align-items: center;
            width: 65%;
            padding-bottom: 1rem;
            i {
                padding-right: .5rem;
            }

            .fa-chevron-right {
                font-size: .7rem;
            }
            a {
                font-size: .9rem;
                text-decoration: none;
            }
        }
    }
}

// general styles
h1 {
    color: #fff;
    font-size: 1.4rem;
    padding-bottom: 2rem;
}

a,
i {
    color: rgb(160, 160, 160);
}
</style>