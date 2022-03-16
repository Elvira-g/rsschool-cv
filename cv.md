# Elvira Galiakhmedova

## Contacts:

* **Address:** Kolomna, Moscow Area, Russia
* **Phone:** +79261330021
* **E-mail:** elvira_27@mail.ru
* **GitHub:** [Elvira-g](https://github.com/Elvira-g)
* **Telegram:** ellevira

## About
For a large part of my professional life, I have worked in the HR department. At the age of 30, I realized that this is not the direction I want to develop in. So I decided to change my profession. The direction of IT was always interesting for me, but there was no opportunity to get a second higher education. So when various courses for changing specialization appeared, I decided to try myself. Now my main goal is to gain knowledge and start my career in the area that is really interesting to me.

## Skills
* HTML5/CSS3
* jQuery
* JavaScript (Fundamentals)
* React (in process, Skillbox courses)
* PHP, Laravel (Fundamentals)
* Git
* Figma

## Code Examples
**JavaScript**

```const menuBtn = document.querySelector('.hamburger');
const menuBlock = document.querySelector('.menu-block');
const menuItem = document.querySelectorAll('.menu-item-link');

menuItem.forEach((item) => {
        item.addEventListener('click', (e) => {
            e.preventDefault();
            scrollToBlock(item);
            if (screen.width <= 812) {
                if(menuBtn.classList.contains('is-active')){
                    closeMenuBtn(menuBtn);
                } else {
                    openMenuBtn(menuBtn);
                }  
            }
            
        })
    })

    function scrollToBlock(item) {
    const link = item.attributes.href.value;
    sections.forEach((section) => {
        const id = `#${section.id}`;
        if ( link == id ){ 
            if ( link == '#contacts' ) {
                const height = section.offsetTop - 280;
                window.scroll(0, height);
            } else {
               const height = section.offsetTop - 60;
               window.scroll(0, height);
            }
        }
    })
}
```
**PHP**
```<?php
include_once ('models/M_Faq.php');

class C_Faq extends Controller {

    public function action_index () {
        $faq = new M_Faq();
        $result = $faq->showFaq();

        $this->title = 'Часто задаваемые вопросы';
        $this->content = $this->Template('views/v_faq.php', array('faq'=>$result));

    }
}
```

## Experience
* [Commercial project](https://sidelki-zabota.ru/)
* [Task for a vacancy](https://github.com/Elvira-g/ABC_Mobile_test)
* [Study project](https://rolling-scopes-school.github.io/elvira-g-JSFEPRESCHOOL/portfolio/)
* [Study project](https://rolling-scopes-school.github.io/elvira-g-JSFEPRESCHOOL/audiopleer/)


