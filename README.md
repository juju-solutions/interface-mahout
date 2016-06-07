# Overview

This interface layer handles the communication between the Apache Mahout and
its clients.


# Usage

## Provides

Charms providing this interface need the Apache Mahout.

This interface layer will set the following states, as appropriate:

  * `{relation_name}.joined`   The relation to a Mahout provider has been initialized.


## Requires

Charms requiring this interface make Apache Mahout available.

This interface layer will set the following state, as appropriate:

  * `{relation_name}.joined`   The relation to a Maout provider has been initialized.

An example use might be:

```python
@when('mahout.joined')
def mahout_joined(syslog):
    .....
```

# Contact Information

- <bigdata@lists.ubuntu.com>
