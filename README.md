# Deprecation Notice

MakerDAO’s Changelog was deprecated in favor of its on-chain counterpart, the Chainlog. Please refer to the following resources:

* [Forum post for the change](https://forum.makerdao.com/t/chainlog-improving-how-we-keep-track-of-our-deployed-contracts/11834)
* [Chainlog contract’s source code](https://github.com/makerdao/dss-chain-log)
* [Chainlog contract’s mainnet deployment](https://etherscan.io/address/0xda0ab1e0017debcd72be8599041a2aa3ba7e740f)
* [UI and API’s source code](https://github.com/makerdao/chainlog-ui)
* [UI](https://chainlog.makerdao.com)
* [API](https://chainlog.makerdao.com/api.html)

# Old README

## Maker Foundation Multi-Collateral DAI Public Releases Page

Go to https://changelog.makerdao.com/ to see the details.

### Process for updating the changelog

1. The Protocol Engineering Core Unit creates a PR; review done by someone else from the PECU and someone from the TechOps Team.

2. New contract addresses are published first to specific version URLs, e.g. https://changelog.makerdao.com/releases/mainnet/1.9.9/contracts.json . On the main page there is a disclaimer, saying that the addresses might not be yet in use.

3. Once the spell is cast and everything is deployed, "active" links would be updated to point to the new addresses - https://changelog.makerdao.com/releases/goerli/active/contracts.json and https://changelog.makerdao.com/releases/mainnet/active/contracts.json, as well as https://changelog.makerdao.com/releases/goerli/active/ and https://changelog.makerdao.com/releases/mainnet/active/. For backwards compatibility, URLs using "latest" instead of "active" are also updated to point to the new addresses. Change [vercel.json](./vercel.json) to update the links using redirects.

4. Changes are communicated internally and externally - Rocket Chat and Forum topic.

### Using the changelog

Projects and developers who need to programmatically encode contract addresses are encouraged to use the "active" URLs rather than copy-pasting the addresses from the current changelog.
