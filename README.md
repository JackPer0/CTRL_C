<h1 align="center">❗CTRL+C </h1>

```python
from signal import signal , SIGINT
import sys

def handel(sig,frame):
    print("Eixt This is Exit")
    sys.exit(0)


if __name__ == "__main__":
    signal(SIGINT,handel)
    print("Running.....")
    while True:
        pass


````
