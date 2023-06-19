# Gruf Demo Rails Application

This is a demo Rails application that utilizes [gruf](https://github.com/bigcommerce/gruf) 2.1.0+, a gRPC Ruby framework.

## Running

Set the database URL as a `DATABASE_URL` env var in a `.env` file, then:

```bash
bundle install
bundle exec rake db:create db:migrate
bundle exec rake db:seed
foreman start
```

## Testing with a Client

Then in another console, you can run provided rake tasks to see it in action.

### Request/Response (Get a Product)

```bash
bundle exec rake test:get_product
```

### Server Streamer (Get a list of Products)

```bash
bundle exec rake test:get_products
```

### Client Streamer (Create a list of Products)

```bash
bundle exec rake test:create_products
```

### Bidirectional Streamer (Create a list of Products and get back responses immediately in stream)

```bash
bundle exec rake test:create_products_in_stream
```
