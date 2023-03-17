# Reto día #17

## 🎄 La locura de enviar paquetes en esta época

### 🟥 Difícil

### Llega la época de navidades y las empresas de transporte están sacando cuentas del número de paquetes van a poder enviar. ¡A ver cómo lo hacemos!

```js
export default function countPackages(carriers, carrierID) {
  const carrier = carriers.find(c => c[0] === carrierID)
  let count = carrier[1]
  carrier[2].forEach(c => {
    count += countPackages(carriers, c)
  })
  return count
}


```

- [Link al reto 17](https://adventjs.dev/challenges/17)
- [Link al reto anterior](./reto16.md)
- [Link al siguiente reto](./reto18.md)