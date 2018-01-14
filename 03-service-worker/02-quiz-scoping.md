# 03.02: QUIZ: SCOPING QUIZ
Given this registration code, which page URLs will this service worker control?

```js
navigator.serviceWorker.register('/sw.js', {
  scope: '/foo/'
});
```

  - [ ] /
  - [ ] /sw.js
  - [ ] /foo
  - [ ] /foo.html
  - [ ] /foo/
  - [ ] /foo/bar/index.html
  - [ ] /foo/bar

<details>
  <summary>ANSWER</summary>
  <p>
    - [ ] /
    - [ ] /sw.js
    - [ ] /foo
    - [ ] /foo.html
    - [x] /foo/
    - [x] /foo/bar/index.html
    - [x] /foo/bar
  </p>
  <p>
    The Service Worker will control any page URL that begins with the scope. Remember, the trailing slash is important!
  </p>
</details>

- - -

Next: [Adding a Service Worker To the Project](./03-adding-service-worker.md)