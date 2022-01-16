# 알아두면 유용한 html 태그

## progrss

```html
<progress value="50" ,min="0" max="100"></progress>
```

<progress value="50" min="0" max="100"></progress>

- 자바스크립트로 해야할 것 만 같았던 진행 표시줄을 `progress`태그 한줄로 표시할 수 있음.
- css로 커스텀 가능

## meter

```html
<meter min="0" max="100" low="20" high="80" optimum="15" value="50"></meter>
```

<meter min="0" max="100" low="20" high="50" optimum="15" value="10"></meter>

- 진행표시줄 (`progress`)과는 다르게 값이 높고 낮을때 따라 색상이 바뀌는것
- 활용 예시는 미세먼지 레벨 등을 표현

## details && summary

```html
<details>
    <span></span>    <summary>clickme<summary>
        <span>info</span>
</details>
```

<details>
    <span></span> 
    <summary>clickme</summary>
    <span>info</span>
</details>

## input

```html
<input type="date" /> <input type="month" /> <input type="week" /><input
  type="time"
/>
```

<input type="date" /> <input type="month" /> <input type="week" /><input
  type="time"
/>

## picture

```html
<picture>
  <source srcset="src01.png" media="(min-width:1200px)" />
  <source srcset="src02.png" media="(min-width:900px)" />
  <source srcset="src03.png" media="(min-width:500px)" />
  <img src="src/04.jpg" />
</picture>
```

미디어쿼리 대신에 `picture`태그로 화면에 따라 다른 이미지를 보여줄 수 있다.

## datalist

datalist를 사용하면 자바스크립트 대신에 자동완성을 사용할 수 있다.

```html
<label for="movie">What is your favourite moive?</label>
<input type="text" list="movie-options" />
<datalist id="movie-options">
  <option value="Dune"></option>
  <option value="Dune"></option>
  <option value="Dune"></option>
  <option value="Dune"></option>
  <option value="Dune"></option>
</datalist>
```

<label for="movie">What is your favourite moive?</label>
<input type="text" list="movie-options" />
<datalist id="movie-options">

  <option value="Dune"></option>
  <option value="Dune1"></option>
  <option value="Dune2"></option>
  <option value="Dune3"></option>
  <option value="Dune4"></option>
</datalist>
