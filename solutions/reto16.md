# Reto día #16

## 🎄 Decifrando los números

### 🟩 Fácil

### Hemos encontrado unas cartas misteriores que contienen un montón de símbolos. Por suerte tenemos el diccionario para decodificarlas. ¡Vamos a ver qué contienen!

```js
export default function decodeNumber(symbols) {
  let decoded = 0
 	const dictionary = {
    ".": 1,
    ",": 5,
    ":": 10,
    ";": 50,
    "!": 100,
  }
  const symbolsArray = Array.from(symbols)
  symbolsArray.forEach((symbol, i, array) => {
    if(dictionary[symbol] < dictionary[array[i + 1]]) {
      decoded = -dictionary[symbols[i]] + decoded
    } else {
      decoded = dictionary[symbols[i]] + decoded
    }
  })
  
  return decoded
}

```

- [Link al reto 16](https://adventjs.dev/challenges/16)
- [Link al reto anterior](./reto15.md)
- [Link al siguiente reto](./reto17.md)
