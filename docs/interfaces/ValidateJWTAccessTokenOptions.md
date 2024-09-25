# Interface: ValidateJWTAccessTokenOptions

[💗 Help the project](https://github.com/sponsors/panva)

Support from the community to continue maintaining and improving this module is welcome. If you find the module useful, please consider supporting the project by [becoming a sponsor](https://github.com/sponsors/panva).

***

## Properties

### \[clockSkew\]?

• `optional` **\[clockSkew\]**: `number`

See [clockSkew](../variables/clockSkew.md).

***

### \[clockTolerance\]?

• `optional` **\[clockTolerance\]**: `number`

See [clockTolerance](../variables/clockTolerance.md).

***

### \[customFetch\]()?

• `optional` **\[customFetch\]**: (`input`, `init`?) => [`Promise`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Promise)\<[`Response`](https://developer.mozilla.org/docs/Web/API/Response)\>

See [customFetch](../variables/customFetch.md).

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `input` | `RequestInfo` \| [`URL`](https://developer.mozilla.org/docs/Web/API/URL) |
| `init`? | `RequestInit` |

#### Returns

[`Promise`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Promise)\<[`Response`](https://developer.mozilla.org/docs/Web/API/Response)\>

***

### \[jwksCache\]?

• `optional` **\[jwksCache\]**: [`JWKSCacheInput`](../type-aliases/JWKSCacheInput.md)

See [jwksCache](../variables/jwksCache.md).

***

### headers?

• `optional` **headers**: [`Record`](https://www.typescriptlang.org/docs/handbook/utility-types.html#recordkeys-type)\<`string`, `string`\> \| [`string`, `string`][] \| [`Headers`](https://developer.mozilla.org/docs/Web/API/Headers)

Headers to additionally send with the HTTP request(s) triggered by this function's invocation.

***

### requireDPoP?

• `optional` **requireDPoP**: `boolean`

Indicates whether DPoP use is required.

***

### signal?

• `optional` **signal**: [`AbortSignal`](https://developer.mozilla.org/docs/Web/API/AbortSignal) \| () => [`AbortSignal`](https://developer.mozilla.org/docs/Web/API/AbortSignal)

An AbortSignal instance, or a factory returning one, to abort the HTTP request(s) triggered by
this function's invocation.

#### Example

A 5000ms timeout AbortSignal for every request

```js
const signal = () => AbortSignal.timeout(5_000) // Note: AbortSignal.timeout may not yet be available in all runtimes.
```
