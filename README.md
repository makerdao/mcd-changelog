# Maker Foundation Multi-Collateral DAI Public Releases Page

Go to https://changelog.makerdao.com/ to see the details.

## Process for updating the changelog

1. The Smart Contracts Team creates a PR; review done by someone else from the Smart Contracts Team and someone from the TechOps Team.

2. New contract addresses are published first to specific version URLs, e.g. https://changelog.makerdao.com/releases/mainnet/1.1.1/contracts.json . On the main page there is a disclaimer, saying that the addresses might not be yet in use.

3. Once the spell is cast and everything is deployed, "active" links would be updated to point to the new addresses - https://changelog.makerdao.com/releases/kovan/active/contracts.json and https://changelog.makerdao.com/releases/mainnet/active/contracts.json. For backwards compatibility, URLs using "latest" instead of "active" are also updated to point to the new addresses. Change [vercel.json](./vercel.json) to update the links using redirects.

4. Changes are communicated internally and externally - Rocket Chat and Forum topic.

## Using the changelog

Projects and developers who need to programmatically encode contract addresses are encouraged to use the "active" URLs rather than copy-pasting the addresses from the current changelog.
