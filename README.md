Object tracking with OpenCV and TensorFlow.

## getting start
```console
$ pipenv install
```

if `MemoryError`
```console
$ sudo fallocate -l 1G /var/swapfile
$ sudo mkswap /var/swapfile
$ sudo swapon /var/swapfile
$ sudo sh -c 'echo "/var/swapfile none swap defaults 0 0" >> /etc/fstab'
```
