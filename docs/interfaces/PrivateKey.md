# Interface: PrivateKey

[💗 Help the project](https://github.com/sponsors/panva)

Support from the community to continue maintaining and improving this module is welcome. If you find the module useful, please consider supporting the project by [becoming a sponsor](https://github.com/sponsors/panva).

***

Interface to pass an asymmetric private key and, optionally, its associated JWK Key ID to be
added as a `kid` JOSE Header Parameter.

## Properties

### key

• **key**: [`CryptoKey`](https://developer.mozilla.org/docs/Web/API/CryptoKey)

An asymmetric private CryptoKey.

Its algorithm must be compatible with a supported [JWS `alg` Algorithm](../type-aliases/JWSAlgorithm.md).

***

### \[modifyAssertion\]?

• `optional` **\[modifyAssertion\]**: [`ModifyAssertionFunction`](ModifyAssertionFunction.md)

Use to modify the JWT signed by this key right before it is signed.

#### See

[modifyAssertion](../variables/modifyAssertion.md)

***

### kid?

• `optional` **kid**: `string`

JWK Key ID to add to JOSE headers when this key is used. When not provided no `kid` (JWK Key
ID) will be added to the JOSE Header.
