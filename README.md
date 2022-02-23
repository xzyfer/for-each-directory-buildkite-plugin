# For Each Directory Buildkite Plugin

Execute a command in each directory provided

## Example

Add the following to your `pipeline.yml`:

```yml
steps:
  - command: ls
    plugins:
      - xzyfer/for-each-directory#v1.0.0:
          parent: /apps
```

## Configuration

<!-- ### `directories` (Optional, []string)

An array of directories to `cd` into before executing the given command. -->

### `parent` (Required, string)

From this directory all child directories will be `cd`'d into before executing the given command.

## Developing

To run the tests:

```shell
docker-compose run --rm tests
```

## Contributing

1. Fork the repo
2. Make the changes
3. Run the tests
4. Commit and push your changes
5. Send a pull request
