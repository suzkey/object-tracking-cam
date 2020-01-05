Object tracking with OpenCV and TensorFlow, and serve it on the web.

## getting start with pipenv
```console
$ pipenv install
$ git submodule update --init
$ pipenv shell
$ cd darkflow && python setup.py build_ext --inplace && pip install -e .
$ pipenv run python server.py
```
You will be able to check the camera startup by accessing localhost:5000.

![](https://i.gyazo.com/1814043ab5576d2561554d0a25747b57.png)

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
