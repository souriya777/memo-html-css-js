# CSS

## breakpoints

![image](https://user-images.githubusercontent.com/1582479/187416458-e4799583-0fde-4682-b8ae-710c7199a0c1.png)

(src: https://polypane.app/blog/the-breakpoints-we-tested-in-2021-and-the-ones-to-test-in-2022/)

# JS

## mini bounce / throttle

```
let debounceTimer;
let throttlePause;

function debounce(callback, time) {
  window.clearTimeout(debounceTimer);
  debounceTimer = window.setTimeout(callback, time);
}

function throttle(callback, time) {
  if (throttlePause) return;

  throttlePause = true;
  callback();

  setTimeout(() => {
    throttlePause = false;
  }, time);
}
```
