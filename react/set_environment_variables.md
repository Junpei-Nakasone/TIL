# Set environment variable in React application

- create `.env` file at root directory(same as `src` directory, not in `src` directory).

- Define environment variable in `.env` file
variable name needs to begin with `REACT_APP_` like below.
```bash
REACT_APP_EXAMPLE=12345
```

- Read environment variable
You can read environment variable using `process.env` like below.
```js
{process.env.REACT_APP_EXAMPLE}
```

- Start local server
Run `npm start` to start local server. If you already stated before set the environment variables, you need to stop and restart that.
