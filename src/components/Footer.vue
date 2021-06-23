<template>
  <footer>
      <div class="container-60">
        <div class="summary">
             <div v-for="(item, index) in summary" :key="index" class="cols">
                <h5>{{item.title}}</h5>
                <ul>
                    <li v-for="(itemSub,index) in item.subtitle" :key="index"><a href="">{{itemSub}}</a></li>
                </ul>
            </div>
        </div>
        <div class="social">
            <ul>
                <li v-for="(contact, index) in contacts" :key="index"><i :class="`${contact.iconClass}`"></i></li>
            </ul>
        </div>
      </div>
  </footer>
</template>

<script>
export default {
    name: 'Footer',
    data: function () {
        return {
            summary: [
                {
                    title: "Address",
                    subtitle: ["382 NE 191st St# 87394 Miami, FL 33179-3899", "+1(305)547-9909 (9am - 5pm EST, Monday - Friday)", "support@maxcoach.com"]
                },
                {
                    title: "Explore",
                    subtitle: ["Start here", "Blog", "About us"]
                },
                {
                    title: "",
                    subtitle: ["Success Story", "Courses", "Contact us"]
                },
                {
                    title: "Information",
                    subtitle: ["Membership", "Purchase guide", "Privacy policy", "Terms of service"]
                }
            ],
            contacts: [
                {
                    name: "facebook",
                    iconClass: 'fab fa-facebook-square'
                },
                {
                    name: "twitter",
                    iconClass: 'fab fa-twitter'
                },
                {
                    name: "instagram",
                    iconClass: 'fab fa-instagram'
                },
                {
                    name: "linkedin",
                    iconClass: 'fab fa-linkedin'
                }
                
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/mixins.scss';

footer {
    background-color: $darkBlue;

    h5 {
        color: $white;
        font-weight: 600;
        font-size: $h5;
    }

    .container-60 {
        padding: 60px 0px;

        .summary {
        @include flex;

            & div:nth-child(1) {
                width: 55%;
            }
        }


        .social {
            width: 55%;
            margin-top: -20px;

           & ul {
                @include flex-vertical-only;

                & li {
                    margin-right: 24px;
                    font-size: $h5;
                }
            }
        }

        ul {
            @include ul-clean;
            height: 80px;

            li, a {
                @include link-clean;
                color: $silver;
                padding: 5px 0;
                font-size: $smallText;
            }

        }
    }
}

</style>
