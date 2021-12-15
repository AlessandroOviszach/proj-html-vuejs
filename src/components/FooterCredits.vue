<template>
<div>
    <div class="square">
        <div></div>
    </div>

    <div class="credits-container">
        <div class="container">
            <div class="left-credit">
                &copy; Copiright 2020 tophive. All Rights Reserved.
            </div>

            <div class="right-credit">
                <ul>
                    <li class="link">Privacy</li>
                    <li class="link">Terms</li>
                    <li class="link">Coockie Privacy</li>
                    <li class="link">Sitemap</li>
                </ul>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name : 'FooterCredits',
}
</script>

<style scoped lang='scss'>


div {
    .square {
        display: flex;
        justify-content: end;
        align-items: flex-end;
        padding: 1.8rem;
        div {
            padding: 1.3rem;
            background-color: #d5d7da;
        }
    }

    .credits-container {
        background-color: #15222e;
        padding: 1rem;
        font-size: .9rem;
        color: #a0a0a0;
        .container {
            display: flex;
            align-items: center;
            justify-content: space-between;
            .left-credit {
    
            }
            .right-credit {
                ul {
                    display: flex;
                    align-items: center;
                    list-style: none;
                    .link {
                        padding-left: 1rem;
                    }
                }
            }
        }
    }
}

</style>