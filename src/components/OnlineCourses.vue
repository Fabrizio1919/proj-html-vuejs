<script>

export default {
    name: 'OnlineCourses',
    data() {
        return {
            activeIndex: 0,
            images: [
                {
                    image: '/src/assets/img/course-02-480x298.jpg',
                    title: 'Learning to Write as a Professional Author',
                    text: 'The purpose of this course is to provide the advanced writing techniques commonly used for inspiring readers and get your work published. Enroll soon to get the best offer for course fee discount.',
                }, {
                    image: '/src/assets/img/stock-full-hd-03-480x298.jpg',
                    title: 'Strategie info-tech incentrate sul cliente',
                    text: 'Now more than ever, corporations are investing heavily in IT. The quality of these investments affects the daily work of millions.',
                }, {
                    image: '/src/assets/img/stock-full-hd-04-480x298.jpg',
                    title:  'Open Programming Courses for Everyone: Python',
                    text: 'The objective of this course is to teach everyone the basics of programming computers using Python. We cover the basics of how one constructs a program from a series of simple instructions in Python.',
                }, {
                    image: '/src/assets/img/stock-full-hd-06-480x298.jpg',
                    title: 'Stray',
                    text: 'Lost, injured and alone, a stray cat must untangle an ancient mystery to escape a long-forgotten city',
                }, {
                    image: '/src/assets/img/stock-full-hd-11-670x450.jpg',
                    title: "Learning to Write as a Professional Author",
                    text: 'The purpose of this course is to provide the advanced writing techniques commonly used for inspiring readers and get your work published. Enroll soon to get the best offer for course fee discount.',
                },
                {
                    image: '/src/assets/img/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg',
                    title: "Strategie info-tech incentrate sul cliente",
                    text: 'Lost, injured and alone, a stray cat must untangle an ancient mystery to escape a long-forgotten city',
                },
                {
                    image: '/src/assets/img/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg',
                    title: "Open Programming Courses for Everyone: Python",
                    text: 'Lost, injured and alone, a stray cat must untangle an ancient mystery to escape a long-forgotten city',
                },
                {
                    image: '/src/assets/img/stock-full-hd-03-480x298.jpg',
                    title: 'Strategie info-tech incentrate sul cliente',
                    text: 'Now more than ever, corporations are investing heavily in IT. The quality of these investments affects the daily work of millions.',
                }, {
                    image: '/src/assets/img/stock-full-hd-04-480x298.jpg',
                    title:  'Open Programming Courses for Everyone: Python',
                    text: 'The objective of this course is to teach everyone the basics of programming computers using Python. We cover the basics of how one constructs a program from a series of simple instructions in Python.',
                }, 
                {
                    image: '/src/assets/img/course-02-480x298.jpg',
                    title: 'Learning to Write as a Professional Author',
                    text: 'The purpose of this course is to provide the advanced writing techniques commonly used for inspiring readers and get your work published. Enroll soon to get the best offer for course fee discount.',
                }, {
                    image: '/src/assets/img/stock-full-hd-03-480x298.jpg',
                    title: 'Strategie info-tech incentrate sul cliente',
                    text: 'Now more than ever, corporations are investing heavily in IT. The quality of these investments affects the daily work of millions.',
                }, {
                    image: '/src/assets/img/stock-full-hd-04-480x298.jpg',
                    title:  'Open Programming Courses for Everyone: Python',
                    text: 'The objective of this course is to teach everyone the basics of programming computers using Python. We cover the basics of how one constructs a program from a series of simple instructions in Python.',
                }, {
                    image: '/src/assets/img/stock-full-hd-06-480x298.jpg',
                    title: 'Stray',
                    text: 'Lost, injured and alone, a stray cat must untangle an ancient mystery to escape a long-forgotten city',
                }, {
                    image: '/src/assets/img/stock-full-hd-11-670x450.jpg',
                    title: "Learning to Write as a Professional Author",
                    text: 'The purpose of this course is to provide the advanced writing techniques commonly used for inspiring readers and get your work published. Enroll soon to get the best offer for course fee discount.',
                },
                {
                    image: '/src/assets/img/artist-blog-03-480x325.jpeg',
                    title: "Strategie info-tech incentrate sul cliente",
                    text: 'Lost, injured and alone, a stray cat must untangle an ancient mystery to escape a long-forgotten city',
                },
                {
                    image: '/src/assets/img/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg',
                    title: "Open Programming Courses for Everyone: Python",
                    text: 'Lost, injured and alone, a stray cat must untangle an ancient mystery to escape a long-forgotten city',
                },
                {
                    image: '/src/assets/img/artist-blog-01-480x325.jpg',
                    title: 'Strategie info-tech incentrate sul cliente',
                    text: 'Now more than ever, corporations are investing heavily in IT. The quality of these investments affects the daily work of millions.',
                }, {
                    image: '/src/assets/img/artist-blog-02-480x325.jpg',
                    title:  'Open Programming Courses for Everyone: Python',
                    text: 'The objective of this course is to teach everyone the basics of programming computers using Python. We cover the basics of how one constructs a program from a series of simple instructions in Python.',
                }, 

            ]

        }  
    },
    methods: {
        changeImages(number) {
            console.log(number);
            if (number + 3 >= this.images.length) {
                console.log("Here");
                this.activeIndex = this.images.length - 3;
            } else {
                this.activeIndex = number;
                console.log("Normal");
            }
        }
}
}
</script>


