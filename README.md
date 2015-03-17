# PyCrypt

PyCrypt is a small python utility for encrypting and decrypting AES.

## Requirements

* Python (2.7)
* pycrypto - [PyPI](https://pypi.python.org/pypi/pycrypto)

## Scripts

### encrypt.py

#### Usage

```
python encrypt.py [-h] key msg
```

#### Arguments

Argument|Explenation
--------|-----------
key     |The encryption key to encrypt the message with
msg     |The message to encrypt

### decrypt.py

#### Usage

```
python decrypt.py [-h] key msg
```

#### Arguments

Argument|Explenation
--------|-----------
key     |The encryption key to decrypt the message with
msg     |The encrypted message to decrypt

### Example

```
> python encrypt.py secret "Hello World\!"
9729c82afb07bcddd67b8d54b1efe13237d0c71edc96b7ceeae390c2b3

> python decrypt.py secret 9729c82afb07bcddd67b8d54b1efe13237d0c71edc96b7ceeae390c2b3
Hello World\!
```

(Notice the back-slash before the exclamation mark, this is to escape it, as it otherwise has special meaning in bash)
