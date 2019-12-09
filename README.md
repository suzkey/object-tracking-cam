Object tracking with OpenCV and TensorFlow.

## getting start with pipenv
```console
$ pipenv install
$ git submodule update --init
$ pipenv shell
$ cd darkflow && python setup.py build_ext --inplace && pip install -e .
$ pipenv run python server.py
```
You will be able to check the camera startup by accessing localhost:5000.

![](https://gyazo.com/cd208c4f54bcb46cd4ecdd0db459d48e.png)

## `MemoryError`
Please try this commands.
```console
$ sudo fallocate -l 1G /var/swapfile
$ sudo mkswap /var/swapfile
$ sudo swapon /var/swapfile
$ sudo sh -c 'echo "/var/swapfile none swap defaults 0 0" >> /etc/fstab'
```

## references
[GitHub - thtrieu/darkflow: Translate darknet to tensorflow. Load trained weights, retrain/fine-tune using tensorflow, export constant graph def to mobile devices](https://github.com/thtrieu/darkflow)
