## Momentum Hompage clone

### [Momentum_BY_SU](https://oiosu.github.io/Motivational-Homepage/)

![image](https://user-images.githubusercontent.com/99783474/201279269-11e27ca3-bd3f-48eb-80c0-72368e2f73f0.png)




> with spartacodingclub

---

### ๐  STACK
> HTML, CSS, JavaScript


### ๐ก ๋ชฉํ 
> 1. HTML, CSS ๊ธฐ์ด ์ง์์ ์ดํดํ๋ค. 
> 2. ์ฝ๋ฉ์ ํ์ฉํ, ๋๋ง์ ๋๊ธฐ๋ถ์ฌ ํ๋ก๊ทธ๋จ์ ์ ์ํ  ์ ์๋ค. 

    Momentum ๊ตฌ๊ธ ํฌ๋กฌ ๋ธ๋ผ์ฐ์ ์์ ์ถ๊ฐ๋ก ์ ์ฉํ  ์ ์๋ ๊ธฐ๋ฅ ์ค ํ๋๋ก 
    ๋ฐฐ๊ฒฝํ๋ฉด ๊พธ๋ฏธ๊ธฐ, ์ค์๊ฐ ์๊ฐํ์, ์ค๋์ ํ ์ผ, ๋ช์ธ์ ๋ณผ ์ ์๋ ๊ธฐ๋ฅ์ ์ ๊ณตํฉ๋๋ค. 
    
##### ๊ธฐ๋ฅ :  ๋๋ง์ ๋ฐฐ๊ฒฝํ๋ฉด ๊พธ๋ฏธ๊ธฐ, ์ค์๊ฐ ์๊ฐ ๊ธฐ๋ฅ, ๋๋ง์ ๋๊ธฐ๋ถ์ฌ ๋ฉ์์ง ๊ธฐ๋ฅ, ๋๋ค ๋ช์ธ ๋ณด์ฌ์ฃผ๊ธฐ ๊ธฐ๋ฅ


---

### ๐ก HTML ๊ธฐ์ด 
> * HTML ์์ ๋ง๋ค๊ธฐ 
1. ์ธ์ฌ๋ง ๋ฃ๊ธฐ 
``` html
 <div class="main">
        <div class="greeting">Hello, Migdracios!</div>
    </div>
```

2. ์๊ฐ, ํ  ์ผ ๊ตฌ์ญ ๋ง๋ค๊ธฐ 
```html 
 <div class="main">
        <div class="greeting">Hello, Migdracios!</div>
				<div class="todo"></div>
    </div>
```

3. ์๊ฐ ๋ฃ๊ธฐ 
```html
<div class="todo">
	<div class="time">12:25</div>
</div>
```

4. ์ด์ฃผ์ ๋ชฉํ ๋ฃ๊ธฐ 
```html
  <div class="main">
				<div class="time">12:25</div>
        <div class="greeting">Hello, Migdracios!</div>
				<div class="todo"></div>
		</div>
```

5. ๋ช์ธ ๋ฃ๊ธฐ 
```html 
<div class="quote">
	<div class="author">- ๋ช์ธ ์ ์ - </div>
	<div class="content">" ์ฌ๊ธฐ๋ ๋ช์ธ ๋ด์ฉ์ด ๋ค์ด๊ฐ๋๋ค! " </div>
</div>
```

---


### ๐ก CSS ๊ธฐ์ด 

1. ๋ฐฐ๊ฒฝ ์ด๋ฏธ์ง ์ฝ์๊ณผ ์๊น ๋ฃ๊ธฐ  
```css
        body{
            background-image: url("https://mir-s3-cdn-cf.behance.net/project_modules/1400/e6f371148022401.62cdd9fb8ba9d.jpg");
            /* ๋ฐฐ๊ฒฝ์ด๋ฏธ์ง ๊ณฝ ์ฑ์ฐ๊ธฐ */
            background-size: cover;
            background-position: center;
            /* background-position: center; 
            ๋ผ๊ณ  ํ  ๊ฒฝ์ฐ ์ด๋ฏธ์ง ๊นจ์ง๋ ํ์๊ณผ ๋ฐ๋ณต๋จ์ ํ์ธ */
            /* ๋ฐ๋ผ์   background-size: cover; ๋ผ๋ ์ฝ๋๋ฅผ ์์ฑํ๊ณ  ์์๊ฐ์ ์ด์ ํด๊ฒฐํจ*/
            color: #fff;
            /* font์ ์ง์ ์ ์ธ ์คํ์ผ๋ง์ ํ์ง์์๋, body ๋ถ๋ถ์ ์ ์ฒด์ ์ผ๋ก font ์๊น์ ์ง์ ํด ์ค ์ ์๋ค. */
        }
```

2. ํฐํธ ์คํ์ผ 
```css
 .time {
            font-size: 80px;
        }
        .greeting{
            font-size: 50px;
        }
        .todo {
            font-size: 30px;
        }
        .author {
            font-size: 25px;
            font-style: italic;
        }
```

3. vw, vh??
```css
.quote {
	width: 80vw;
	height: 20vh;
}
```
> px(ํฝ์) ๊ฐ์ ๊ณ ์ , vw(ํ๋ฉด๋น๊ฐ๋ก), vh(ํ๋ฉด๋น์ธ๋ก)๋ก ์ค์ ํ๋ฉด ํ๋ฉด ๋น์จ์ด ๋ฌ๋ผ๋ ๋น์จ๋ก ๊ธธ์ด๊ฐ ๋ง์ถฐ์ง๋ค. 


4. ํ๋ฉด ๊ฐ์ด๋ฐ ์ ๋ ฌ
>  width: 100vw, height: 28vw์ ํ์ ๊ฒฝ์ฐ, ์คํฌ๋กค ์ ๊ณต๊ฐ์ด ์๊ธฐ๋ ์ด์๊ฐ ๋ฐ์ํ์๋ค. ๋ฐ๋ผ์ ๋ ์ฝ๋๋ฅผ ์ฃผ์ ์ฒ๋ฆฌ ํ ํ์ธํ ๊ฒฐ๊ณผ, 
ํ ํ๋ฉด์ ์ํ๋ ๊ตฌํ๋ ๋ชจ์ต์ ํ์ธ ํ  ์ ์์๋ค. 

```css
        .main {
            width: 100vw;
            height: 80vh;

            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }

        .quote {
            /* width: 100vw;
            height: 28vw; */

            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }
```

---


### ๐ก Javasctipt
3. ์๊ฐ, ๋ช์ธ api ์ฝ๋ 
```Javasctipt
$(document).ready(function () {
            renderCurrentTime();
            renderQuote();
        });


function renderCurrentTime() {
    let url = `https://worldtimeapi.org/api/timezone/Asia/Seoul`;
    fetch(url)
        .then(res => res.json()).then((data) => {
            let datetime = data['datetime'].substr(11,5);
            $('#time').text(datetime);
        });
}


        function renderQuote() {
            let url = `https://api.quotable.io/random`;
            fetch(url)
                .then(res => res.json()).then((data) => {
                    let content = `" ${data['content']} "`;
                    let author = `- ${data['author']} -`;
                    $('#content').text(content);
                    $('#author').text(author);
                });
        }
```

---


