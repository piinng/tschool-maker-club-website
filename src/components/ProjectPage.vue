<template>
    <div class="w3-content" style="max-width:1400px">
    <!-- Projects Header-->
    <div class="w3-container w3-padding-32" id="projects">
        <h3 class="w3-border-bottom w3-border-light-grey w3-padding-16">Projects</h3>
    </div>

    <!-- Projects content -->
    <div class="w3-content w3-padding" style="max-width:1564px">
        <div class="w3-row-padding" v-for="achievement in achievements" :key="achievement.id">
            <!-- One Project -->
            <div class="w3-col l3 m6 w3-margin-bottom" v-for="index in achievement.content" :key="index.id">
                <div class="w3-display-container">
                    <div class="w3-card-4 w3-margin w3-white">
                        <img :src="index.Image" style="width:100%" height="175px">
                        <div class="w3-container">
                            <h3><b>{{ index.Title }}</b></h3>
                            <h5>{{ index.Author }}, <span class="w3-opacity">{{ index.Date }}</span></h5>
                        </div>
                
                        <div class="w3-container">
                            <p>{{ index.content }}</p>
                            <div class="w3-row">
                                <div class="w3-col m8 s12">
                                    <p><button @click="openLinks(index.ReadMoreLink)" class="w3-button w3-padding-large w3-white w3-border"><b>READ MORE »</b></button></p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        </div>
    </div>
    </template>
    
    <script>
    export default {
    methods: {
            openLinks(link) {
                window.open(link, '_blank');
            }
        },
    data() {
        return {
            achievements: [
                { id: 1, content: [
                    {
                        id: 104,
                        Image: './ProjectsImg/image.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                    {
                        id: 103,
                        Image: './ProjectsImg/103Cover.jpeg',
                        Title: '雙面的早ㄤ',
                        Author: '孫逸平',
                        Date: 'May 30, 2024',
                        content: '不論現在時間，見到人都要說「早安」，這是數位實中的傳統（？',
                        ReadMoreLink: 'https://www.instructables.com/3D-Dual-Letters/',
                    },
                    {
                        id: 102,
                        Image: './ProjectsImg/102Cover.jpeg',
                        Title: '行星齒輪時鐘 DIY',
                        Author: '創客社',
                        Date: 'Mar. 7, 2024',
                        content: '日本大宮北高校學生來到本校進行國際交流，利用數位實中之諧音「時鐘」，帶領日本的高中生 DIY 製作行星齒輪時鐘。',
                        ReadMoreLink: 'https://www.instructables.com/Laser-Cut-DIY-Epicyclic-Gearing/',
                    },
                    {
                        id: 101,
                        Image: './ProjectsImg/101Cover.jpeg',
                        Title: '小夜燈工作坊',
                        Author: '創客社',
                        Date: 'Nov. 29, 2023',
                        content: '與北市大同高中 Robot maker 社團進行交流，透過三個下午的時間，舉辦工作坊製作獨一無二的小夜燈。',
                        ReadMoreLink: '',
                    },
                ]
                },
            ],
        };
    },
    };
    </script>
    
    <style scoped>
    /* 在這裡添加 CSS 樣式 */
    </style>