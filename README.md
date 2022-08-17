# substrate-connect-bundle

This page just serves to show how you can use Substrate connect as bundle with the help of Polkadot JS Bundle.
Use them like so:

```js
  <script src="https://unpkg.com/@polkadot/api/bundle-polkadot-api.js"></script>
```
```js
  const { ApiPromise, ScProvider } = polkadotApi;
  const { WellKnownChain } = ScProvider;

  const provider = new ScProvider(WellKnownChain.polkadot);
  provider.connect()
  const polkadotLight = await ApiPromise.create({ provider });
  ......
  polkadotLight.derive.chain.subscribeNewHeads((header) => {
    polkadotLightBlock.innerText = header.number;
  });
```