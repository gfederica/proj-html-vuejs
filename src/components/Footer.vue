<template>
  <footer>
      <div class="container-70">
        <div v-for="(item, index) in summary" :key="index">
            <h3>{{item.title}}</h3>
            <ul>
                <li v-for="(itemSub,index) in item.subtitle" :key="index"><a href="">{{itemSub}}</a></li>
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
                subtitle: ["Start here", "Blog", "About us", "Success Story", "Courses", "Contact us"]
                },
                {
                title: "Information",
                subtitle: ["Membership", "Purchase guide", "Privacy policy", "Terms of service"]
                }
            ],
            contacts: [
                {
                    name: "facebook",
                    iconClass: '<i class="fab fa-facebook-square"></i>'
                },
                {
                    name: "twitter",
                    iconClass: '<i class="fab fa-twitter"></i>'
                },
                {
                    name: "instagram",
                    iconClass: '<i class="fab fa-instagram"></i>'
                },
                {
                    name: "linkedin",
                    iconClass: '<i class="fab fa-linkedin"></i>'
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

    h3 {
        color: $white;
        font-weight: 600;
    }

    .container-70 {
    @include container-70;
    @include flex;
    padding: 100px 0px;
    margin: auto;


    ul {
        @include ul-clean;

        li, a {
            color: $white;
            text-decoration: none;
        }

    }

    }
}

</style>
