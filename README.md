# use-scroll-bar
[![Build Status](https://travis-ci.org/jskod/use-scroll-bar.svg?branch=master)](https://travis-ci.org/jskod/use-scroll-bar)

Get information of window scrollbar like current position and direction of last scroll.

# How to use?
```jsx
import React from 'react'
import { useScrollbar } from 'use-scroll-bar'


function App() {

	const scrollState = useScrollbar({ delay: 200 })

	retrun (
		<div>
			User has scrolled {scrollState.directionX}
		</div>
	)
}

```

# What this hook return?
```js
{
	directionX: 'left' || 'right',
	directionY: 'up' || 'down',
	scrollX: number,
	scrollY: number
}
```

