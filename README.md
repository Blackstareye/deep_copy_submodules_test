# Deep Copy Submodules Testing

this repo contains the testing that is done for the project [Deep Copy Submodules](todo)

## Prerequisites

You need to install [bats-core](https://github.com/bats-core/bats-core)

### Testing Ini Parser

 you need to create the reports:
toggle this comment in [ini_parser_caller](manual/ini_parser_caller.sh)#create_test_output

## Test Methods

### Unit Testing

you can run the unit tests with:

```bash
bats *.bats

```

or if you want a more pretty output (experimental)

```bash
# if you toggle one param '-s' it creates also an report file
# if you toggle also param'-p' it creates a pretty segmented unit testing report
bash run_all_tests.sh [-s -p]
```

### Manual

Use the caller of the sub units for debugging purposes

### Integration Tests

You can also have integration tests.
Therefore you need to copy the [integration test config](integration_test/integration_test.conf) to `"~/integration_test.conf"`. You can also toggle if the integration test helper contains your passwords in this conf or not.

You can also use the interactive mode and select the method you want to test.

```bash
# param '-s' make a silent integration test helper for your needed testing commands
# otherwise: interactive mode
bash integration_test.sh [-s]
```

## TestCoverage

see [Testcoverage](testcoverage.md)
