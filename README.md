# sliderCarusel
пример вызова

div class="underline"></div>
            <div class="companies-wrapper">
                <div class="companies-hor">
                    <div class="companies-hor-item"><img src="images/companies/companies-1.png" alt=""></div>
                    <!--....
                  .....-->
                    <div class="companies-hor-item"><img src="images/companies/companies-7.png" alt=""></div>
                </div>
            </div>
              <!-- <button id="test-left"> < </button>
            <button id="test-right"> > </button>-->
    const carousel = new SliderCarusel({
            main: '.companies-wrapper',
            wrap: '.companies-hor',
            //prev: '#test-left', //клавиши можно передать свои или они создадутся сами
            //next: '#test-right',
            slidesToShow: 4, // количество видимых слайдов
            infinity: true, // прокрутка в круг
            responsive: [{
                breakpoint: 1024,
                slidesToShow: 3
            }, {
                breakpoint: 768,
                slidesToShow: 2
            }, {
                breakpoint: 576,
                slidesToShow: 1
            }, ]
        });

        carousel.init();
