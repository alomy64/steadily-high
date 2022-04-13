# 日期格式化 YYYY-MM-DD HH-MM-SS

# 日期

### 不补零 `/` => 2020/5/20

```js
const currentTime = new Date().toLocaleDateString();   
```

### 补零 `/` => 2020/05/20

```js
const currentTime = new Date()
  .toLocaleDateString()
  .split("/")
  .map((item) => {
    return (item = item <= 9 ? `0${item}` : item);
  })
  .join("/");
```

### 不补零 `-` => 2020-5-20

```js
const currentTime = new Date().toLocaleDateString().replace(/\//g, '-');
```

### 补零 `-` => 2020-05-20

```js
const currentTime = new Date()
  .toLocaleDateString()
  .replace(/\//g, "-")
  .split("-")
  .map((item) => {
    return (item = item <= 9 ? `0${item}` : item);
  })
  .join("-");
```

## 时间

### Hour12 => 下午5:20

```js
let timer = new Date().toLocaleTimeString();
const currentTime = timer.substring(0, timer.lastIndexOf(':'));
```

### Hour24 => 17:20

```js
let timer = new Date().toLocaleString('chinese', { hour12: false });
const currentTime = timer.substring(timer.indexOf(' '), timer.lastIndexOf(':'));  
```

## 日期 + 时间

### Hour12 `/` => 2020/5/20 下午5:20:20

```js
const currentTime = new Date().toLocaleString();
```

### Hour24 `/` => 2020/5/20 17:20

```js
let timer = new Date().toLocaleString('chinese', { hour12: false });
const currentTime = timer.substring(0, timer.lastIndexOf(':'));
```

### Hour12 `:` => 2020-05-20 05:20

```js
function dateFormat() {
  // YYYY-MM-DD
  let timer = new Date()
    .toLocaleDateString()
    .replace(/\//g, "-")
    .split("-")
    .map((item) => {
      item = item <= 9 ? `0${item}` : item;
      return item;
    })
    .join("-");
  // HH-MM
  let timer2 = new Date()
    .toLocaleTimeString()
    .substring(2, new Date().toLocaleTimeString().lastIndexOf(":"))
    .split(":")
    .map((item) => {
      item = item <= 9 ? `0${item}` : item;
      return item;
    })
    .join(":");
  let currentTime = `${timer} ${timer2}`;
} 
```

### Hour24 `:` => 2020-05-20 17:20

```js
function dateFormat() {
  let timer = new Date().toLocaleString("chinese", { hour12: false });
  let timer2 = timer
    .replace(/\//g, "-")
    .substring(0, timer.indexOf(" "))
    .split("-")
    .map((item) => {
      return (item = item <= 9 ? `0${item}` : item);
    })
    .join("-");
  const currentTime = `${timer2}${timer.substring(
    timer.indexOf(" "),
    timer.length - 3
  )}`;
}  
```