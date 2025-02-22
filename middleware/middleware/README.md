# Middleware: Various

This example showcases a bunch of different uses of middleware. See also the [Middleware guide](https://actix.rs/docs/middleware/).

## Usage

```sh
cd basics/middleware
cargo run
# Started http server: 127.0.0.1:8080
```

Look in `src/main.rs` and comment the different middleware in/out to see how they function.

## Middleware

### `redirect::CheckLogin`

A middleware implementing a request guard which sketches a rough approximation of what a login could look like.

### `read_request_body::Logging`

A middleware demonstrating how to read out the incoming request body.

### `read_response_body::Logging`

A middleware demonstrating how to read out the outgoing response body.

### `simple::SayHi`

A minimal middleware demonstrating the sequence of operations in an actix middleware.
There is a second version of the same middleware using `wrap_fn` which shows how easily a middleware can be implemented in actix.

## See Also

- The `from_fn` middleware constructor from [`actix-web-lab`](https://crates.io/crates/actix-web-lab).
