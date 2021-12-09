<template>
    <section class="homepage">
        <div class="container d-flex justify-content-between pt-3">
            <div class="logoBrand">
                <img src="../assets/dark-logo.png" alt="logo">
            </div>
            <div class="flex-grow-1">
                <ul class="listnavigation d-flex">
                    <li  
                        class="d-flex list" 
                        v-for="(item, index) in navigationHeader" 
                        :key="`item-${index}`">
                            <p>{{ item.text }}</p>
                            <i class="fas fa-chevron-down"></i>
                    </li>
                </ul>
            </div>
            <div>
                <ul class="listsocials">
                    <li class="social">
                        <i class="fab fa-twitter"></i>
                    </li>
                    <li class="social">
                        <i class="fab fa-facebook-f"></i>
                    </li>
                    <li class="social">
                        <i class="fab fa-instagram"></i>
                    </li>
                    <li class="social">
                        <i class="fab fa-linkedin"></i>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Sec2Header',
    data() {
        return {
            navigationHeader: [
                {
                    text: 'Home',
                    url: '#',
                },
                {
                    text: 'Pages',
                    url: '#',
                },
                {
                    text: 'Courses',
                    url: '#',
                },
                {
                    text: 'Features',
                    url: '#',
                },
                {
                    text: 'Blog',
                    url: '#',
                },
                {
                    text: 'Shop',
                    url: '#',
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
.homepage {
    width: 100vw;
    background-color: yellow;
    color: gray;
    .logoBrand {
        img {
            width: 50%;
        }
    }
    .listnavigation {
        list-style: none;
        cursor: pointer;
        li {
            align-items: baseline;
            padding-right: 2rem;
            i {
                font-size: 10px;
                padding: 0 5px;
            }
        }
    }
    .listsocials {
        cursor: pointer;
        display: flex;
        list-style: none;
        .social {
            padding-right: 2rem;
        }
    }
}
</style>