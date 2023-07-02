# Evgeniya Zelenkova

## Contacts
* **Location:** Russia, Nizhny Novgorod
* **Phone:** +7 910 877 42 34
* **Email:** evgeniia.er@gmail.com
* **GitHub:** https://github.com/Aqualiffe

## About Me

## Skills
* HTML5, CSS3
* JavaScript Basics
* Git, GitHub
* VS Code
* Adobe Photoshop

## Code Example
**My first slider**
```javascript

const prev = document.getElementById('btn-prev'),
next = document.getElementById('btn-next'),
slides = document.querySelectorAll('.slide'),
dots = document.querySelectorAll('.dot');

let index = 0;

const activeSlide = n => {
for(slide of slides) {
  slide.classList.remove('active');
}
slides[n].classList.add('active');
}
const activeDot = n => {
for(dot of dots) {
  dot.classList.remove('active');
}
dots[n].classList.add('active');
}

const prepareCurrentSlide = ind => {
activeSlide(index);
activeDot(index);
}

const nextSlide = () => {
if(index == slides.length - 1) {
  index = 0;
  prepareCurrentSlide(index);
}else {
  index++;
  prepareCurrentSlide(index);
}
}

const prevSlide = () => {
if(index == 0) {
  index = slides.length - 1;
  prepareCurrentSlide(index);
}else {
  index--;
  prepareCurrentSlide(index);
}
}

dots.forEach((item, indexDot)=> {
item.addEventListener('click', () => {
  index = indexDot;
  prepareCurrentSlide(index);
})
})
next.addEventListener('click', nextSlide);
prev.addEventListener('click', prevSlide);
const interval = setInterval(nextSlide, 2000);

```

## Experience
* [portfolio fl.ru](https://www.fl.ru/users/alberta/portfolio/)
## Education
* N. I. Lobachevsky State University of Nizhny Novgorod, VMK
* WayUP "Web layout designer: getting started"
* JavaScript Manual on learnjavascript.ru (in progress)
* RS Schools Course «JavaScript/Front-end. Stage 0» (in progress)
## Languages
* English - Intermediate/Upper-intermediate
