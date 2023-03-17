# Reto día #18

## 🎄 El sistema operativo de Santa Claus

### 🟩 Fácil

### Estamos programando un sistema operativo para los ordenadores del taller de Santa Claus... Tenemos que gestionar los nombres de los archivos para que no se repitan.

```js
export default function fixFiles(files) {
 	const count = {}
  return files.map(file => {
    if(file in count) return `${file}(${++count[file]})`
    else {
      count[file] = 0
      return file
    }
  })
}


```

- [Link al reto 18](https://adventjs.dev/challenges/18)
- [Link al reto anterior](./reto17.md)
- [Link al siguiente reto](./reto19.md)
