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
                        <img :src="index.Image" style="width:100%">
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
                        id: 101,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                    {
                        id: 102,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                    {
                        id: 103,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                    {
                        id: 104,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                ]
                },
                { id: 2, content: [
                    {
                        id: 201,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                    {
                        id: 202,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                    {
                        id: 203,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                    {
                        id: 204,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                ]
                },
                { id: 3, content: [
                    {
                        id: 301,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                    {
                        id: 302,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                    {
                        id: 303,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                    {
                        id: 304,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                ]
                },
                { id: 4, content: [
                    {
                        id: 401,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                    {
                        id: 402,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                    {
                        id: 403,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
                    },
                    {
                        id: 404,
                        Image: '../ProjectsImg/images.jpeg',
                        Title: '這是標題',
                        Author: 'Author',
                        Date: 'April 7, 2014',
                        content: '這是內文',
                        ReadMoreLink: 'https://www.google.com',
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