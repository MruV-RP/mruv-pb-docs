# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [accounts/accounts.proto](#accounts/accounts.proto)
    - [LogInRequest](#mruv.LogInRequest)
    - [LogInResponse](#mruv.LogInResponse)
    - [RegisterAccountRequest](#mruv.RegisterAccountRequest)
    - [RegisterAccountResponse](#mruv.RegisterAccountResponse)
  
  
  
    - [MruVAccountsService](#mruv.MruVAccountsService)
  

- [accounts/accounts_model.proto](#accounts/accounts_model.proto)
    - [Account](#mruv.Account)
    - [AccountID](#mruv.AccountID)
  
  
  
  

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
  
  
  
    - [MruVGroupsService](#mruv.MruVGroupsService)
  

- [groups/groups_model.proto](#groups/groups_model.proto)
    - [Group](#mruv.Group)
    - [GroupID](#mruv.GroupID)
    - [Permission](#mruv.Permission)
    - [PermissionID](#mruv.PermissionID)
  
  
  
  

- [items/items.proto](#items/items.proto)
    - [GetContainerItemsRequest](#mruv.GetContainerItemsRequest)
    - [GetContainerItemsResponse](#mruv.GetContainerItemsResponse)
    - [GetContainerTypesRequest](#mruv.GetContainerTypesRequest)
    - [GetContainerTypesResponse](#mruv.GetContainerTypesResponse)
    - [GetContainersRequest](#mruv.GetContainersRequest)
    - [GetContainersResponse](#mruv.GetContainersResponse)
    - [GetItemTypesRequest](#mruv.GetItemTypesRequest)
    - [GetItemTypesResponse](#mruv.GetItemTypesResponse)
    - [GetItemsRequest](#mruv.GetItemsRequest)
    - [GetItemsResponse](#mruv.GetItemsResponse)
    - [GetNearestItemsRequest](#mruv.GetNearestItemsRequest)
    - [GetNearestItemsResponse](#mruv.GetNearestItemsResponse)
    - [PullItemRequest](#mruv.PullItemRequest)
    - [PutItemRequest](#mruv.PutItemRequest)
    - [PutItemResponse](#mruv.PutItemResponse)
    - [SortItemsRequest](#mruv.SortItemsRequest)
    - [SortItemsResponse](#mruv.SortItemsResponse)
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
  
    - [SortingMode](#mruv.SortingMode)
  
  
  

- [server/server.proto](#server/server.proto)
    - [RegisterServerRequest](#mruv.RegisterServerRequest)
    - [RegisterServerResponse](#mruv.RegisterServerResponse)
  
  
  
    - [MruVServerService](#mruv.MruVServerService)
  

- [server/server_model.proto](#server/server_model.proto)
    - [ServerID](#mruv.ServerID)
    - [ServerInfo](#mruv.ServerInfo)
    - [ServerStatus](#mruv.ServerStatus)
  
  
  
  

- [Scalar Value Types](#scalar-value-types)



<a name="accounts/accounts.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## accounts/accounts.proto



<a name="mruv.LogInRequest"></a>

### LogInRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| login | [string](#string) |  |  |
| password | [string](#string) |  |  |






<a name="mruv.LogInResponse"></a>

### LogInResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| success | [bool](#bool) |  |  |
| id | [AccountID](#mruv.AccountID) |  |  |






<a name="mruv.RegisterAccountRequest"></a>

### RegisterAccountRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| account | [Account](#mruv.Account) |  |  |
| password | [string](#string) |  |  |






<a name="mruv.RegisterAccountResponse"></a>

### RegisterAccountResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| success | [bool](#bool) |  |  |
| id | [AccountID](#mruv.AccountID) |  |  |





 

 

 


<a name="mruv.MruVAccountsService"></a>

### MruVAccountsService


| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| RegisterAccount | [RegisterAccountRequest](#mruv.RegisterAccountRequest) | [RegisterAccountResponse](#mruv.RegisterAccountResponse) |  |
| LogIn | [LogInRequest](#mruv.LogInRequest) | [LogInResponse](#mruv.LogInResponse) |  |
| GetAccount | [AccountID](#mruv.AccountID) | [Account](#mruv.Account) |  |

 



<a name="accounts/accounts_model.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## accounts/accounts_model.proto



<a name="mruv.Account"></a>

### Account



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [AccountID](#mruv.AccountID) |  |  |
| login | [string](#string) |  |  |
| nick | [string](#string) |  |  |
| email | [string](#string) |  |  |






<a name="mruv.AccountID"></a>

### AccountID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int64](#int64) |  |  |





 

 

 

 



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
| CreateCharacter | [Character](#mruv.Character) | [CharacterID](#mruv.CharacterID) | CRUD |
| GetCharacter | [CharacterID](#mruv.CharacterID) | [Character](#mruv.Character) |  |
| RemoveCharacter | [CharacterID](#mruv.CharacterID) | [CharacterID](#mruv.CharacterID) |  |
| PermanentCharacterKill | [CharacterID](#mruv.CharacterID) | [CharacterID](#mruv.CharacterID) | Deaths |
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
| id | [CharacterID](#mruv.CharacterID) |  |  |
| owner_id | [AccountID](#mruv.AccountID) |  |  |
| first_name | [string](#string) |  |  |
| second_name | [string](#string) |  |  |
| age | [uint32](#uint32) |  |  |
| sex | [uint32](#uint32) |  |  |
| position | [Position](#mruv.Position) |  |  |






<a name="mruv.CharacterID"></a>

### CharacterID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int64](#int64) |  |  |





 


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





 

 

 


<a name="mruv.MruVGroupsService"></a>

### MruVGroupsService


| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateGroup | [Group](#mruv.Group) | [GroupID](#mruv.GroupID) | CRUD |
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
| id | [GroupID](#mruv.GroupID) |  |  |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |
| permissions | [Permission](#mruv.Permission) | repeated |  |
| members | [AccountID](#mruv.AccountID) | repeated |  |






<a name="mruv.GroupID"></a>

### GroupID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int32](#int32) |  |  |






<a name="mruv.Permission"></a>

### Permission



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [PermissionID](#mruv.PermissionID) |  |  |
| name | [string](#string) |  |  |
| role | [string](#string) |  |  |






<a name="mruv.PermissionID"></a>

### PermissionID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int64](#int64) |  |  |





 

 

 

 



<a name="items/items.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## items/items.proto



<a name="mruv.GetContainerItemsRequest"></a>

### GetContainerItemsRequest
Request message for `MruVItemsService.GetContainerItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [ContainerID](#mruv.ContainerID) |  | ID of container with items. |
| limit | [uint32](#uint32) |  | Limit of the returned items. |






<a name="mruv.GetContainerItemsResponse"></a>

### GetContainerItemsResponse
Request message for `MruVItemsService.GetContainerItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| items | [InsideItem](#mruv.InsideItem) | repeated | List of items inside containers. |






<a name="mruv.GetContainerTypesRequest"></a>

### GetContainerTypesRequest
Request message for `MruVItemsService.GetContainerTypes`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [uint32](#uint32) |  | Limit of the returned container types. |






<a name="mruv.GetContainerTypesResponse"></a>

### GetContainerTypesResponse
Response message for `MruVItemsService.GetContainers`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_types | [ContainerType](#mruv.ContainerType) | repeated | List of container types. |






<a name="mruv.GetContainersRequest"></a>

### GetContainersRequest
Request message for `MruVItemsService.GetContainers`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [uint32](#uint32) |  | Limit of the returned containers. |






<a name="mruv.GetContainersResponse"></a>

### GetContainersResponse
Response message for `MruVItemsService.GetContainers`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| containers | [Container](#mruv.Container) | repeated | List of containers. |






<a name="mruv.GetItemTypesRequest"></a>

### GetItemTypesRequest
Request message for `MruVItemsService.GetItemTypes`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [uint32](#uint32) |  | Limit of the returned item types. |






<a name="mruv.GetItemTypesResponse"></a>

### GetItemTypesResponse
Response message for `MruVItemsService.GetItemTypes`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| item_types | [ItemType](#mruv.ItemType) | repeated | List of item types. |






<a name="mruv.GetItemsRequest"></a>

### GetItemsRequest
Request message for `MruVItemsService.GetItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [uint32](#uint32) |  | Limit of the returned items. |






<a name="mruv.GetItemsResponse"></a>

### GetItemsResponse
Response message for `MruVItemsService.GetItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| items | [Item](#mruv.Item) | repeated | List of items. |






<a name="mruv.GetNearestItemsRequest"></a>

### GetNearestItemsRequest
Request message for `MruVItemsService.GetNearestItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| position | [Position](#mruv.Position) |  | Position from which to calculate the distance |
| container_id | [ContainerID](#mruv.ContainerID) |  | ID of container that contains items. |
| distance_limit | [double](#double) |  | The distance over which the items are ignored. |






<a name="mruv.GetNearestItemsResponse"></a>

### GetNearestItemsResponse
Response message for `MruVItemsService.GetNearestItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| item | [InsideItem](#mruv.InsideItem) | repeated | List of items sorted from nearest to farthest. |






<a name="mruv.PullItemRequest"></a>

### PullItemRequest
Request message for `MruVItemsService.PullItem`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [ContainerID](#mruv.ContainerID) |  | ID of the container from which we pull out a item. |
| item_id | [ItemID](#mruv.ItemID) |  | ID of the item we want to pull out. That item must be inside the container. |






<a name="mruv.PutItemRequest"></a>

### PutItemRequest
Request message for `MruVItemsService.PutItem`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [ContainerID](#mruv.ContainerID) |  | ID of container where to put item. |
| item_id | [ItemID](#mruv.ItemID) |  | ID of item we wan to put in. |
| slot | [int32](#int32) |  | Position used for sorting items |






<a name="mruv.PutItemResponse"></a>

### PutItemResponse
Response message for `MruVItemsService.PutItem`


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| inside_item | [InsideItem](#mruv.InsideItem) |  | Container with items inside. |






<a name="mruv.SortItemsRequest"></a>

### SortItemsRequest
Request message for `MruVItemsService.SortItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [ContainerID](#mruv.ContainerID) |  | ID of the container which contain items. |
| sort_by | [SortingMode](#mruv.SortingMode) |  | Sorting mode. |






<a name="mruv.SortItemsResponse"></a>

### SortItemsResponse
Response message for `MruVItemsService.SortItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container | [Container](#mruv.Container) |  | Container with sorted items inside. |






<a name="mruv.UseItemRequest"></a>

### UseItemRequest
Request message for `MruVItemsService.UseItem`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| item_id | [ItemID](#mruv.ItemID) |  |  |






<a name="mruv.UseItemResponse"></a>

### UseItemResponse
Response message for `MruVItemsService.UseItem`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| success | [bool](#bool) |  | Is item usage was successful. |





 

 

 


<a name="mruv.MruVItemService"></a>

### MruVItemService
The MruV items service provides procedures for managing items and containers

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateItem | [Item](#mruv.Item) | [ItemID](#mruv.ItemID) | Create new item. |
| GetItem | [ItemID](#mruv.ItemID) | [Item](#mruv.Item) | Get item by id. |
| DeleteItem | [ItemID](#mruv.ItemID) | [ItemID](#mruv.ItemID) | Delete item by id. |
| GetItems | [GetItemsRequest](#mruv.GetItemsRequest) | [GetItemsResponse](#mruv.GetItemsResponse) | Gets all items. |
| CreateItemType | [ItemType](#mruv.ItemType) | [ItemTypeID](#mruv.ItemTypeID) | Create item type. |
| GetItemType | [ItemTypeID](#mruv.ItemTypeID) | [ItemType](#mruv.ItemType) | Get item type by id. |
| DeleteItemType | [ItemTypeID](#mruv.ItemTypeID) | [ItemTypeID](#mruv.ItemTypeID) | Delete item type by id. |
| GetItemTypes | [GetItemTypesRequest](#mruv.GetItemTypesRequest) | [GetItemTypesResponse](#mruv.GetItemTypesResponse) | Gets all item types. |
| CreateContainer | [Container](#mruv.Container) | [ContainerID](#mruv.ContainerID) | Create container. |
| GetContainer | [ContainerID](#mruv.ContainerID) | [Container](#mruv.Container) | Get container by id. |
| DeleteContainer | [ContainerID](#mruv.ContainerID) | [ContainerID](#mruv.ContainerID) | Delete container by id. |
| GetContainers | [GetContainersRequest](#mruv.GetContainersRequest) | [GetContainersResponse](#mruv.GetContainersResponse) | Get all containers. |
| CreateContainerType | [ContainerType](#mruv.ContainerType) | [ContainerTypeID](#mruv.ContainerTypeID) | Create container type. |
| GetContainerType | [ContainerTypeID](#mruv.ContainerTypeID) | [ContainerType](#mruv.ContainerType) | Get container type by id. |
| DeleteContainerType | [ContainerTypeID](#mruv.ContainerTypeID) | [ContainerTypeID](#mruv.ContainerTypeID) | Detele container type by id. |
| GetContainerTypes | [GetContainerTypesRequest](#mruv.GetContainerTypesRequest) | [GetContainerTypesResponse](#mruv.GetContainerTypesResponse) | Get all container types. |
| GetContainerItems | [GetContainerItemsRequest](#mruv.GetContainerItemsRequest) | [GetContainerItemsResponse](#mruv.GetContainerItemsResponse) | Get items inside a container. |
| PullItem | [PullItemRequest](#mruv.PullItemRequest) | [Item](#mruv.Item) | Pull item from container. |
| PutItem | [PutItemRequest](#mruv.PutItemRequest) | [PutItemResponse](#mruv.PutItemResponse) | Put item into container. |
| SortItems | [SortItemsRequest](#mruv.SortItemsRequest) | [SortItemsResponse](#mruv.SortItemsResponse) | Sort items inside container. This procedure change order of items inside container. |
| GetNearestItems | [GetNearestItemsRequest](#mruv.GetNearestItemsRequest) | [GetNearestItemsResponse](#mruv.GetNearestItemsResponse) | Retrieves from the container the list of items nearest to the given position. |
| UseItem | [UseItemRequest](#mruv.UseItemRequest) | [UseItemResponse](#mruv.UseItemResponse) | Trigger action associated with the item usage. |
| GetServiceStatus | [ServiceStatusRequest](#mruv.ServiceStatusRequest) | [ServiceStatusResponse](#mruv.ServiceStatusResponse) | Get service health status. |
| GetServiceVersion | [VersionRequest](#mruv.VersionRequest) | [VersionResponse](#mruv.VersionResponse) | Get service current version. |

 



<a name="items/items_model.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## items/items_model.proto



<a name="mruv.Container"></a>

### Container
Container data structure.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [ContainerID](#mruv.ContainerID) |  |  |
| type_id | [ContainerTypeID](#mruv.ContainerTypeID) |  | ID of an container type. |
| item_id | [ItemID](#mruv.ItemID) |  | ID of container item representing container. |
| items_inside | [uint32](#uint32) |  | Number of items inside container. |
| items | [InsideItem](#mruv.InsideItem) | repeated | List of items inside container. |






<a name="mruv.ContainerID"></a>

### ContainerID
Container ID.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.ContainerType"></a>

### ContainerType
Container type data structure.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [ContainerTypeID](#mruv.ContainerTypeID) |  |  |
| container_item_type_id | [ItemTypeID](#mruv.ItemTypeID) |  | ID of an item type. |
| max_number | [uint32](#uint32) |  | Max items in the container. |
| max_volume | [float](#float) |  | Max volume of items in the container. |
| max_weight | [float](#float) |  | Max weight of items in the container. |
| valid_item_types | [ItemTypeID](#mruv.ItemTypeID) | repeated |  |






<a name="mruv.ContainerTypeID"></a>

### ContainerTypeID
Container type ID.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.InsideItem"></a>

### InsideItem
Item inside container data structure.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [ContainerID](#mruv.ContainerID) |  | ID of container containing the item. |
| item_id | [ItemID](#mruv.ItemID) |  |  |
| item | [Item](#mruv.Item) |  |  |
| position | [int32](#int32) |  | Position representing order in container. In ascending manner. |






<a name="mruv.Item"></a>

### Item
Item data structure.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [ItemID](#mruv.ItemID) |  |  |
| item_type_id | [ItemTypeID](#mruv.ItemTypeID) |  | ID of an item type. |
| weight | [float](#float) |  | Current weight of the item. |
| volume | [float](#float) |  | Current volume of the item. |






<a name="mruv.ItemID"></a>

### ItemID
Item ID.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint64](#uint64) |  |  |






<a name="mruv.ItemType"></a>

### ItemType
Item type data structure


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [ItemTypeID](#mruv.ItemTypeID) |  |  |
| name | [string](#string) |  | Short name of item type. |
| description | [string](#string) |  | Description of item type. |
| base_weight | [float](#float) |  | Default weight of items created with that item type. |
| base_volume | [float](#float) |  | Default volume of items created with that item type. |
| model_name | [string](#string) |  | GTA V model name. |
| model_hash | [int32](#int32) |  | GTA V model hash. |






<a name="mruv.ItemTypeID"></a>

### ItemTypeID
Item type ID.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |





 


<a name="mruv.SortingMode"></a>

### SortingMode
Sorting modes for container items.

| Name | Number | Description |
| ---- | ------ | ----------- |
| UNKNOWN | 0 | undefined behaviour |
| WEIGHT_DESC | 1 | sort by weight descending |
| WEIGHT_ASC | 2 | sort by weight ascending |
| VOLUME_DESC | 3 | sort by volume descending |
| VOLUME_ASC | 4 | sort by volume ascending |


 

 

 



<a name="server/server.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## server/server.proto



<a name="mruv.RegisterServerRequest"></a>

### RegisterServerRequest
Request message for `MruVServerService`






<a name="mruv.RegisterServerResponse"></a>

### RegisterServerResponse
Response message for `MruVServerService`





 

 

 


<a name="mruv.MruVServerService"></a>

### MruVServerService
The MruV server service provides procedures for managing game platform server actions

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| RegisterServer | [RegisterServerRequest](#mruv.RegisterServerRequest) | [RegisterServerResponse](#mruv.RegisterServerResponse) | Register instance of server for further managing |
| GetServerStatus | [ServerID](#mruv.ServerID) | [ServerStatus](#mruv.ServerStatus) | Get game server status |

 



<a name="server/server_model.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## server/server_model.proto



<a name="mruv.ServerID"></a>

### ServerID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [int32](#int32) |  |  |






<a name="mruv.ServerInfo"></a>

### ServerInfo
Data that describe server


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  | Short name of the server |
| host | [string](#string) |  | Host (ip) of the server |
| port | [string](#string) |  | Port of the server |
| platform | [string](#string) |  | Platform, on which server is running |






<a name="mruv.ServerStatus"></a>

### ServerStatus
State of the server


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| active | [bool](#bool) |  | Is server active and working |
| players | [int32](#int32) |  | How many players are registered on that server |





 

 

 

 



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

