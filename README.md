# substrate-connect-bundle

This page just serves to show how you can use Substrate connect as bundle with the help of Polkadot JS Bundle.
Use them like so:

```js
<script src="//unpkg.com/@polkadot/rpc-provider/substrate-connect/index.js"></script>
<script src="//unpkg.com/@polkadot/api/bundle-polkadot-api.js"></script>
```
```js
console.log('ScProvider', ScProvider)
const { WsProvider, ApiPromise } = polkadotApi;
```