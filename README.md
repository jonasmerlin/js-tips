# js-tips
A collection of small but useful tips for JavaScript development.

Once every now and then I stumble upon some small tips for how to improve your quality of life (keep your sanity) while devloping with JavaScript. Things that would almost certainly not be covered in a run of the mill introduction to the language.

These tips come from many different places and I will document their sources whereever I can (remember them.)

## Logging

### console.table

This exists:

```console.table(tableLikeVariableToLog)```

You're welcome.

Source: https://developer.mozilla.org/de/docs/Web/API/Console/table

(Though many people discovered this via @wesbos as far es I can tell, so credit where credit is due.)

### console.log object literal wrapping

Wrapping console.log arguments in an object literal will print the variable name along with its value.

```console.log(variableToLog)```

becomes

```console.log({ variableToLog })```

Source: https://twitter.com/DaniStefanovic/status/1011923716085821440

### The console.table object literal wrapping 1-2 punch (also there is destructuring)

```
const [isThisRealLife, year, til] = [false, 93, 'infinity']
console.table([{ isThisRealLife, year, til }])
```

Source: https://twitter.com/ThomasG77/status/798598482894295040

