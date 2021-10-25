# Frontend Mentor - Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [Continued development](#continued-development)
- [Author](#author)


## Overview

### The challenge

Users should be able to:

- Check how the mediaqueries work on different screen sizes
- Check how 3 backgrounds at the same time in one container

### Screenshot

#### Mobile design

<img src="https://i.imgur.com/0zuIEum.png" width="400px" ></a>

#### Desktop design

<img src="https://i.imgur.com/5am0kJp.png" width="600px" ></a>



### Links

- Solution URL: (https://www.frontendmentor.io/solutions/responsive-component-3columncard-using-html-and-sass-H03GkZRJ6)
- Live Site URL: (https://bryanclouddev.github.io/ProfileCardComponent/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- SASS preprocessor

### What I learned

I learned on how to colocate 3 backgrounds, including 2 images and one color background in one container at the time, I was surprising for me since I knew I could use one at the time only per container.

```css
.main {
  transition: ease 3s;
  background-color: #19a2ae;
  background-image: url("../images/bg-pattern-top.svg"), url("../images/bg-pattern-bottom.svg");
  background-size: 637.5px, 637.5px;
  background-repeat: no-repeat;
  background-position: top -358px left -423px, bottom -358px right -403px; }
```
In here we can see the order that the backgrounds use in this case, if we use multiple they have to be seprated with a comma, then we have to make sure the order of the images we use, they will appear as in layers, the very first image will show up above the second image and the second one above the third image and so on.

A really good challenge also was the fact of havnig this rounded profile picture with that white border and having it above the background image of the cover photo. I was able to solve it with a negative margin-top:

```css
.main .container .card .box .profile-photo {
          margin-top: -6.3rem;
          width: 11rem; }
```

Really good challenge, I learned a lot!
### Continued development

I will definetely continue learning on how to make better responsive backgrounds without using so many meadiaqueries, I know there has to be a better way to do it and also focusing on how to better structure a page and naming classes.

## Acknowledgments
I want to thank to the Youtube channel of [The Net Ninja](https://www.youtube.com/channel/UCW5YeuERMmlnqo4oq8vwUpg) since I was able to find out in [this video](https://www.youtube.com/watch?v=Sj7Hs94uZjE) how to use multiple backgrounds in CSS for one container.

## Author

- Website - [bryancloud.dev](https://bryancloud.dev)
- Frontend Mentor - [@bryan-cloud](https://www.frontendmentor.io/profile/BryanCloudDev)
- Twitter - [@BryanCloudDev](https://twitter.com/BryanCloudDev)
