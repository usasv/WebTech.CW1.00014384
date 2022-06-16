$(document).ready(function () {
    var $link = $('.menu-top a')

        $link.click(function (e) {
            e.preventDefault();
            $link.removeClass('active')
            var id = $(this).addClass('active').attr('href');
            var target= $(id).offset().top -76;
            console.log(target);
            $('html, body').animate({
                scrollTop: target
            }, 1000)
        })
        var link2 = $('.contact a');
        link2.click(function (e) {
            e.preventDefault();
            $('html, body').animate({
                scrollTop: $('#home').offset().top -76
            }, 1000)
        })
    $(window).scroll(function () {
        var menu = $('.menu-top');
        if (window.pageYOffset >= 76) {
            menu.css('position', 'fixed')
        }
        var scroll = $(this).scrollTop();
        console.log($(this).scrollTop());
        $link.each(function () {
            var attr = $(this).attr('href');
            var selector = $(attr).offset().top -76;
            
            if(scroll >= selector){
                $link.removeClass('active');
                $(this).addClass('active')
            }
        })
    })
});








