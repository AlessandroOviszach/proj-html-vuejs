<template>
    <div class="form-container">
        <div class="content">
            <div class="rectangle"></div>
            <div class="input-container">
                <input type="text" placeholder="Subscribe to our newsletter">
                <button>Register</button>
            </div>
            <div class="text-container">
                <p>
                    <span>Insights is Picwik</span>
                    Univerity'&apos;s thought leadership publication for sharing knowledge on management, technology and innovation.
                </p>
                <div class="cta">
                    <a href="#">Take me there</a>
                    <i class="fas fa-chevron-right"></i>
                </div>
            </div>

        </div>
    </div>
</template>

<script>
export default {
    name : 'NewsLetterForm',

}
</script>

<style scoped lang='scss'>
.form-container {
    padding: 4rem 0;
    .content {
        display: flex;
        align-items: center;
        padding: 3rem 5rem 3rem 0;
        box-shadow: 10px 10px 30px #11161d;
        border-radius: .4rem;
        .rectangle {
            background-color: #23374b;
            width: .7rem;
            height: 6rem;
        }
        .input-container {
            display: flex;
            align-items: center;
            padding-left: 2rem;
            padding-right: 4rem;
            input {
                width: 20rem;
                border-style: none;
                background-color: #fff;
                padding: 1.5rem;
            }
            button {
                color: #fff;
                background-color: #d74d52;
                border-style: none;
                padding: 1.5rem 2.5rem;
            }
        }
        .text-container {
            color: rgb(160, 160, 160);
            p {
                font-size: .9rem;
                span {
                    text-decoration: underline #fff;
                    font-weight: bold;
                    line-height: 1.6rem;
                    color: #d74d52;
                }
            }
            .cta {
                display: flex;
                align-items: center;
                padding-top: .5rem;
                a {
                    padding-right: .5rem;
                    font-weight: bold;
                    text-decoration: none;
                    color: #fff;

                }
            }
        }
    }
    
}

</style>