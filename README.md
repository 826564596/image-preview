ENGLISH | [简体中文](./REAEME-zh-CN.md) 

# image-preview(The most fluent & The most comfortable)
front end image preview
for mobile-web application.
### features:
1. most of operation is supported by gensture.
2. rotate and zoom image.
### How to use it:
#### install:
* Clone it ,then `npm run build`,find source `ImagePreview-prd.js` in `release/ts`,finally use it in your project.
* Or you can install this project's `release/ts/ImagePreview-prd.js` directily.
* If you are using module-sysetem:
* The `release/image-preview` directory is built for different module-system , include AMD,CommonJS,ES6,UMD. You can choose one adapt to your project.
#### example
[click here](https://daxiazilong.github.io/) . 
#### usage:
html:
```html
  <div class="imageWraper">
    <img data-src="/images/IMG_0512.JPG" src="/images/IMG_0512.JPG">
    <img data-src="/images/main_body3.png" src="/images/main_body3.png">
  </div>
```
javascript:
``` javascript
//just
let imgObj = new ImagePreview({
  selector:`.imageWraper img`
})
//or mvvm project

let imgObj =  new ImagePreview({
  curImg:'imgsrc',
  imgs:[
    'imgsrc',
    'imgsrc',
    'imgsrc'
  ]
})
//then show n-th picture,use
imgObj.show(n);

// distroy instance.  remove HTML generated by this ImagePreview instance
// for better performance, then you can set imgObj = null;
imgObj.distory();

```
### communicate
yon can join qq-group 977121370 and chat with me.
