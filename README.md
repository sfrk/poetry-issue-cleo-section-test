To execute this test:

```shell
$ poetry install
$ poetry run python main.py greet johndoe > output.txt
$ cat output.txt
lul
Hello johndoe
```

So both `section.write_line` and `self._io.write_line` from inside the command end up in stdout – as opposed to what happens to some of the output when running `$ poetry install -vvv` in a poetry project.
