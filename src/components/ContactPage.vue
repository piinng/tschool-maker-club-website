<template>
    <div class="w3-content" style="max-width:1400px">
    <!-- Contect Header-->
    <div class="w3-container w3-padding-32" id="contact">
        <h3 class="w3-border-bottom w3-border-light-grey w3-padding-16">Contact</h3>
        <div class="w3-col m4 w3-container">
            <img :src="Image" class="w3-image w3-round" style="width:100%">
        </div>
        <div class="w3-col m8 w3-panel">
        <div class="w3-large w3-margin-bottom">
            <i class="fa fa-map-marker fa-fw w3-hover-text-black w3-xlarge w3-margin-right"></i><a href="https://maps.app.goo.gl/g68JeVwu2eZdDETy8" target="_blank" style="text-decoration:none;">104台北市中山區吉林路110號5樓(吉林學習基地)</a><br>
            <i class="fa fa-instagram fa-fw w3-hover-text-black w3-xlarge w3-margin-right"></i><a href="https://www.instagram.com/tschool_maker" target="_blank" style="text-decoration:none;">tschool_maker</a><br>
            <i class="fa fa-envelope fa-fw w3-hover-text-black w3-xlarge w3-margin-right"></i><a href="mailto:maker@tschool.tp.edu.tw" style="text-decoration:none;">maker@tschool.tp.edu.tw</a><br>
        </div>
        </div>
        
    </div>

    
    </div>
    </template>
    
    <script>
    export default {
    data() {
        return {
            Image: "./ContactImg/MakerClubLogo.png"
        };
    },
    };
    </script>
    
    <style scoped>
        @import url(https://www.w3schools.com/w3css/4/w3.css);
        @import url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css);
    </style>