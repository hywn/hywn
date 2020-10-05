```
const self = new Proxy({}, {
	get: (_, prop) => (...args) => obj => obj[prop](...args)
})

console.log(['hello', 'world'].map(self.slice(1)))
```
