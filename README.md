## Momentum Hompage clone

### [Momentum_BY_SU](https://oiosu.github.io/Motivational-Homepage/)

![image](https://user-images.githubusercontent.com/99783474/201279269-11e27ca3-bd3f-48eb-80c0-72368e2f73f0.png)




> with spartacodingclub

---

### 🛠 STACK
> HTML, CSS, JavaScript


### 💡 목표 
> 1. HTML, CSS 기초 지식을 이해한다. 
> 2. 코딩을 활용한, 나만의 동기부여 프로그램을 제작할 수 있다. 

    Momentum 구글 크롬 브라우저에서 추가로 적용할 수 있는 기능 중 하나로 
    배경화면 꾸미기, 실시간 시간표시, 오늘의 할일, 명언을 볼 수 있는 기능을 제공합니다. 
    
##### 기능 :  나만의 배경화면 꾸미기, 실시간 시간 기능, 나만의 동기부여 메시지 기능, 랜덤 명언 보여주기 기능


---

### 💡 HTML 기초 
> * HTML 요소 만들기 
1. 인사말 넣기 
``` html
 <div class="main">
        <div class="greeting">Hello, Migdracios!</div>
    </div>
```

2. 시간, 할 일 구역 만들기 
```html 
 <div class="main">
        <div class="greeting">Hello, Migdracios!</div>
				<div class="todo"></div>
    </div>
```

3. 시간 넣기 
```html
<div class="todo">
	<div class="time">12:25</div>
</div>
```

4. 이주의 목표 넣기 
```html
  <div class="main">
				<div class="time">12:25</div>
        <div class="greeting">Hello, Migdracios!</div>
				<div class="todo"></div>
		</div>
```

5. 명언 넣기 
```html 
<div class="quote">
	<div class="author">- 명언 저자 - </div>
	<div class="content">" 여기는 명언 내용이 들어갑니다! " </div>
</div>
```

---


### 💡 CSS 기초 

1. 배경 이미지 삽입과 색깔 넣기  
```css
        body{
            background-image: url("https://mir-s3-cdn-cf.behance.net/project_modules/1400/e6f371148022401.62cdd9fb8ba9d.jpg");
            /* 배경이미지 곽 채우기 */
            background-size: cover;
            background-position: center;
            /* background-position: center; 
            라고 할 경우 이미지 깨지는 현상과 반복됨을 확인 */
            /* 따라서   background-size: cover; 라는 코드를 작성하고 위와같은 이슈 해결함*/
            color: #fff;
            /* font에 직접적인 스타일링을 하지않아도, body 부분에 전체적으로 font 색깔을 지정해 줄 수 있다. */
        }
```

2. 폰트 스타일 
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
> px(픽셀) 값은 고정, vw(화면비가로), vh(화면비세로)로 설정하면 화면 비율이 달라도 비율로 길이가 맞춰진다. 


4. 화면 가운데 정렬
>  width: 100vw, height: 28vw을 했을 경우, 스크롤 시 공간이 생기는 이슈가 발생하였다. 따라서 두 코드를 주석 처리 후 확인한 결과, 
한 화면에 원하는 구현된 모습을 확인 할 수 있었다. 

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


### 💡 Javasctipt
3. 시간, 명언 api 코드 
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


