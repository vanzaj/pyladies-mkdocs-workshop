# Technical details

Labore non nisi id aliquip ea. Cupidatat aliquip tempor qui adipisicing excepteur velit irure deserunt deserunt ullamco. Laborum deserunt deserunt laborum culpa laborum voluptate cillum est ex. Cillum eiusmod magna veniam dolore in tempor do esse do sint aliquip Lorem anim eiusmod. Qui amet laboris cupidatat aliquip tempor ut proident amet consectetur elit id exercitation.


## Code example

Mollit fugiat velit excepteur consequat dolor. Consequat nostrud do voluptate Lorem veniam nostrud culpa cupidatat est. Elit commodo ullamco dolor enim consequat nulla dolor commodo. Excepteur aliqua voluptate quis anim anim est est magna occaecat laborum amet culpa do. Nisi nisi aute ex quis velit.


    #!/bin/bash

    if [ ! -n "$1" ]; then
      echo "Usage: $(basename $0) file"
      exit 0
    fi

    today=$(date "+%Y%m%d")

    file_path=$(dirname "$1")
    file_name=$(basename "$1")
    new_name="${today}_${file_name}"

    /bin/mv "$1" $file_path/$new_name

## Images

Local img:
![Git commands](../img/git_cmd.png)

External img:
![Git commands](
  http://www.markus-gattol.name/misc/mm/si/content/git_everthing_is_local.png)

## Markdown extensions

### Tables

|Col A | Col B | Col C|
|------|-------|------|
| a1   |  b1   | c1   |
| a2   |  b2   | c2   |


### Fenced code blocks

~~~python
import random

def passwd(len=6):
    chars = '-_!abcdef123'
    return ''.join([random.choice(chars) for _ in range(len)])
~~~
