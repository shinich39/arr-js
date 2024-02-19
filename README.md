## arr-js

Array utilities in javascript.

## Usage

```js
import arrJs from 'arr-js';
```

- min

```js
const data = [3,1,2];

const result = arrJs.min(data);
// 1
```

- max

```js
const data = [3,1,2];

const result = arrJs.min(data);
// 3
```

- mean

```js
const data = [10,20,70];

const result = arrJs.mean(data);
// 50
```

- mode

```js
const data = [3,1,3,1,3,2];

const result = arrJs.mode(data);
// 3
```

- spread

```js
const data = [
	[1,2,3],		// first values
	[11,12,13],	// second values
	[21,22,23],	// third values
							// ...
];

const result = arrJs.spread(data);
// [
// 	[ 1, 11, 21 ],
// 	[ 2, 11, 21 ],
// 	[ 3, 11, 21 ],
// 	[ 1, 12, 21 ],
// 	[ 2, 12, 21 ],
// 	[ 3, 12, 21 ],
// 	[ 1, 13, 21 ],
// 	[ 2, 13, 21 ],
// 	[ 3, 13, 21 ],
// 	[ 1, 11, 22 ],
// 	[ 2, 11, 22 ],
// 	...
// ]
```

- around

```js
const data = [0,1,2,3,4,5,6,7,8,9];
const index = 0;
const size = 3;

const result = arrJs.around(data, index, size);
// [ 0, 1, 2 ]

const result = arrJs.around(data, 9, 3);
// [ 7, 8, 9 ]
```