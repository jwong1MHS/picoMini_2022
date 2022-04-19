# Beginner PicoMini 2022

A beginner-style CTF hosted on picoGym at https://play.picoctf.org/practice?originalEvent=69

## Table of Contents

| Categories     | Completed | Progress                                                     | Points    |
| -------------- | --------- | ------------------------------------------------------------ | --------- |
| General Skills | 13/13     | ![](https://us-central1-progress-markdown.cloudfunctions.net/progress/100) | 1300/1300 |

## Codebooks

### *Description*

Run the Python script <span style="color: #e83e8c;">`code.py`</span> in the same directory as <span style="color: #e83e8c;">`codebook.txt`</span>.

- [Download code.py](https://artifacts.picoctf.net/c/101/code.py)
- [Download codebook.txt](https://artifacts.picoctf.net/c/101/codebook.txt)

<details>
    <summary>Hint 1</summary>
    On the webshell, use <span style="color: #e83e8c;">ls</span> to see if both files are in the directory you are in
</details>

<details>
    <summary>Hint 2</summary>
    The <span style="color: #e83e8c;">str_xor</span> function does not need to be reverse engineered for this challenge.
</details>

### *Writeup*

Run the Python script as such: `python3 code.py`. Make sure `codebooks.txt` is in the same directory as the python program.

```bash
└─$ python3 code.py
picoCTF{c0d3b00k_455157_7d102d7a}
```

Flag: `picoCTF{c0d3b00k_455157_7d102d7a}`

## convertme.py

### *Description*

Run the Python script and convert the given number from decimal to binary to get the flag.

[Download Python script](https://artifacts.picoctf.net/c/30/convertme.py)

<details>
    <summary>Hint 1</summary>
    Look up a decimal to binary number conversion app on the web or use your computer's calculator!
</details>

<details>
    <summary>Hint 2</summary>
    The <span style="color: #e83e8c;">str_xor</span> function does not need to be reverse engineered for this challenge.
</details>

<details>
    <summary>Hint 3</summary>
    If you have Python on your computer, you can download the script normally and run it. Otherwise, use the <span style="color: #e83e8c;">wget</span> command in the webshell.
</details>

<details>
    <summary>Hint 4</summary>
    To use <span style="color: #e83e8c;">wget</span> in the webshell, first right click on the download link and select 'Copy Link' or 'Copy Link Address'
</details>

<details>
    <summary>Hint 5</summary>
    Type everything after the dollar sign in the webshell: <span style="color: #e83e8c;">$ wget </span>, then paste the link after the space after <span style="color: #e83e8c;">wget</span> and press enter. This will download the script for you in the webshell so you can run it!
</details>

<details>
    <summary>Hint 6</summary>
    Finally, to run the script, type everything after the dollar sign and then press enter: <span style="color: #e83e8c;">$ python3 convertme.py</span>
</details>

### *Writeup*

Run the Python script as such: `python3 convertme.py` and do the decimal to binary challenge. The number will change every time.

```bash
└─$ python3 convertme.py
If 38 is in decimal base, what is it in binary base?
Answer: 100110
That is correct! Here's your flag: picoCTF{4ll_y0ur_b4535_762f748e}
```

Flag: `picoCTF{4ll_y0ur_b4535_762f748e}`

## fixme1.py

### *Description*

Fix the syntax error in this Python script to print the flag.

[Download Python script](https://artifacts.picoctf.net/c/38/fixme1.py)

<details>
    <summary>Hint 1</summary>
    Indentation is very meaningful in Python
</details>

<details>
    <summary>Hint 2</summary>
    To view the file in the webshell, do: <span style="color: #e83e8c;">$ nano fixme1.py</span>
</details>

<details>
    <summary>Hint 3</summary>
    To exit <span style="color: #e83e8c;">nano</span>, press Ctrl and x and follow the on-screen prompts.
</details>

<details>
    <summary>Hint 4</summary>
    The <span style="color: #e83e8c;">str_xor</span> function does not need to be reverse engineered for this challenge.
</details>

### *Writeup*

Run `nano fixme1.py` to remove the spaces before the last print statement. Save by using <kbd>Ctrl+S</kbd> and exit by <kbd>Ctrl+X</kbd>. Then run the Python script as such: `python3 fixme1.py`.

```bash
└─$ python3 fixme1.py
That is correct! Here's your flag: picoCTF{1nd3nt1ty_cr1515_09ee727a}
```

Flag: `picoCTF{1nd3nt1ty_cr1515_09ee727a}`

## fixme2.py

### *Description*

Fix the syntax error in the Python script to print the flag.

[Download Python script](https://artifacts.picoctf.net/c/67/fixme2.py)https://artifacts.picoctf.net/c/38/fixme1.py)

<details>
    <summary>Hint 1</summary>
    Are equality and assignment the same symbol?
</details>

<details>
    <summary>Hint 2</summary>
    To view the file in the webshell, do: <span style="color: #e83e8c;">$ nano fixme2.py</span>
</details>

<details>
    <summary>Hint 3</summary>
    To exit <span style="color: #e83e8c;">nano</span>, press Ctrl and x and follow the on-screen prompts.
</details>

<details>
    <summary>Hint 4</summary>
    The <span style="color: #e83e8c;">str_xor</span> function does not need to be reverse engineered for this challenge.
</details>

### *Writeup*

Run `nano fixme2.py` to add another `=` symbol when the program checks if the `flag` variable is equal to an empty string.

`flag = ''` is an assignment, `flag == ''` is an equality check. Then run the Python script as such: `python3 fixme2.py`.

```bash
└─$ python3 fixme2.py
That is correct! Here's your flag: picoCTF{3qu4l1ty_n0t_4551gnm3nt_f6a5aefc}
```

Flag: `picoCTF{3qu4l1ty_n0t_4551gnm3nt_f6a5aefc}`

## Glitch Cat

### *Description*

Our flag printing service has started glitching! <span style="color: #e83e8c;">`$ nc saturn.picoctf.net 53933`</span>

<details>
    <summary>Hint 1</summary>
    ASCII is one of the most common encodings used in programming
</details>

<details>
    <summary>Hint 2</summary>
    We know that the glitch output is valid Python, somehow!
</details>

<details>
    <summary>Hint 3</summary>
    Press Ctrl and c on your keyboard to close your connection and return to the command prompt.
</details>

### *Writeup*

Running netcat on the server will print `'picoCTF{gl17ch_m3_n07_' + chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65) + '}'`, which if ran in python will print the flag.

```bash
└─$ python3
Python 3.9.12 (main, Mar 24 2022, 13:02:21)
[GCC 11.2.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> print('picoCTF{gl17ch_m3_n07_' + chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65) + '}')
picoCTF{gl17ch_m3_n07_a4392d2e}
```

Flag: `picoCTF{gl17ch_m3_n07_a4392d2e}`

## HashingJobApp

### *Description*

If you want to hash with the best, beat this test! <span style="color: #e83e8c;">`$ nc saturn.picoctf.net 63116`</span>

<details>
    <summary>Hint 1</summary>
    You can use a commandline tool or web app to hash text
</details>

<details>
    <summary>Hint 2</summary>
    Press Ctrl and c on your keyboard to close your connection and return to the command prompt.
</details>

### *Writeup*

Use `md5sum`.

```bash
└─$ nc saturn.picoctf.net 63116
Please md5 hash the text between quotes, excluding the quotes: 'hairballs'
Answer:
360927e98748b8675251a4a68b637b4b
360927e98748b8675251a4a68b637b4b
Correct.
Please md5 hash the text between quotes, excluding the quotes: 'Keanu Reeves'
Answer:
4d2e1f8eabca061706aec58b21c2e199
4d2e1f8eabca061706aec58b21c2e199
Correct.
Please md5 hash the text between quotes, excluding the quotes: 'my sixteenth birthday'
Answer:
97a710ca19764e4bcdd09966d7a28859
97a710ca19764e4bcdd09966d7a28859
Correct.
picoCTF{4ppl1c4710n_r3c31v3d_bf2ceb02}
```

Flag: `picoCTF{4ppl1c4710n_r3c31v3d_bf2ceb02}`

## PW Crack 1

### *Description*

Can you crack the password to get the flag?

Download the password checker [here](https://artifacts.picoctf.net/c/51/level1.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/51/level1.flag.txt.enc) in the same directory too.

### *Writeup*

Looking at the contents of level1.py shows that the program falls through the if statement if `user_pw == "691d"`.

```bash
└─$ python3 level1.py
Please enter correct password for flag: 691d
Welcome back... your flag, user:
picoCTF{545h_r1ng1ng_56891419}
```

Flag: `picoCTF{545h_r1ng1ng_56891419}`

## PW Crack 2

### *Description*

Can you crack the password to get the flag?

Download the password checker [here](https://artifacts.picoctf.net/c/17/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/17/level2.flag.txt.enc) in the same directory too.

### *Writeup*

View the contents again, but this time the string that `user_pw` checks against is in unicode, so throwing it in python should return the password as an ASCII string.

```bash
└─$ python3
Python 3.9.12 (main, Mar 24 2022, 13:02:21)
[GCC 11.2.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> print(chr(0x34) + chr(0x65) + chr(0x63) + chr(0x39))
4ec9
```

```bash
└─$ python3 level2.py
Please enter correct password for flag: 4ec9
Welcome back... your flag, user:
picoCTF{tr45h_51ng1ng_9701e681}
```

Flag: `picoCTF{tr45h_51ng1ng_9701e681}`

## PW Crack 3

### *Description*

Can you crack the password to get the flag?

Download the password checker [here](https://artifacts.picoctf.net/c/24/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/24/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/24/level3.hash.bin) in the same directory too.

There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.

### *Writeup*

```bash
└─$ python3 level3.py
Please enter correct password for flag: dba8
Welcome back... your flag, user:
picoCTF{m45h_fl1ng1ng_cd6ed2eb}
```

Flag: `picoCTF{m45h_fl1ng1ng_cd6ed2eb}`

## PW Crack 4

### *Description*

Can you crack the password to get the flag?

Download the password checker [here](https://artifacts.picoctf.net/c/60/level4.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/60/level4.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/60/level4.hash.bin) in the same directory too.

There are 100 potential passwords with only 1 being correct. You can find these by examining the password checker script.

### *Writeup*

Make a python file that will iterate through all 100 passwords and calculate the md5sum of each one, and compare it to the has bin file, and then return the password.

```bash
import hashlib

correct_pw_hash = open('level4.hash.bin', 'rb').read()

def hash_pw(pw_str):
    pw_bytes = bytearray()
    pw_bytes.extend(pw_str.encode())
    m = hashlib.md5()
    m.update(pw_bytes)
    return m.digest()

pos_pw_list = ["8c86", "7692", "a519", "3e61", "7dd6", "8919", "aaea", "f34b", "d9a2", "39f7", "626b", "dc78", "2a98", "7a85", "cd15", "80fa", "8571", "2f8a", "2ca6", "7e6b", "9c52", "7423", "a42c", "7da0", "95ab", "7de8", "6537", "ba1e", "4fd4", "20a0", "8a28", "2801", "2c9a", "4eb1", "22a5", "c07b", "1f39", "72bd", "97e9", "affc", "4e41", "d039", "5d30", "d13f", "c264", "c8be", "2221", "37ea", "ca5f", "fa6b", "5ada", "607a", "e469", "5681", "e0a4", "60aa", "d8f8", "8f35", "9474", "be73", "ef80", "ea43", "9f9e", "77d7", "d766", "55a0", "dc2d", "a970", "df5d", "e747", "dc69", "cc89", "e59a", "4f68", "14ff", "7928", "36b9", "eac6", "5c87", "da48", "5c1d", "9f63", "8b30", "5534", "2434", "4a82", "d72c", "9b6b", "73c5", "1bcf", "c739", "6c31", "e138", "9e77", "ace1", "2ede", "32e0", "3694", "fc92", "a7e2"]

for i in pos_pw_list:
    user_pw = i
    user_pw_hash = hash_pw(user_pw)
    if( user_pw_hash == correct_pw_hash ):
        print(user_pw)
```

```bash
└─$ python3 input.py
607a
```

```bash
└─$ python3 level4.py
Please enter correct password for flag: 607a
Welcome back... your flag, user:
picoCTF{fl45h_5pr1ng1ng_d770d48c}
```

Flag: `picoCTF{fl45h_5pr1ng1ng_d770d48c}`

## PW Crack 5

### *Description*

Can you crack the password to get the flag?

Download the password checker [here](https://artifacts.picoctf.net/c/79/level5.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/79/level5.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/79/level5.hash.bin) in the same directory too. Here's a [dictionary](https://artifacts.picoctf.net/c/79/dictionary.txt) with all possible passwords based on the password conventions we've seen so far.

### *Writeup*

Make a python file that will iterate through all 16^4 passwords and calculate the md5sum of each one, and compare it to the has bin file, and then return the password.

```bash
import hashlib

correct_pw_hash = open('level5.hash.bin', 'rb').read()

def hash_pw(pw_str):
    pw_bytes = bytearray()
    pw_bytes.extend(pw_str.encode())
    m = hashlib.md5()
    m.update(pw_bytes)
    return m.digest()

with open('dictionary.txt') as f:
    pos_pw_list = f.readlines()

for i in pos_pw_list:
    user_pw = i.strip()
    user_pw_hash = hash_pw(user_pw)
    if( user_pw_hash == correct_pw_hash ):
        print(user_pw)
```

```bash
└─$ python3 input.py
9581
```

```bash
└─$ python3 level5.py
Please enter correct password for flag: 9581
Welcome back... your flag, user:
picoCTF{h45h_sl1ng1ng_36e992a6}
```

Flag: `picoCTF{h45h_sl1ng1ng_36e992a6}`

## runme.py

### *Description*

Run the `runme.py` script to get the flag. Download the script with your browser or with `wget` in the webshell.[Download runme.py Python script](https://artifacts.picoctf.net/c/86/runme.py)

### *Writeup*

```bash
└─$ python3 runme.py
picoCTF{run_s4n1ty_run}
```

Flag: `picoCTF{run_s4n1ty_run}`

## Serpentine

### *Description*

Find the flag in the Python script!

[Download Python script](https://artifacts.picoctf.net/c/94/serpentine.py)

### *Writeup*

Take a segment of the python program and run the print_flag function.

```bash
def str_xor(secret, key):
    #extend key to secret length
    new_key = key
    i = 0
    while len(new_key) < len(secret):
        new_key = new_key + key[i]
        i = (i + 1) % len(key)
    return "".join([chr(ord(secret_c) ^ ord(new_key_c)) for (secret_c,new_key_c) in zip(secret,new_key)])

flag_enc = chr(0x15) + chr(0x07) + chr(0x08) + chr(0x06) + chr(0x27) + chr(0x21) + chr(0x23) + chr(0x15) + chr(0x5c) + chr(0x01) + chr(0x57) + chr(0x2a) + chr(0x17) + chr(0x5e) + chr(0x5f) + chr(0x0d) + chr(0x3b) + chr(0x19) + chr(0x56) + chr(0x5b) + chr(0x5e) + chr(0x36) + chr(0x53) + chr(0x07) + chr(0x51) + chr(0x18) + chr(0x58) + chr(0x05) + chr(0x57) + chr(0x11) + chr(0x3a) + chr(0x0f) + chr(0x0a) + chr(0x5b) + chr(0x57) + chr(0x41) + chr(0x55) + chr(0x0c) + chr(0x59) + chr(0x14)

def print_flag():
    flag = str_xor(flag_enc, 'enkidu')
    print(flag)

print_flag()
```

```bash
└─$ python3 input.py
picoCTF{7h3_r04d_l355_7r4v3l3d_aa2340b2}
```

Flag: `picoCTF{7h3_r04d_l355_7r4v3l3d_aa2340b2}`

