# Class: NameAccessor

## Hierarchy

* [SingleSchema](_identity_offchain_schema_utils_.singleschema.md)‹[NameType](../modules/_identity_offchain_schemas_.md#nametype)›

  ↳ **NameAccessor**

## Index

### Constructors

* [constructor](_identity_offchain_schemas_.nameaccessor.md#constructor)

### Properties

* [dataPath](_identity_offchain_schemas_.nameaccessor.md#datapath)
* [type](_identity_offchain_schemas_.nameaccessor.md#type)
* [wrapper](_identity_offchain_schemas_.nameaccessor.md#wrapper)

### Methods

* [read](_identity_offchain_schemas_.nameaccessor.md#read)
* [write](_identity_offchain_schemas_.nameaccessor.md#write)

## Constructors

###  constructor

\+ **new NameAccessor**(`wrapper`: [OffchainDataWrapper](_identity_offchain_data_wrapper_.offchaindatawrapper.md)): *[NameAccessor](_identity_offchain_schemas_.nameaccessor.md)*

*Overrides [SingleSchema](_identity_offchain_schema_utils_.singleschema.md).[constructor](_identity_offchain_schema_utils_.singleschema.md#constructor)*

*Defined in [packages/contractkit/src/identity/offchain/schemas.ts:13](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/identity/offchain/schemas.ts#L13)*

**Parameters:**

Name | Type |
------ | ------ |
`wrapper` | [OffchainDataWrapper](_identity_offchain_data_wrapper_.offchaindatawrapper.md) |

**Returns:** *[NameAccessor](_identity_offchain_schemas_.nameaccessor.md)*

## Properties

###  dataPath

• **dataPath**: *string*

*Inherited from [SingleSchema](_identity_offchain_schema_utils_.singleschema.md).[dataPath](_identity_offchain_schema_utils_.singleschema.md#datapath)*

*Defined in [packages/contractkit/src/identity/offchain/schema-utils.ts:33](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/identity/offchain/schema-utils.ts#L33)*

___

###  type

• **type**: *Type‹[NameType](../modules/_identity_offchain_schemas_.md#nametype)›*

*Inherited from [SingleSchema](_identity_offchain_schema_utils_.singleschema.md).[type](_identity_offchain_schema_utils_.singleschema.md#type)*

*Defined in [packages/contractkit/src/identity/offchain/schema-utils.ts:32](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/identity/offchain/schema-utils.ts#L32)*

___

###  wrapper

• **wrapper**: *[OffchainDataWrapper](_identity_offchain_data_wrapper_.offchaindatawrapper.md)*

*Overrides [SingleSchema](_identity_offchain_schema_utils_.singleschema.md).[wrapper](_identity_offchain_schema_utils_.singleschema.md#wrapper)*

*Defined in [packages/contractkit/src/identity/offchain/schemas.ts:14](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/identity/offchain/schemas.ts#L14)*

## Methods

###  read

▸ **read**(`account`: string): *Promise‹[FailedTask](../interfaces/_identity_task_.failedtask.md)‹[IOffchainError](../interfaces/_identity_offchain_schema_utils_.ioffchainerror.md) | [InvalidDataError](../interfaces/_identity_offchain_schema_utils_.invaliddataerror.md)› | [OKTask](../interfaces/_identity_task_.oktask.md)‹T››*

*Inherited from [SingleSchema](_identity_offchain_schema_utils_.singleschema.md).[read](_identity_offchain_schema_utils_.singleschema.md#read)*

*Defined in [packages/contractkit/src/identity/offchain/schema-utils.ts:36](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/identity/offchain/schema-utils.ts#L36)*

**Parameters:**

Name | Type |
------ | ------ |
`account` | string |

**Returns:** *Promise‹[FailedTask](../interfaces/_identity_task_.failedtask.md)‹[IOffchainError](../interfaces/_identity_offchain_schema_utils_.ioffchainerror.md) | [InvalidDataError](../interfaces/_identity_offchain_schema_utils_.invaliddataerror.md)› | [OKTask](../interfaces/_identity_task_.oktask.md)‹T››*

___

###  write

▸ **write**(`data`: [NameType](../modules/_identity_offchain_schemas_.md#nametype)): *Promise‹void›*

*Inherited from [SingleSchema](_identity_offchain_schema_utils_.singleschema.md).[write](_identity_offchain_schema_utils_.singleschema.md#write)*

*Defined in [packages/contractkit/src/identity/offchain/schema-utils.ts:40](https://github.com/celo-org/celo-monorepo/blob/master/packages/contractkit/src/identity/offchain/schema-utils.ts#L40)*

**Parameters:**

Name | Type |
------ | ------ |
`data` | [NameType](../modules/_identity_offchain_schemas_.md#nametype) |

**Returns:** *Promise‹void›*