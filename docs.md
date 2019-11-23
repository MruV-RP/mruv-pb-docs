# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [characters/characters.proto](#characters/characters.proto)
    - [DeathStreamRequest](#mruv.DeathStreamRequest)
    - [DeathStreamResponse](#mruv.DeathStreamResponse)
  
  
  
    - [MruVCharactersService](#mruv.MruVCharactersService)
  

- [characters/characters_model.proto](#characters/characters_model.proto)
    - [Character](#mruv.Character)
    - [CharacterID](#mruv.CharacterID)
  
    - [DeathType](#mruv.DeathType)
  
  
  

- [common/health.proto](#common/health.proto)
    - [ServiceStatusRequest](#mruv.ServiceStatusRequest)
    - [ServiceStatusResponse](#mruv.ServiceStatusResponse)
    - [VersionRequest](#mruv.VersionRequest)
    - [VersionResponse](#mruv.VersionResponse)
  
  
  
  

- [common/spatial.proto](#common/spatial.proto)
    - [Position](#mruv.Position)
    - [Rotation](#mruv.Rotation)
  
  
  
  

- [groups/groups.proto](#groups/groups.proto)
    - [GetGroupsRequest](#mruv.GetGroupsRequest)
    - [GetGroupsResponse](#mruv.GetGroupsResponse)
    - [GroupID](#mruv.GroupID)
  
  
  
    - [MruVGroupsService](#mruv.MruVGroupsService)
  

- [groups/groups_model.proto](#groups/groups_model.proto)
    - [Group](#mruv.Group)
    - [Permission](#mruv.Permission)
    - [User](#mruv.User)
  
  
  
  

- [items/items.proto](#items/items.proto)
    - [GetContainerItemsResponse](#mruv.GetContainerItemsResponse)
    - [GetContainerTypesRequest](#mruv.GetContainerTypesRequest)
    - [GetContainersRequest](#mruv.GetContainersRequest)
    - [GetContainersResponse](#mruv.GetContainersResponse)
    - [GetItemTypesRequest](#mruv.GetItemTypesRequest)
    - [GetItemTypesResponse](#mruv.GetItemTypesResponse)
    - [GetItemsRequest](#mruv.GetItemsRequest)
    - [GetItemsResponse](#mruv.GetItemsResponse)
    - [GetNearestItemsRequest](#mruv.GetNearestItemsRequest)
    - [GetNearestItemsResponse](#mruv.GetNearestItemsResponse)
    - [PutItemRequest](#mruv.PutItemRequest)
    - [RemoveItemRequest](#mruv.RemoveItemRequest)
    - [SortItemsRequest](#mruv.SortItemsRequest)
    - [SortItemsResponse](#mruv.SortItemsResponse)
    - [TakeItemRequest](#mruv.TakeItemRequest)
    - [TakeItemResponse](#mruv.TakeItemResponse)
    - [UseItemRequest](#mruv.UseItemRequest)
    - [UseItemResponse](#mruv.UseItemResponse)
  
  
  
    - [MruVItemService](#mruv.MruVItemService)
  

- [items/items_model.proto](#items/items_model.proto)
    - [Container](#mruv.Container)
    - [ContainerID](#mruv.ContainerID)
    - [ContainerType](#mruv.ContainerType)
    - [ContainerTypeID](#mruv.ContainerTypeID)
    - [InsideItem](#mruv.InsideItem)
    - [Item](#mruv.Item)
    - [ItemID](#mruv.ItemID)
    - [ItemType](#mruv.ItemType)
    - [ItemTypeID](#mruv.ItemTypeID)
  
  
  
  

- [Scalar Value Types](#scalar-value-types)



<a name="characters/characters.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## characters/characters.proto



<a name="mruv.DeathStreamRequest"></a>

### DeathStreamRequest
requests &amp; response messages


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| death_types | [DeathType](#mruv.DeathType) | repeated |  |






<a name="mruv.DeathStreamResponse"></a>

### DeathStreamResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [Character](#mruv.Character) |  |  |
| death_type | [DeathType](#mruv.DeathType) |  |  |





 

 

 


<a name="mruv.MruVCharactersService"></a>

### MruVCharactersService


| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| Create | [Character](#mruv.Character) | [CharacterID](#mruv.CharacterID) | CRUD |
| Get | [CharacterID](#mruv.CharacterID) | [Character](#mruv.Character) |  |
| Update | [Character](#mruv.Character) | [CharacterID](#mruv.CharacterID) |  |
| Remove | [CharacterID](#mruv.CharacterID) | [CharacterID](#mruv.CharacterID) |  |
| KillCharacter | [CharacterID](#mruv.CharacterID) | [CharacterID](#mruv.CharacterID) | Deaths |
| DeathsStream | [DeathStreamRequest](#mruv.DeathStreamRequest) | [DeathStreamResponse](#mruv.DeathStreamResponse) stream |  |
| GetServiceStatus | [ServiceStatusRequest](#mruv.ServiceStatusRequest) | [ServiceStatusResponse](#mruv.ServiceStatusResponse) | Service status |
| GetServiceVersion | [VersionRequest](#mruv.VersionRequest) | [VersionResponse](#mruv.VersionResponse) |  |

 



<a name="characters/characters_model.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## characters/characters_model.proto



<a name="mruv.Character"></a>

### Character



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int32](#int32) |  |  |
| first_name | [string](#string) |  |  |
| second_name | [string](#string) |  |  |
| age | [uint32](#uint32) |  |  |
| sex | [uint32](#uint32) |  |  |






<a name="mruv.CharacterID"></a>

### CharacterID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int32](#int32) |  |  |





 


<a name="mruv.DeathType"></a>

### DeathType


| Name | Number | Description |
| ---- | ------ | ----------- |
| DEATH_TYPE_NONE | 0 |  |
| DEATH_TYPE_BW | 1 |  |
| DEATH_TYPE_BW_KILL | 2 |  |
| DEATH_TYPE_CK | 3 |  |


 

 

 



<a name="common/health.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## common/health.proto



<a name="mruv.ServiceStatusRequest"></a>

### ServiceStatusRequest







<a name="mruv.ServiceStatusResponse"></a>

### ServiceStatusResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| status | [string](#string) |  |  |






<a name="mruv.VersionRequest"></a>

### VersionRequest







<a name="mruv.VersionResponse"></a>

### VersionResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| version | [string](#string) |  |  |
| build_date | [string](#string) |  |  |
| commit | [string](#string) |  |  |
| os_arch | [string](#string) |  |  |





 

 

 

 



<a name="common/spatial.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## common/spatial.proto



<a name="mruv.Position"></a>

### Position



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| x | [double](#double) |  |  |
| y | [double](#double) |  |  |
| z | [double](#double) |  |  |






<a name="mruv.Rotation"></a>

### Rotation



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| rx | [double](#double) |  |  |
| ry | [double](#double) |  |  |
| rz | [double](#double) |  |  |





 

 

 

 



<a name="groups/groups.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## groups/groups.proto



<a name="mruv.GetGroupsRequest"></a>

### GetGroupsRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [int32](#int32) |  |  |






<a name="mruv.GetGroupsResponse"></a>

### GetGroupsResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| groups | [Group](#mruv.Group) | repeated |  |






<a name="mruv.GroupID"></a>

### GroupID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int32](#int32) |  |  |





 

 

 


<a name="mruv.MruVGroupsService"></a>

### MruVGroupsService


| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateGroup | [Group](#mruv.Group) | [GroupID](#mruv.GroupID) | CRUD items |
| GetGroup | [GroupID](#mruv.GroupID) | [Group](#mruv.Group) |  |
| UpdateGroup | [Group](#mruv.Group) | [GroupID](#mruv.GroupID) |  |
| DeleteGroup | [GroupID](#mruv.GroupID) | [GroupID](#mruv.GroupID) |  |
| GetGroups | [GetGroupsRequest](#mruv.GetGroupsRequest) | [GetGroupsResponse](#mruv.GetGroupsResponse) |  |
| GetServiceStatus | [ServiceStatusRequest](#mruv.ServiceStatusRequest) | [ServiceStatusResponse](#mruv.ServiceStatusResponse) | Service status |
| GetServiceVersion | [VersionRequest](#mruv.VersionRequest) | [VersionResponse](#mruv.VersionResponse) |  |

 



<a name="groups/groups_model.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## groups/groups_model.proto



<a name="mruv.Group"></a>

### Group



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int32](#int32) |  |  |
| permissions | [Permission](#mruv.Permission) | repeated |  |
| users | [User](#mruv.User) | repeated |  |






<a name="mruv.Permission"></a>

### Permission



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| role | [string](#string) |  |  |






<a name="mruv.User"></a>

### User



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int32](#int32) |  |  |
| name | [string](#string) |  |  |





 

 

 

 



<a name="items/items.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## items/items.proto



<a name="mruv.GetContainerItemsResponse"></a>

### GetContainerItemsResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| items | [Item](#mruv.Item) | repeated |  |






<a name="mruv.GetContainerTypesRequest"></a>

### GetContainerTypesRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [int32](#int32) |  |  |






<a name="mruv.GetContainersRequest"></a>

### GetContainersRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [int32](#int32) |  |  |






<a name="mruv.GetContainersResponse"></a>

### GetContainersResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| containers | [Container](#mruv.Container) | repeated |  |






<a name="mruv.GetItemTypesRequest"></a>

### GetItemTypesRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [int32](#int32) |  |  |






<a name="mruv.GetItemTypesResponse"></a>

### GetItemTypesResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| item_types | [ItemType](#mruv.ItemType) | repeated |  |






<a name="mruv.GetItemsRequest"></a>

### GetItemsRequest
Requests messages


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [int32](#int32) |  |  |






<a name="mruv.GetItemsResponse"></a>

### GetItemsResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| items | [Item](#mruv.Item) | repeated |  |






<a name="mruv.GetNearestItemsRequest"></a>

### GetNearestItemsRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player_position | [Position](#mruv.Position) |  |  |
| container_id | [ContainerID](#mruv.ContainerID) |  |  |






<a name="mruv.GetNearestItemsResponse"></a>

### GetNearestItemsResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| item | [InsideItem](#mruv.InsideItem) | repeated |  |






<a name="mruv.PutItemRequest"></a>

### PutItemRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [ContainerID](#mruv.ContainerID) |  |  |
| item_id | [ItemID](#mruv.ItemID) |  |  |
| slot | [int32](#int32) |  |  |






<a name="mruv.RemoveItemRequest"></a>

### RemoveItemRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [ContainerID](#mruv.ContainerID) |  |  |
| item_id | [ItemID](#mruv.ItemID) |  |  |






<a name="mruv.SortItemsRequest"></a>

### SortItemsRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [ContainerID](#mruv.ContainerID) |  |  |
| sort_by | [string](#string) |  |  |






<a name="mruv.SortItemsResponse"></a>

### SortItemsResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| items | [Item](#mruv.Item) | repeated |  |






<a name="mruv.TakeItemRequest"></a>

### TakeItemRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [ItemID](#mruv.ItemID) |  |  |






<a name="mruv.TakeItemResponse"></a>

### TakeItemResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| item | [Item](#mruv.Item) |  |  |






<a name="mruv.UseItemRequest"></a>

### UseItemRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| item_id | [ItemID](#mruv.ItemID) |  |  |






<a name="mruv.UseItemResponse"></a>

### UseItemResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| success | [bool](#bool) |  |  |





 

 

 


<a name="mruv.MruVItemService"></a>

### MruVItemService


| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateItem | [Item](#mruv.Item) | [ItemID](#mruv.ItemID) | CRUD items |
| GetItem | [ItemID](#mruv.ItemID) | [Item](#mruv.Item) |  |
| DeleteItem | [ItemID](#mruv.ItemID) | [ItemID](#mruv.ItemID) |  |
| GetItems | [GetItemsRequest](#mruv.GetItemsRequest) | [GetItemsResponse](#mruv.GetItemsResponse) |  |
| CreateItemType | [ItemType](#mruv.ItemType) | [ItemTypeID](#mruv.ItemTypeID) | CRUD itemsTypes |
| GetItemType | [ItemTypeID](#mruv.ItemTypeID) | [ItemType](#mruv.ItemType) |  |
| DeleteItemType | [ItemTypeID](#mruv.ItemTypeID) | [ItemTypeID](#mruv.ItemTypeID) |  |
| GetItemTypes | [GetItemTypesRequest](#mruv.GetItemTypesRequest) | [GetItemTypesResponse](#mruv.GetItemTypesResponse) |  |
| CreateContainer | [Container](#mruv.Container) | [ContainerID](#mruv.ContainerID) | CRUD containers |
| GetContainer | [ContainerID](#mruv.ContainerID) | [Container](#mruv.Container) |  |
| DeleteContainer | [ContainerID](#mruv.ContainerID) | [ContainerID](#mruv.ContainerID) |  |
| GetContainers | [GetContainersRequest](#mruv.GetContainersRequest) | [GetContainersResponse](#mruv.GetContainersResponse) |  |
| CreateContainerType | [ContainerType](#mruv.ContainerType) | [ContainerTypeID](#mruv.ContainerTypeID) | CRUD container types |
| GetContainerType | [ContainerTypeID](#mruv.ContainerTypeID) | [ContainerType](#mruv.ContainerType) |  |
| DeleteContainerType | [ContainerTypeID](#mruv.ContainerTypeID) | [ContainerID](#mruv.ContainerID) |  |
| GetContainerTypes | [GetContainerTypesRequest](#mruv.GetContainerTypesRequest) | [ContainerType](#mruv.ContainerType) stream |  |
| GetContainerItems | [ContainerID](#mruv.ContainerID) | [GetContainerItemsResponse](#mruv.GetContainerItemsResponse) | Container Methods |
| RemoveContainerItem | [RemoveItemRequest](#mruv.RemoveItemRequest) | [Item](#mruv.Item) |  |
| PutItem | [PutItemRequest](#mruv.PutItemRequest) | [ItemID](#mruv.ItemID) |  |
| SortItems | [SortItemsRequest](#mruv.SortItemsRequest) | [SortItemsResponse](#mruv.SortItemsResponse) | TODO: SortItemsStream |
| GetNearestItems | [GetNearestItemsRequest](#mruv.GetNearestItemsRequest) | [GetNearestItemsResponse](#mruv.GetNearestItemsResponse) | TODO: GetNearestItemsStream |
| UseItem | [UseItemRequest](#mruv.UseItemRequest) | [UseItemResponse](#mruv.UseItemResponse) |  |
| GetServiceStatus | [ServiceStatusRequest](#mruv.ServiceStatusRequest) | [ServiceStatusResponse](#mruv.ServiceStatusResponse) | Service status |
| GetServiceVersion | [VersionRequest](#mruv.VersionRequest) | [VersionResponse](#mruv.VersionResponse) |  |

 



<a name="items/items_model.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## items/items_model.proto



<a name="mruv.Container"></a>

### Container



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int32](#int32) |  |  |
| type_id | [int32](#int32) |  |  |
| item_id | [int64](#int64) |  |  |
| items_inside | [int32](#int32) |  |  |
| items | [InsideItem](#mruv.InsideItem) | repeated |  |






<a name="mruv.ContainerID"></a>

### ContainerID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int32](#int32) |  |  |






<a name="mruv.ContainerType"></a>

### ContainerType



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int32](#int32) |  |  |
| container_item_type_id | [int32](#int32) |  |  |
| max_number | [int32](#int32) |  |  |
| max_volume | [float](#float) |  |  |
| max_weight | [float](#float) |  |  |
| valid_item_types | [int32](#int32) | repeated |  |






<a name="mruv.ContainerTypeID"></a>

### ContainerTypeID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int32](#int32) |  |  |






<a name="mruv.InsideItem"></a>

### InsideItem



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [int32](#int32) |  |  |
| item_id | [int64](#int64) |  |  |
| position | [Position](#mruv.Position) |  |  |
| rotation | [Rotation](#mruv.Rotation) |  |  |






<a name="mruv.Item"></a>

### Item



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int64](#int64) |  |  |
| item_type_id | [int32](#int32) |  |  |
| weight | [float](#float) |  |  |
| volume | [float](#float) |  |  |






<a name="mruv.ItemID"></a>

### ItemID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int64](#int64) |  |  |






<a name="mruv.ItemType"></a>

### ItemType



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int32](#int32) |  |  |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |
| base_weight | [float](#float) |  |  |
| base_volume | [float](#float) |  |  |
| model_name | [string](#string) |  |  |
| model_hash | [int32](#int32) |  |  |






<a name="mruv.ItemTypeID"></a>

### ItemTypeID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int32](#int32) |  |  |





 

 

 

 



## Scalar Value Types

| .proto Type | Notes | C++ Type | Java Type | Python Type |
| ----------- | ----- | -------- | --------- | ----------- |
| <a name="double" /> double |  | double | double | float |
| <a name="float" /> float |  | float | float | float |
| <a name="int32" /> int32 | Uses variable-length encoding. Inefficient for encoding negative numbers – if your field is likely to have negative values, use sint32 instead. | int32 | int | int |
| <a name="int64" /> int64 | Uses variable-length encoding. Inefficient for encoding negative numbers – if your field is likely to have negative values, use sint64 instead. | int64 | long | int/long |
| <a name="uint32" /> uint32 | Uses variable-length encoding. | uint32 | int | int/long |
| <a name="uint64" /> uint64 | Uses variable-length encoding. | uint64 | long | int/long |
| <a name="sint32" /> sint32 | Uses variable-length encoding. Signed int value. These more efficiently encode negative numbers than regular int32s. | int32 | int | int |
| <a name="sint64" /> sint64 | Uses variable-length encoding. Signed int value. These more efficiently encode negative numbers than regular int64s. | int64 | long | int/long |
| <a name="fixed32" /> fixed32 | Always four bytes. More efficient than uint32 if values are often greater than 2^28. | uint32 | int | int |
| <a name="fixed64" /> fixed64 | Always eight bytes. More efficient than uint64 if values are often greater than 2^56. | uint64 | long | int/long |
| <a name="sfixed32" /> sfixed32 | Always four bytes. | int32 | int | int |
| <a name="sfixed64" /> sfixed64 | Always eight bytes. | int64 | long | int/long |
| <a name="bool" /> bool |  | bool | boolean | boolean |
| <a name="string" /> string | A string must always contain UTF-8 encoded or 7-bit ASCII text. | string | String | str/unicode |
| <a name="bytes" /> bytes | May contain any arbitrary sequence of bytes. | string | ByteString | str |

