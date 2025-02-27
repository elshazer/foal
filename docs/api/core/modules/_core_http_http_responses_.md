[@foal/core](../README.md) > ["core/http/http-responses"](../modules/_core_http_http_responses_.md)

# External module: "core/http/http-responses"

## Index

### Classes

* [HttpResponse](../classes/_core_http_http_responses_.httpresponse.md)
* [HttpResponseBadRequest](../classes/_core_http_http_responses_.httpresponsebadrequest.md)
* [HttpResponseClientError](../classes/_core_http_http_responses_.httpresponseclienterror.md)
* [HttpResponseConflict](../classes/_core_http_http_responses_.httpresponseconflict.md)
* [HttpResponseCreated](../classes/_core_http_http_responses_.httpresponsecreated.md)
* [HttpResponseForbidden](../classes/_core_http_http_responses_.httpresponseforbidden.md)
* [HttpResponseInternalServerError](../classes/_core_http_http_responses_.httpresponseinternalservererror.md)
* [HttpResponseMethodNotAllowed](../classes/_core_http_http_responses_.httpresponsemethodnotallowed.md)
* [HttpResponseMovedPermanently](../classes/_core_http_http_responses_.httpresponsemovedpermanently.md)
* [HttpResponseNoContent](../classes/_core_http_http_responses_.httpresponsenocontent.md)
* [HttpResponseNotFound](../classes/_core_http_http_responses_.httpresponsenotfound.md)
* [HttpResponseNotImplemented](../classes/_core_http_http_responses_.httpresponsenotimplemented.md)
* [HttpResponseOK](../classes/_core_http_http_responses_.httpresponseok.md)
* [HttpResponseRedirect](../classes/_core_http_http_responses_.httpresponseredirect.md)
* [HttpResponseRedirection](../classes/_core_http_http_responses_.httpresponseredirection.md)
* [HttpResponseServerError](../classes/_core_http_http_responses_.httpresponseservererror.md)
* [HttpResponseSuccess](../classes/_core_http_http_responses_.httpresponsesuccess.md)
* [HttpResponseUnauthorized](../classes/_core_http_http_responses_.httpresponseunauthorized.md)

### Interfaces

* [CookieOptions](../interfaces/_core_http_http_responses_.cookieoptions.md)

### Functions

