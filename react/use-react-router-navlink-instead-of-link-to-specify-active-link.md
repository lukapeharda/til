# Use React Router `<NavLink>` component instead of `<Link>` to specify active navigation link

If using React Router for navigation and you're wondering how to show `active` state for a navigation link just use `<NavLink>` component which accepts additional param called `activeClassName` which will be appended to element based on active route.

```js
import { NavLink } from 'react-router-dom';

...

<NavLink 
  to="/dashboard" 
  className="text-gray-500" 
  activeClassName="bg-gray-500 text-white">
    Dashboard
</NavLink>
```

[Source](https://reacttraining.com/react-router/web/api/NavLink)
