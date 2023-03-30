# No Azure Action

This is a github action for ubuntu os that will remove azure from the apt source list.

I've found the azure apt source to be routinely offline on weekends, causing actions to fail. Removing the azure source fixes that problem.

## Usage

```yml
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: christopherpickering/no-azure
```

## Version

It is a good idea to add a version to prevent changes from surprising you.

```yml
- uses: christopherpickering/no-azure@0.0.1
```

Thanks for using! 🙏
