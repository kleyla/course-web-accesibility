## Navigation Content

### Navigating by Headers

- http://webaim.org/standards/wcag/checklist#sc1.3.2
- http://webaim.org/standards/wcag/checklist#sc2.4.10
- http://webaim.org/standards/wcag/checklist#sc1.3.1
- http://webaim.org/standards/wcag/checklist#sc2.4.1
- http://webaim.org/standards/wcag/checklist#sc2.4.6

```js
for (var i = 0, headings = $$("h1,h2,h3,h4,h5,h6"); i < headings.length; i++) {
  console.log(
    headings[i].textContent.trim() + " " + headings[i].tagName,
    headings[i]
  );
}
```

### Link Text

http://webaim.org/standards/wcag/checklist#sc2.4.9

```html
<a href="#internal">I am a link</a>
```

- shows up in links list
- works with the keyboard
- can be bookmarked

_Anti-patterns_

```html
<span class="link" onclick="doSomething()">Not a link</span>
<!-- code smell -->
<a href="#" onclick="doSomething()">Do something</a>
<button class="link" onclick="doSomething()">Do something</button>
```

Text like `learn more` van mal `learn more about resposive layouts`

### Landmarks

- <header>
- <nav>
- <main>
- <article>
- <aside>
- <section>
- <footer>
