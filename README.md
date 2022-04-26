
#### 
1. Run `yarn install `
2. Run `yarn run gsn-with-ganache` to run local ganache and bring up GSN contracts and relayer.
3. In another terminal, run `truffle migrate` to install MetaCoin
4. Run `yarn run dev` to run metacoin demo on `http://localhost:8080`
5. open a browser, and you can mint, and send coins, with no eth in your (metamask) account
6. you can also switch to `ropsten`/`kovan`/`rinkeby` to see it running there
    (or open it in http://metacoin.opengsn.org)

#### NOTES:

The `gsn-with-ganache` script above does 2 things:

- Starts `ganache` with same chainId and networkId (to overcome [limitation](https://github.com/MetaMask/metamask-extension/issues/8385) of Metamask)
- calls `npx gsn start`, to start all GSN components locally.
