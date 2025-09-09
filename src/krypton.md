# Krypton Solutions

## Krypton 0 -> 1
[Commands of your local shell included]
```
base64 -d S1JZUFRPTklTR1JFQVQ=
```
Password => KRYPTONISGREAT

## Krypton 1 -> 2
```
cd /krypton/krypton1
cat krypton2 | tr A-Za-z N-ZA-Mn-za-m
```
Password => ROTTEN

## Krypton 2 -> 3
```
mkdir /tmp/tempdir
cd /tmp/tempdir
ln -s /krypton/krypton2/ krypton2
ln -s /krypton/krypton2/keyfile.dat keyfile.dat
echo "A" > text
krypton2/encrypt text
cat ciphertext
cat krypton2/krypton3 | tr M-ZA-L A-Z
```
Password => CAESARISEASY
