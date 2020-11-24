# JavaScript30
This is my repo of 30 days JavaScript Challenge

<img src="https://camo.githubusercontent.com/13a16597bc17b350b043e30ab701082fc276d3c4/68747470733a2f2f6a61766173637269707433302e636f6d2f696d616765732f4a53332d736f6369616c2d73686172652e706e67" alt="JavaScript30">
Starter Files from https://github.com/wesbos/JavaScript30

## Day-1

Data-key, keycode, and audio tag

## Day-2

CSS transform rotate degrees, setInterval, and use `new Date()` method to get current time

## Day-3 

Make CSS variables, change spacing, blur, and color

## Day-4 

Cool array functions of `filter`, `map`, `reduce`, and `sort`

## Day-5

Flex and Flex Items https://flexbox.io/

```
    /* Flex Children */
    .panel > * {
    }

    .panel > *:first-child {
      transform: translateY(-100%);
    }

    .panel > *:last-child {
      transform: translateY(100%);
    }

```

Toggle effect when transition end 

```
function toggleActive(e) {
      console.log(e.propertyName);
      // if (e.propertyName === 'flex-grow') {
      if (e.propertyName.includes('flex')) {
        this.classList.toggle('open-active')
      }
    }
panels.forEach(panel => panel.addEventListener('transitionend', toggleActive))
```

## Day-6

show search results while typing

regular express `RegExp`:
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp

## Day-7

more array phototypes of `some`, `every`, `find`, `findIndex`, `splice`, `slice`

```
    // Some and Every Checks
    // Array.prototype.some() // is at least one person 19 or older?
    const isAdult = people.some(person => {
      const currentYear = (new Date()).getFullYear()
      return currentYear - person.year >= 19
    })
    console.log({isAdult});

    // Array.prototype.every() // is everyone 19 or older?
    const everyAdult = people.every(person => (new Date()).getFullYear() - person.year >= 19)
    console.log({everyAdult});
```

## Day-8

Draw rainbow line in Cavas

```
  const canvas = document.querySelector('#draw')
  const ctx = canvas.getContext('2d')
  canvas.width = window.innerWidth
  canvas.height = window.innerHeight
  ctx.strokeStyle = 'blue'
  ctx.lineJoin = 'round'
  ctx.lineCap = 'round'
  ctx.lineWidth = '50'
  ctx.globalCompositeOperation = 'screen'
```