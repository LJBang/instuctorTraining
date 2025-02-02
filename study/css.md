## CSS
`css` 도입  

`css` 선언
  - external 
  - internal 
  - inline    

`css` 선택자
  - `tag`
  - `*`
  - `id`
  - `class`
  - `parent > child`
```css
/* CSS comment */
/* 1.tag name */
header {
  color: red;
  font-size: 20px;
}
/* 2. select all */
* {
  margin: 0;
  padding: 0;
}
/* 3. id selector */
#foot {
  background-color: black;
  color: white;
}
/* 4. class selector */
.art {
  font-size: 30px;
  color: green;
}
/* 5. parent child */
ol > li {
  color: yellow;
}
p > b {
  color: gray;
}
```


`css` 우선순위
  1. `!important`
  2. `css inline` 선언
  3. `id`
  4. `class`
  5. `tag`
  6. `parent`에 의해 상속
  
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
  <style>
    /* CSS의 우선순위를 파악하자*/
    /* 6.상위 객체에 의해 상속된 속성 */
    div {
      color: red;
    }
    /* 5.태그 이름으로 지정한 속성 */
    h1{
      color: blue;
    }
    /* 4.클래스 이름으로 지정한 속성 */
    .hello{
      color: brown;
    }
    /* 3. id로 지정한 속성 */
    #mulcam{
      color: yellow;
    }
    /* 2. HTML에서 style을 직접 지정한 속성 */
    /* 1. 속성값 위에 !important를 붙인 속성 */
    h1{
      color: black !important;
    }
  </style>
</head>
<body>
  <div>
    <h1 id="mulcam" class="hello" style="color: green;">Hello, Multicampus!</h1>
  </div>
</body>
</html>
```
`font`
  - `font-size`
  - `font-style`
  - `font-weight`
  - `font-family`

`google font`

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
  <link href="https://fonts.googleapis.com/css?family=Nanum+Myeongjo|Ubuntu&display=swap" rel="stylesheet">
  <style>
    .font{
      font-size: 40px;
      font-style: italic;
      font-weight: 400;
      /* font-family: 'Times New Roman', Times, serif; */
      font-family: 'Ubuntu', 'Nanum Myeongjo', serif;
    }
  </style>
</head>
<body>
  <p class="font">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorum incidunt excepturi vel velit explicabo illo. Perferendis dolor animi consequuntur dolorem culpa est non corrupti libero quibusdam eveniet magni rem, odio nesciunt consectetur, repellendus at eius expedita ad aliquam quo amet molestiae? Deserunt veritatis voluptatibus, ut dolore soluta natus porro nulla similique assumenda numquam exercitationem ratione unde accusamus quis corporis quos. Possimus, at libero! Harum molestias magni cum nam itaque magnam quibusdam dolorem! Assumenda, voluptatem non blanditiis inventore error cupiditate expedita modi quidem tempora officia aut dicta accusamus, nihil, vero vel. Nesciunt dignissimos similique odio quidem quibusdam hic reiciendis, totam quis!</p>
  <p class="font">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Earum dignissimos illum pariatur repudiandae assumenda tempore facilis necessitatibus, perspiciatis minus beatae non ipsa nesciunt suscipit id, molestiae iste neque deleniti ex excepturi ipsam officiis sunt? Fugit, debitis animi numquam placeat sint harum, quidem sequi ad obcaecati quis maiores voluptatem alias temporibus.</p>
</body>
</html>
```

`Bootstrap` 도입
      
