# Bitcoin Synthesizer API

<br>

![](https://media.giphy.com/media/KPDZ55SvovQv6/giphy.gif)

<br>

This API was written for the [Bitcoin Synthesizer](https://bitcoinsynth.net/). You can query either a list of available cryptocurrency assets and corresponding to that audio buffer per cryptocurrency pair to use with the Web Audio API.

Early versions of the Blockchain Synthesizer used to query every single time against an API endpoint of a cryptocurrency marketplace. Due to request limits on those API's, I came up with this simple "API". It's used to buffer and minimize API calls and it automatically takes care of converting the trade data into usable audio buffer data.
<br><br><br>


### Request the list of available crypto asset pairs
```https://api.bitcoinsynth.net/?action=assetlist```

GET parameter
* action=assetlist
<br><br>


### Request the sample buffer data of a specific asset pair
```https://api.bitcoinsynth.net/?action=assetpair&assetpair=dasheur```

GET parameter
* action=assetpair
* assetpair=yourassetpair (e.g. DASHEUR (Dash in Euro) -> get full list using action=assetlist)
