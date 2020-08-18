# External module: "utils/signing-utils"

## Index

### Interfaces

* [RLPEncodedTx](../interfaces/_utils_signing_utils_.rlpencodedtx.md)

### Functions

* [chainIdTransformationForSigning](_utils_signing_utils_.md#chainidtransformationforsigning)
* [decodeSig](_utils_signing_utils_.md#decodesig)
* [encodeTransaction](_utils_signing_utils_.md#encodetransaction)
* [getHashFromEncoded](_utils_signing_utils_.md#gethashfromencoded)
* [recoverMessageSigner](_utils_signing_utils_.md#recovermessagesigner)
* [recoverTransaction](_utils_signing_utils_.md#recovertransaction)
* [rlpEncodedTx](_utils_signing_utils_.md#rlpencodedtx)
* [verifyEIP712TypedDataSigner](_utils_signing_utils_.md#verifyeip712typeddatasigner)

## Functions

###  chainIdTransformationForSigning

▸ **chainIdTransformationForSigning**(`chainId`: number): *number*

*Defined in [packages/contractkit/src/utils/signing-utils.ts:27](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/utils/signing-utils.ts#L27)*

**Parameters:**

Name | Type |
------ | ------ |
`chainId` | number |

**Returns:** *number*

___

###  decodeSig

▸ **decodeSig**(`sig`: any): *object*

*Defined in [packages/contractkit/src/utils/signing-utils.ts:208](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/utils/signing-utils.ts#L208)*

**Parameters:**

Name | Type |
------ | ------ |
`sig` | any |

**Returns:** *object*

* **r**: *Buffer‹›* = ethUtil.toBuffer(r) as Buffer

* **s**: *Buffer‹›* = ethUtil.toBuffer(s) as Buffer

* **v**: *number* = parseInt(v, 16)

___

###  encodeTransaction

▸ **encodeTransaction**(`rlpEncoded`: [RLPEncodedTx](../interfaces/_utils_signing_utils_.rlpencodedtx.md), `signature`: object): *Promise‹EncodedTransaction›*

*Defined in [packages/contractkit/src/utils/signing-utils.ts:120](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/utils/signing-utils.ts#L120)*

**Parameters:**

▪ **rlpEncoded**: *[RLPEncodedTx](../interfaces/_utils_signing_utils_.rlpencodedtx.md)*

▪ **signature**: *object*

Name | Type |
------ | ------ |
`r` | Buffer |
`s` | Buffer |
`v` | number |

**Returns:** *Promise‹EncodedTransaction›*

___

###  getHashFromEncoded

▸ **getHashFromEncoded**(`rlpEncode`: string): *string*

*Defined in [packages/contractkit/src/utils/signing-utils.ts:31](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/utils/signing-utils.ts#L31)*

**Parameters:**

Name | Type |
------ | ------ |
`rlpEncode` | string |

**Returns:** *string*

___

###  recoverMessageSigner

▸ **recoverMessageSigner**(`signingDataHex`: string, `signedData`: string): *string*

*Defined in [packages/contractkit/src/utils/signing-utils.ts:187](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/utils/signing-utils.ts#L187)*

**Parameters:**

Name | Type |
------ | ------ |
`signingDataHex` | string |
`signedData` | string |

**Returns:** *string*

___

###  recoverTransaction

▸ **recoverTransaction**(`rawTx`: string): *[Tx, string]*

*Defined in [packages/contractkit/src/utils/signing-utils.ts:155](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/utils/signing-utils.ts#L155)*

**Parameters:**

Name | Type |
------ | ------ |
`rawTx` | string |

**Returns:** *[Tx, string]*

___

###  rlpEncodedTx

▸ **rlpEncodedTx**(`tx`: Tx): *[RLPEncodedTx](../interfaces/_utils_signing_utils_.rlpencodedtx.md)*

*Defined in [packages/contractkit/src/utils/signing-utils.ts:69](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/utils/signing-utils.ts#L69)*

**Parameters:**

Name | Type |
------ | ------ |
`tx` | Tx |

**Returns:** *[RLPEncodedTx](../interfaces/_utils_signing_utils_.rlpencodedtx.md)*

___

###  verifyEIP712TypedDataSigner

▸ **verifyEIP712TypedDataSigner**(`typedData`: EIP712TypedData, `signedData`: string, `expectedAddress`: string): *boolean*

*Defined in [packages/contractkit/src/utils/signing-utils.ts:197](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/utils/signing-utils.ts#L197)*

**Parameters:**

Name | Type |
------ | ------ |
`typedData` | EIP712TypedData |
`signedData` | string |
`expectedAddress` | string |

**Returns:** *boolean*