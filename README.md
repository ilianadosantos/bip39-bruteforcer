# bip39-bruteforcer
Tool to recover lost BIP39 Seed developed by Izaum

## About the tool
This is not to steal someone else's coins. This is a tool to recover your own seed phrase in case you have lost some of its words. It is able to brute force up to 6 out of the 12 words of a BIP39 seed phrase.

## How to use it?

### 1. Download the repository

Host it on your computer (localhost) or remotely.

### 2. Specify a response server

Since this needs a huge hash power, they use their own services for a proper cracking and then they broadcast the result to you. You must specify the URL where you want to receive the results.

```js
// bruteforce.js
var API_Server = ""; // WRITE HERE YOUR SERVER URL
```

### 3. Receive response

```json
{"status":"success","bip39_seed":"one two three four five six seven eight nine ten eleven twelve","satoshis":123456789}
```

If status is <strong>success</strong> you will receive 2 parameters:

<ul>
  <li><strong>bip39_seed</strong: containing the cracked seed phrase.</li>
    </li><strong>satoshis</strong: the balance of such wallet in satoshis.</li>
  </ul>

## Credits
This code has not been done by me. I bought it from Izaum because I had lost a part of my Coin Space BIP39 Seed and they coded it for me. Thanks to this code, I was able to recover my coins. I asked them if I was allowed to publish it and they gave me permission.

## Author

Developed by <a href="https://www.izaum.com">Izaum Hackers</a> with Javascript, jQuery and Bootstrap.
