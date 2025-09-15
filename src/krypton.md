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

## Krypton 3 -> 4
```
letters_sorted_by_frequency=$(string=$(cat found1 found2 found3); for letter in {A..Z}; do echo $string | tr -cd $letter | wc
-c | xargs echo $letter; done | sort -n -k 2 -r | sed "s/\s.*//" | xargs echo -n | sed "s/\s//g")
english_letters_sorted_by_frequency=EATSORNIHCLDUPGFWYMBKVJXQZ
cat krypton4 | xargs echo | tr $letters_sorted_by_frequency $english_letters_sorted_by_frequency
```
Password => BRUTE