* [createHttpResponseFile](_core_http_http_responses_.md#createhttpresponsefile)
* [isHttpResponse](_core_http_http_responses_.md#ishttpresponse)
* [isHttpResponseBadRequest](_core_http_http_responses_.md#ishttpresponsebadrequest)
* [isHttpResponseClientError](_core_http_http_responses_.md#ishttpresponseclienterror)
* [isHttpResponseConflict](_core_http_http_responses_.md#ishttpresponseconflict)
* [isHttpResponseCreated](_core_http_http_responses_.md#ishttpresponsecreated)
* [isHttpResponseForbidden](_core_http_http_responses_.md#ishttpresponseforbidden)
* [isHttpResponseInternalServerError](_core_http_http_responses_.md#ishttpresponseinternalservererror)
* [isHttpResponseMethodNotAllowed](_core_http_http_responses_.md#ishttpresponsemethodnotallowed)
* [isHttpResponseMovedPermanently](_core_http_http_responses_.md#ishttpresponsemovedpermanently)
* [isHttpResponseNoContent](_core_http_http_responses_.md#ishttpresponsenocontent)
* [isHttpResponseNotFound](_core_http_http_responses_.md#ishttpresponsenotfound)
* [isHttpResponseNotImplemented](_core_http_http_responses_.md#ishttpresponsenotimplemented)
* [isHttpResponseOK](_core_http_http_responses_.md#ishttpresponseok)
* [isHttpResponseRedirect](_core_http_http_responses_.md#ishttpresponseredirect)
* [isHttpResponseRedirection](_core_http_http_responses_.md#ishttpresponseredirection)
* [isHttpResponseServerError](_core_http_http_responses_.md#ishttpresponseservererror)
* [isHttpResponseSuccess](_core_http_http_responses_.md#ishttpresponsesuccess)
* [isHttpResponseUnauthorized](_core_http_http_responses_.md#ishttpresponseunauthorized)

---

## Functions

<a id="createhttpresponsefile"></a>

###  createHttpResponseFile

▸ **createHttpResponseFile**(options: *`object`*): `Promise`<[HttpResponseOK](../classes/_core_http_http_responses_.httpresponseok.md)>

*Defined in [core/http/http-responses.ts:281](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L281)*

Create an HttpResponseOK whose content is the specified file. If returned in a controller, the server sends the file in streaming.

**Parameters:**

**options: `object`**

The options used to create the HttpResponseOK.

| Name | Type | Description |
| ------ | ------ | ------ |
| directory | `string` |  Directory where the file is located. |
| file | `string` |  Name of the file with its extension. If a path is given, only the basename is kept. |
| `Optional` filename | `undefined` \| `string` |
| `Optional` forceDownload | `undefined` \| `false` \| `true` |

**Returns:** `Promise`<[HttpResponseOK](../classes/_core_http_http_responses_.httpresponseok.md)>

___
<a id="ishttpresponse"></a>

###  isHttpResponse

▸ **isHttpResponse**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:171](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L171)*

Check if an object is an instance of HttpResponse.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponse. False otherwise.

___
<a id="ishttpresponsebadrequest"></a>

###  isHttpResponseBadRequest

▸ **isHttpResponseBadRequest**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:628](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L628)*

Check if an object is an instance of HttpResponseBadRequest.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseBadRequest.
False otherwise.

___
<a id="ishttpresponseclienterror"></a>

###  isHttpResponseClientError

▸ **isHttpResponseClientError**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:582](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L582)*

Check if an object is an instance of HttpResponseClientError.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseClientError.
False otherwise.

___
<a id="ishttpresponseconflict"></a>

###  isHttpResponseConflict

▸ **isHttpResponseConflict**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:856](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L856)*

Check if an object is an instance of HttpResponseConflict.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseConflict. False otherwise.

___
<a id="ishttpresponsecreated"></a>

###  isHttpResponseCreated

▸ **isHttpResponseCreated**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:352](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L352)*

Check if an object is an instance of HttpResponseCreated.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseCreated. False otherwise.

___
<a id="ishttpresponseforbidden"></a>

###  isHttpResponseForbidden

▸ **isHttpResponseForbidden**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:720](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L720)*

Check if an object is an instance of HttpResponseForbidden.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseForbidden. False otherwise.

___
<a id="ishttpresponseinternalservererror"></a>

###  isHttpResponseInternalServerError

▸ **isHttpResponseInternalServerError**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:943](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L943)*

Check if an object is an instance of HttpResponseInternalServerError.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of
HttpResponseInternalServerError. False otherwise.

___
<a id="ishttpresponsemethodnotallowed"></a>

###  isHttpResponseMethodNotAllowed

▸ **isHttpResponseMethodNotAllowed**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:811](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L811)*

Check if an object is an instance of HttpResponseMethodNotAllowed.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseMethodNotAllowed.
False otherwise.

___
<a id="ishttpresponsemovedpermanently"></a>

###  isHttpResponseMovedPermanently

▸ **isHttpResponseMovedPermanently**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:489](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L489)*

Check if an object is an instance of HttpResponseMovedPermanently.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an
instance of HttpResponseMovedPermanently. False otherwise.

___
<a id="ishttpresponsenocontent"></a>

###  isHttpResponseNoContent

▸ **isHttpResponseNoContent**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:396](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L396)*

Check if an object is an instance of HttpResponseNoContent.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseNoContent. False otherwise.

___
<a id="ishttpresponsenotfound"></a>

###  isHttpResponseNotFound

▸ **isHttpResponseNotFound**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:765](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L765)*

Check if an object is an instance of HttpResponseNotFound.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseNotFound. False otherwise.

___
<a id="ishttpresponsenotimplemented"></a>

###  isHttpResponseNotImplemented

▸ **isHttpResponseNotImplemented**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:989](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L989)*

Check if an object is an instance of HttpResponseNotImplemented.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseNotImplemented.
False otherwise.

___
<a id="ishttpresponseok"></a>

###  isHttpResponseOK

▸ **isHttpResponseOK**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:262](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L262)*

Check if an object is an instance of HttpResponseOK.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseOK. False otherwise.

___
<a id="ishttpresponseredirect"></a>

###  isHttpResponseRedirect

▸ **isHttpResponseRedirect**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:535](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L535)*

Check if an object is an instance of HttpResponseRedirect.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseRedirect. False otherwise.

___
<a id="ishttpresponseredirection"></a>

###  isHttpResponseRedirection

▸ **isHttpResponseRedirection**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:443](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L443)*

Check if an object is an instance of HttpResponseRedirection.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseRedirection.
False otherwise.

___
<a id="ishttpresponseservererror"></a>

###  isHttpResponseServerError

▸ **isHttpResponseServerError**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:897](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L897)*

Check if an object is an instance of HttpResponseServerError.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseServerError.
False otherwise.

___
<a id="ishttpresponsesuccess"></a>

###  isHttpResponseSuccess

▸ **isHttpResponseSuccess**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:217](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L217)*

Check if an object is an instance of HttpResponseSuccess.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseSuccess. False otherwise.

___
<a id="ishttpresponseunauthorized"></a>

###  isHttpResponseUnauthorized

▸ **isHttpResponseUnauthorized**(obj: *`any`*): `boolean`

*Defined in [core/http/http-responses.ts:675](https://github.com/FoalTS/foal/blob/cf326d07/packages/core/src/core/http/http-responses.ts#L675)*

Check if an object is an instance of HttpResponseUnauthorized.

This function is a help when you have several packages using @foal/core. Npm can install the package several times, which leads to duplicate class definitions. If this is the case, the keyword `instanceof` may return false while the object is an instance of the class. This function fixes this problem.

*__export__*: 

**Parameters:**

| Name | Type | Description |
| ------ | ------ | ------ |
| obj | `any` |  The object to check. |

**Returns:** `boolean`
- True if the error is an instance of HttpResponseUnauthorized.
False otherwise.

___

