You can use the `datetime` module to calculate the difference between two time points.

- This is easiest to demonstrate in a Python shell rather than using a script.

```python
>>> from datetime import datetime
>>> t1 = datetime.now()
>>> t2 = datetime.now()
>>> t2 - t1
```

- Depending on how quickly you could type the `t2 = datetime.now()` command, you should see something like this:

```python
datetime.timedelta(0, 6, 843882)
```

- This is a `timedelta` object. It tells you how many days, seconds, and microseconds it took you to type the line starting with `t2`.

- To extract the days, seconds, or microseconds, you can do the following:

```python
>>> dt = t2 - 21
>>> dt.days
0
>>> dt.seconds
6
>>> dt.microseconds
843822
```
