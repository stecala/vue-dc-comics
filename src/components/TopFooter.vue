<template>
    <div class="footer-container">
        <div class="container-lg">
            <div class="row">
                <div class="col-6 d-flex flex-column flex-wrap py-5 myheight">
                    <div>
                        <h4>DC COMICS</h4>
                        <ul>
                            <li v-for="(element, index) in dcComicsList" :key='index' class="pt-2">
                                <a :href="element.url">{{ element.name }}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h4>SHOP</h4>
                        <ul>
                            <li v-for="(element, index) in shopList" :key='index' class="pt-2">
                                <a :href="element.url">{{ element.name }}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h4>DC</h4>
                        <ul>
                            <li v-for="(element, index) in dcList" :key='index' class="pt-2">
                                <a :href="element.url">{{ element.name }}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h4>SITES</h4>
                        <ul>
                            <li v-for="(element, index) in sitesList" :key='index' class="pt-2">
                                <a :href="element.url">{{ element.name }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col-6 img-bg">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data: function () {
        return {
            dcComicsList: [
                {
                    name: "Character",
                    url: "#",
                },
                {
                    name: "Comics",
                    url: "#",
                },
                {
                    name: "Movies",
                    url: "#",
                },
                {
                    name: "TV",
                    url: "#",
                },
                {
                    name: "Games",
                    url: "#",
                },
                {
                    name: "Videos",
                    url: "#",
                },
                {
                    name: "News",
                    url: "#",
                },
            ],
            shopList: [
                {
                    name: "Shop DC",
                    url: "#",
                },
                {
                    name: "Shop DC Collectibles",
                    url: "#",
                },
            ],
            dcList: [
                {
                    name: "Terms Of Use",
                    url: "#",
                },
                {
                    name: "Privacy policy (New)",
                    url: "#",
                },
                {
                    name: "Ad Choices",
                    url: "#",
                },
                {
                    name: "Advertising",
                    url: "#",
                },
                {
                    name: "Jobs",
                    url: "#",
                },
                {
                    name: "Subscriptions",
                    url: "#",
                },
                {
                    name: "Talent Workshops",
                    url: "#",
                },
                {
                    name: "CPSC Certificates",
                    url: "#",
                },
                {
                    name: "Ratings",
                    url: "#",
                },
                {
                    name: "Shop Help",
                    url: "#",
                },
                {
                    name: "Contact Us",
                    url: "#",
                },
            ],
            sitesList: [
                {
                    name: "DC",
                    url: "#",
                },
                {
                    name: "MAD Magazine",
                    url: "#",
                },
                {
                    name: "DC Kids",
                    url: "#",
                },
                {
                    name: "DC Universe",
                    url: "#",
                },
                {
                    name: "DC Power Visa",
                    url: "#",
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";

.footer-container {
    width: 100%;
    height: 450px;
    background-image: url('../assets/img/footer-bg.jpg');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    color: $textColorPrimary;
}

.img-bg {
    background-image: url('../assets/img/dc-logo-bg.png');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    height: 450px;
}

ul {
    list-style: none;
    padding: 0;

    li {
        font-size: 0.75rem;

        a {
            text-decoration: none;
            color: grey;
        }
    }
}
.myheight{
    height: 450px;
}
</style>