```javascript
const new_clicker = () => {

	let count = 0
	
	return {
		click: () => ++count,
		get_count: () => count
	}
	
}

const my_clicker = new_clicker()

console.log(my_clicker.get_count())
my_clicker.click()
my_clicker.click()
console.log(my_clicker.get_count())
```
