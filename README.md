# MyNFT — ERC-721

Coleccion NFT (ERC-721) implementada desde cero en Solidity, sin dependencias externas,
para demostrar comprension del estandar EIP-721.

## Caracteristicas

- Estandar EIP-721 completo: `ownerOf`, `balanceOf`, `transferFrom`, `safeTransferFrom`.
- **Metadata** via `tokenURI` (baseURI + id del token).
- Aprobaciones por token (`approve`) y por operador (`setApprovalForAll`) — compatible con marketplaces.
- `safeTransferFrom` con comprobacion de receptor (`IERC721Receiver`).
- **Mint** controlado por el owner, con limite de coleccion (`maxSupply`).
- baseURI configurable por el owner (`setBaseURI`).

## Constructor

| Parametro    | Tipo    | Descripcion                                   |
|--------------|---------|-----------------------------------------------|
| `_name`      | string  | Nombre de la coleccion                        |
| `_symbol`    | string  | Simbolo                                        |
| `_baseURI`   | string  | URI base de la metadata (ej. ipfs://.../)     |
| `_maxSupply` | uint256 | Limite de NFTs (0 = sin limite)               |

## Red

- Solidity `^0.8.24`
- Desplegado y verificado en **Base** mainnet.
- **Direccion:** `0x16Da112C0D4CDdfc6bF6526AAcC536713BB24638`
- **Explorer:** https://basescan.org/address/0x16Da112C0D4CDdfc6bF6526AAcC536713BB24638

## Licencia

MIT