<template>
    <div class="titleOn text-center py-5">
        <h6>JOIN MAXCOACH AT BEST</h6>
        <h1>Latest Online <strong class="coulture">Courses</strong></h1>
    </div>
    <div class="carosel">
        <div class="container">
            <div class="row ">
                <div class="col-3" v-for="n in 3">
                    <img class="img-fluid rounded" :src="images[(n - 1) + activeIndex].image" alt="">
                    <div class="card-body">
                        <h5 class="card-title coulture">{{ images[(n - 1) + activeIndex].title }}</h5>
                        <p class="card-text"><strong>{{ images[(n - 1) + activeIndex].text }}</strong></p>
                        <div class="item">
                            <svg xmlns="http://www.w3.org/2000/svg"
                                viewBox="0 0 384 512"><!--! Font Awesome Pro 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. -->
                                <path
                                    d="M64 464c-8.8 0-16-7.2-16-16V64c0-8.8 7.2-16 16-16H224v80c0 17.7 14.3 32 32 32h80V448c0 8.8-7.2 16-16 16H64zM64 0C28.7 0 0 28.7 0 64V448c0 35.3 28.7 64 64 64H320c35.3 0 64-28.7 64-64V154.5c0-17-6.7-33.3-18.7-45.3L274.7 18.7C262.7 6.7 246.5 0 229.5 0H64zm56 256c-13.3 0-24 10.7-24 24s10.7 24 24 24H264c13.3 0 24-10.7 24-24s-10.7-24-24-24H120zm0 96c-13.3 0-24 10.7-24 24s10.7 24 24 24H264c13.3 0 24-10.7 24-24s-10.7-24-24-24H120z" />
                            </svg>
                            <span>20 Lessons</span>
                            <svg xmlns="http://www.w3.org/2000/svg"
                                viewBox="0 0 512 512"><!--! Font Awesome Pro 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. -->
                                <path
                                    d="M406.5 399.6C387.4 352.9 341.5 320 288 320H224c-53.5 0-99.4 32.9-118.5 79.6C69.9 362.2 48 311.7 48 256C48 141.1 141.1 48 256 48s208 93.1 208 208c0 55.7-21.9 106.2-57.5 143.6zm-40.1 32.7C334.4 452.4 296.6 464 256 464s-78.4-11.6-110.5-31.7c7.3-36.7 39.7-64.3 78.5-64.3h64c38.8 0 71.2 27.6 78.5 64.3zM256 512A256 256 0 1 0 256 0a256 256 0 1 0 0 512zm0-272a40 40 0 1 1 0-80 40 40 0 1 1 0 80zm-88-40a88 88 0 1 0 176 0 88 88 0 1 0 -176 0z" />
                            </svg>
                            <span>20 Student</span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="selectionCard py-3">
                <div class="text-center">
                    <button class="dot" @click="changeImages(0)"></button>
                    <button class="dot" @click="changeImages(3)"></button>
                    <button class="dot" @click="changeImages(6)"></button>
                    <button class="dot" @click="changeImages(9)"></button>
                    <button class="dot" @click="changeImages(12)"></button>
                </div>
            </div>
            <div class="descrition text-center py-3">
                <p>Contro your personal preference settings get notified about <br> appropriate coursers. <strong> View all
                        coursers &#129046;</strong>
                </p>
            </div>
        </div>
    </div>
</template>


<style></style>