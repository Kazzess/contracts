# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [category_service/v1/model.proto](#category_service_v1_model-proto)
    - [Category](#category_service-v1-Category)
  
- [category_service/v1/category.proto](#category_service_v1_category-proto)
    - [CreateCategoryRequest](#category_service-v1-CreateCategoryRequest)
    - [CreateCategoryResponse](#category_service-v1-CreateCategoryResponse)
    - [SearchCategoryRequest](#category_service-v1-SearchCategoryRequest)
    - [SearchCategoryResponse](#category_service-v1-SearchCategoryResponse)
    - [UpdateCategoryRequest](#category_service-v1-UpdateCategoryRequest)
    - [UpdateCategoryResponse](#category_service-v1-UpdateCategoryResponse)
  
- [category_service/v1/service.proto](#category_service_v1_service-proto)
    - [CategoryService](#category_service-v1-CategoryService)
  
- [Scalar Value Types](#scalar-value-types)



<a name="category_service_v1_model-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## category_service/v1/model.proto



<a name="category_service-v1-Category"></a>

### Category



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| is_enabled | [bool](#bool) |  |  |
| created_at | [int64](#int64) |  |  |
| updated_at | [int64](#int64) |  |  |





 

 

 

 



<a name="category_service_v1_category-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## category_service/v1/category.proto



<a name="category_service-v1-CreateCategoryRequest"></a>

### CreateCategoryRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |






<a name="category_service-v1-CreateCategoryResponse"></a>

### CreateCategoryResponse







<a name="category_service-v1-SearchCategoryRequest"></a>

### SearchCategoryRequest







<a name="category_service-v1-SearchCategoryResponse"></a>

### SearchCategoryResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| category | [Category](#category_service-v1-Category) | repeated |  |






<a name="category_service-v1-UpdateCategoryRequest"></a>

### UpdateCategoryRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint64](#uint64) |  |  |
| name | [string](#string) |  |  |
| is_enabled | [bool](#bool) |  |  |






<a name="category_service-v1-UpdateCategoryResponse"></a>

### UpdateCategoryResponse






 

 

 

 



<a name="category_service_v1_service-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## category_service/v1/service.proto


 

 

 


<a name="category_service-v1-CategoryService"></a>

### CategoryService
CategoryService

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateCategory | [CreateCategoryRequest](#category_service-v1-CreateCategoryRequest) | [CreateCategoryResponse](#category_service-v1-CreateCategoryResponse) |  |
| UpdateCategory | [UpdateCategoryRequest](#category_service-v1-UpdateCategoryRequest) | [UpdateCategoryResponse](#category_service-v1-UpdateCategoryResponse) |  |
| SearchCategory | [SearchCategoryRequest](#category_service-v1-SearchCategoryRequest) | [SearchCategoryResponse](#category_service-v1-SearchCategoryResponse) |  |

 



## Scalar Value Types

| .proto Type | Notes | C++ | Java | Python | Go | C# | PHP | Ruby |
| ----------- | ----- | --- | ---- | ------ | -- | -- | --- | ---- |
| <a name="double" /> double |  | double | double | float | float64 | double | float | Float |
| <a name="float" /> float |  | float | float | float | float32 | float | float | Float |
| <a name="int32" /> int32 | Uses variable-length encoding. Inefficient for encoding negative numbers – if your field is likely to have negative values, use sint32 instead. | int32 | int | int | int32 | int | integer | Bignum or Fixnum (as required) |
| <a name="int64" /> int64 | Uses variable-length encoding. Inefficient for encoding negative numbers – if your field is likely to have negative values, use sint64 instead. | int64 | long | int/long | int64 | long | integer/string | Bignum |
| <a name="uint32" /> uint32 | Uses variable-length encoding. | uint32 | int | int/long | uint32 | uint | integer | Bignum or Fixnum (as required) |
| <a name="uint64" /> uint64 | Uses variable-length encoding. | uint64 | long | int/long | uint64 | ulong | integer/string | Bignum or Fixnum (as required) |
| <a name="sint32" /> sint32 | Uses variable-length encoding. Signed int value. These more efficiently encode negative numbers than regular int32s. | int32 | int | int | int32 | int | integer | Bignum or Fixnum (as required) |
| <a name="sint64" /> sint64 | Uses variable-length encoding. Signed int value. These more efficiently encode negative numbers than regular int64s. | int64 | long | int/long | int64 | long | integer/string | Bignum |
| <a name="fixed32" /> fixed32 | Always four bytes. More efficient than uint32 if values are often greater than 2^28. | uint32 | int | int | uint32 | uint | integer | Bignum or Fixnum (as required) |
| <a name="fixed64" /> fixed64 | Always eight bytes. More efficient than uint64 if values are often greater than 2^56. | uint64 | long | int/long | uint64 | ulong | integer/string | Bignum |
| <a name="sfixed32" /> sfixed32 | Always four bytes. | int32 | int | int | int32 | int | integer | Bignum or Fixnum (as required) |
| <a name="sfixed64" /> sfixed64 | Always eight bytes. | int64 | long | int/long | int64 | long | integer/string | Bignum |
| <a name="bool" /> bool |  | bool | boolean | boolean | bool | bool | boolean | TrueClass/FalseClass |
| <a name="string" /> string | A string must always contain UTF-8 encoded or 7-bit ASCII text. | string | String | str/unicode | string | string | string | String (UTF-8) |
| <a name="bytes" /> bytes | May contain any arbitrary sequence of bytes. | string | ByteString | str | []byte | ByteString | string | String (ASCII-8BIT) |

