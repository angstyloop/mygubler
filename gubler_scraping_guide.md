# javascript

// In the Javascript console console, run this code to get all full-sized images from the Google search images page.
// Be sure to maximize the number of available search results by adjusting search settings, and scrolling to the bottom.
// You may have to play with the numbers a little.

```
images=[...document.getElementsByTagName('img')].filter(it=>50<Math.max(it.width,it.height))
(async() => {
    for (let i=0; i<images.length; ++i) {
        images[i].click()
        await sleep(2000)
        image = [...document.getElementsByTagName('img')].filter(it=>300<Math.min(it.width,it.height))[0] || {src:''}
        await sleep(2000)
        q.push(image.src)
    }
})()
```
