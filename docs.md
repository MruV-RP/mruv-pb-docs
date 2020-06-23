# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [accounts/accounts.proto](#accounts/accounts.proto)
    - [Account](#mruv.Account)
    - [AccountID](#mruv.AccountID)
    - [GetAccountCharactersResponse](#mruv.GetAccountCharactersResponse)
    - [LogInRequest](#mruv.LogInRequest)
    - [LogInResponse](#mruv.LogInResponse)
    - [RegisterAccountRequest](#mruv.RegisterAccountRequest)
    - [RegisterAccountResponse](#mruv.RegisterAccountResponse)
  
  
  
    - [MruVAccountsService](#mruv.MruVAccountsService)
  

- [business/business.proto](#business/business.proto)
    - [AssignEstateRequest](#mruv.business.AssignEstateRequest)
    - [AssignEstateResponse](#mruv.business.AssignEstateResponse)
    - [AssignOwnerRequest](#mruv.business.AssignOwnerRequest)
    - [AssignOwnerResponse](#mruv.business.AssignOwnerResponse)
    - [Business](#mruv.business.Business)
    - [BuyBusinessRequest](#mruv.business.BuyBusinessRequest)
    - [BuyBusinessResponse](#mruv.business.BuyBusinessResponse)
    - [CreateBusinessRequest](#mruv.business.CreateBusinessRequest)
    - [CreateBusinessResponse](#mruv.business.CreateBusinessResponse)
    - [DeleteBusinessRequest](#mruv.business.DeleteBusinessRequest)
    - [DeleteBusinessResponse](#mruv.business.DeleteBusinessResponse)
    - [GetBusinessRequest](#mruv.business.GetBusinessRequest)
    - [GetBusinessResponse](#mruv.business.GetBusinessResponse)
    - [UnassignEstateRequest](#mruv.business.UnassignEstateRequest)
    - [UnassignEstateResponse](#mruv.business.UnassignEstateResponse)
    - [UpdateBusinessRequest](#mruv.business.UpdateBusinessRequest)
    - [UpdateBusinessResponse](#mruv.business.UpdateBusinessResponse)
    - [WatchBusinessRequest](#mruv.business.WatchBusinessRequest)
    - [WatchBusinessResponse](#mruv.business.WatchBusinessResponse)
    - [WatchBusinessesRequest](#mruv.business.WatchBusinessesRequest)
    - [WatchBusinessesResponse](#mruv.business.WatchBusinessesResponse)
  
    - [OwnerType](#mruv.business.OwnerType)
  
  
    - [MruVBusinessService](#mruv.business.MruVBusinessService)
  

- [characters/characters.proto](#characters/characters.proto)
    - [Character](#mruv.Character)
    - [CharacterID](#mruv.CharacterID)
    - [CreateCharacterRequest](#mruv.CreateCharacterRequest)
    - [CreateCharacterResponse](#mruv.CreateCharacterResponse)
    - [DeathStreamRequest](#mruv.DeathStreamRequest)
    - [DeathStreamResponse](#mruv.DeathStreamResponse)
    - [DeleteCharacterRequest](#mruv.DeleteCharacterRequest)
    - [DeleteCharacterResponse](#mruv.DeleteCharacterResponse)
    - [GetCharacterRequest](#mruv.GetCharacterRequest)
    - [GetCharacterResponse](#mruv.GetCharacterResponse)
    - [UpdateCharacterRequest](#mruv.UpdateCharacterRequest)
    - [UpdateCharacterResponse](#mruv.UpdateCharacterResponse)
  
    - [DeathType](#mruv.DeathType)
  
  
    - [MruVCharactersService](#mruv.MruVCharactersService)
  

- [common/health.proto](#common/health.proto)
    - [ServiceStatusRequest](#mruv.ServiceStatusRequest)
    - [ServiceStatusResponse](#mruv.ServiceStatusResponse)
    - [VersionRequest](#mruv.VersionRequest)
    - [VersionResponse](#mruv.VersionResponse)
  
  
  
  

- [common/spatial.proto](#common/spatial.proto)
    - [Position](#mruv.Position)
    - [Rotation](#mruv.Rotation)
  
  
  
  

- [devtools/devtools.proto](#devtools/devtools.proto)
    - [DeletePositionRequest](#mruv.devtools.DeletePositionRequest)
    - [DeletePositionResponse](#mruv.devtools.DeletePositionResponse)
    - [GetAnimationRequest](#mruv.devtools.GetAnimationRequest)
    - [GetAnimationResponse](#mruv.devtools.GetAnimationResponse)
    - [GetAnimationsRequest](#mruv.devtools.GetAnimationsRequest)
    - [GetAnimationsResponse](#mruv.devtools.GetAnimationsResponse)
    - [GetAnimationsResponse.Row](#mruv.devtools.GetAnimationsResponse.Row)
    - [GetOutfitsRequest](#mruv.devtools.GetOutfitsRequest)
    - [GetOutfitsResponse](#mruv.devtools.GetOutfitsResponse)
    - [GetOutfitsResponse.Row](#mruv.devtools.GetOutfitsResponse.Row)
    - [GetPositionsRequest](#mruv.devtools.GetPositionsRequest)
    - [GetPositionsResponse](#mruv.devtools.GetPositionsResponse)
    - [GetPositionsResponse.Row](#mruv.devtools.GetPositionsResponse.Row)
    - [SaveAnimationRequest](#mruv.devtools.SaveAnimationRequest)
    - [SaveAnimationResponse](#mruv.devtools.SaveAnimationResponse)
    - [SaveOutfitRequest](#mruv.devtools.SaveOutfitRequest)
    - [SaveOutfitResponse](#mruv.devtools.SaveOutfitResponse)
    - [SavePositionRequest](#mruv.devtools.SavePositionRequest)
    - [SavePositionResponse](#mruv.devtools.SavePositionResponse)
  
  
  
    - [MruVDevToolsService](#mruv.devtools.MruVDevToolsService)
  

- [devtools/devtools_model.proto](#devtools/devtools_model.proto)
    - [Animation](#mruv.devtools.Animation)
    - [Outfit](#mruv.devtools.Outfit)
    - [Player](#mruv.devtools.Player)
    - [Position](#mruv.devtools.Position)
  
  
  
  

- [economy/economy.proto](#economy/economy.proto)
    - [BuyProductRequest](#mruv.economy.BuyProductRequest)
    - [BuyProductResponse](#mruv.economy.BuyProductResponse)
    - [DeleteProductRequest](#mruv.economy.DeleteProductRequest)
    - [DeleteProductResponse](#mruv.economy.DeleteProductResponse)
    - [GetPriceRequest](#mruv.economy.GetPriceRequest)
    - [GetPriceResponse](#mruv.economy.GetPriceResponse)
    - [GetProductRequest](#mruv.economy.GetProductRequest)
    - [GetProductResponse](#mruv.economy.GetProductResponse)
    - [RegisterProductRequest](#mruv.economy.RegisterProductRequest)
    - [RegisterProductResponse](#mruv.economy.RegisterProductResponse)
    - [UpdatePriceRequest](#mruv.economy.UpdatePriceRequest)
    - [UpdatePriceResponse](#mruv.economy.UpdatePriceResponse)
    - [UpdateProductRequest](#mruv.economy.UpdateProductRequest)
    - [UpdateProductResponse](#mruv.economy.UpdateProductResponse)
    - [WatchPriceRequest](#mruv.economy.WatchPriceRequest)
    - [WatchPriceResponse](#mruv.economy.WatchPriceResponse)
    - [WatchProductRequest](#mruv.economy.WatchProductRequest)
    - [WatchProductResponse](#mruv.economy.WatchProductResponse)
  
    - [WatchProductResponse.ProductEvent](#mruv.economy.WatchProductResponse.ProductEvent)
  
  
    - [MruVEconomyService](#mruv.economy.MruVEconomyService)
  

- [estates/elevators.proto](#estates/elevators.proto)
    - [CreateElevatorRequest](#mruv.elevators.CreateElevatorRequest)
    - [CreateElevatorResponse](#mruv.elevators.CreateElevatorResponse)
    - [DeleteElevatorRequest](#mruv.elevators.DeleteElevatorRequest)
    - [DeleteElevatorResponse](#mruv.elevators.DeleteElevatorResponse)
    - [GetElevatorFloorsRequest](#mruv.elevators.GetElevatorFloorsRequest)
    - [GetElevatorFloorsResponse](#mruv.elevators.GetElevatorFloorsResponse)
    - [GetElevatorRequest](#mruv.elevators.GetElevatorRequest)
    - [GetElevatorResponse](#mruv.elevators.GetElevatorResponse)
    - [UpdateElevatorRequest](#mruv.elevators.UpdateElevatorRequest)
    - [UpdateElevatorResponse](#mruv.elevators.UpdateElevatorResponse)
  
  
  
    - [MruVElevatorsService](#mruv.elevators.MruVElevatorsService)
  

- [estates/entrances.proto](#estates/entrances.proto)
    - [CreateEntranceRequest](#mruv.entrances.CreateEntranceRequest)
    - [CreateEntranceResponse](#mruv.entrances.CreateEntranceResponse)
    - [DeleteEntranceRequest](#mruv.entrances.DeleteEntranceRequest)
    - [DeleteEntranceResponse](#mruv.entrances.DeleteEntranceResponse)
    - [EnterRequest](#mruv.entrances.EnterRequest)
    - [EnterResponse](#mruv.entrances.EnterResponse)
    - [Entrance](#mruv.entrances.Entrance)
    - [Entrance.EntranceDoor](#mruv.entrances.Entrance.EntranceDoor)
    - [FindNearestEntranceRequest](#mruv.entrances.FindNearestEntranceRequest)
    - [FindNearestEntranceResponse](#mruv.entrances.FindNearestEntranceResponse)
    - [GetEntranceRequest](#mruv.entrances.GetEntranceRequest)
    - [GetEntranceResponse](#mruv.entrances.GetEntranceResponse)
    - [LockRequest](#mruv.entrances.LockRequest)
    - [LockResponse](#mruv.entrances.LockResponse)
    - [UnlockRequest](#mruv.entrances.UnlockRequest)
    - [UnlockResponse](#mruv.entrances.UnlockResponse)
    - [UpdateEntranceRequest](#mruv.entrances.UpdateEntranceRequest)
    - [UpdateEntranceResponse](#mruv.entrances.UpdateEntranceResponse)
  
  
  
    - [MruVEntrancesService](#mruv.entrances.MruVEntrancesService)
  

- [estates/estates.proto](#estates/estates.proto)
    - [AddEntranceRequest](#mruv.estates.AddEntranceRequest)
    - [AddEntranceResponse](#mruv.estates.AddEntranceResponse)
    - [AddGateRequest](#mruv.estates.AddGateRequest)
    - [AddGateResponse](#mruv.estates.AddGateResponse)
    - [CreateEstateRequest](#mruv.estates.CreateEstateRequest)
    - [CreateEstateResponse](#mruv.estates.CreateEstateResponse)
    - [DeleteEstateRequest](#mruv.estates.DeleteEstateRequest)
    - [DeleteEstateResponse](#mruv.estates.DeleteEstateResponse)
    - [DeleteGateRequest](#mruv.estates.DeleteGateRequest)
    - [DeleteGateResponse](#mruv.estates.DeleteGateResponse)
    - [Estate](#mruv.estates.Estate)
    - [GetEstateEntrancesRequest](#mruv.estates.GetEstateEntrancesRequest)
    - [GetEstateEntrancesResponse](#mruv.estates.GetEstateEntrancesResponse)
    - [GetEstateGatesRequest](#mruv.estates.GetEstateGatesRequest)
    - [GetEstateGatesResponse](#mruv.estates.GetEstateGatesResponse)
    - [GetEstateRequest](#mruv.estates.GetEstateRequest)
    - [GetEstatesRequest](#mruv.estates.GetEstatesRequest)
    - [GetEstatesResponse](#mruv.estates.GetEstatesResponse)
    - [RemoveEntranceRequest](#mruv.estates.RemoveEntranceRequest)
    - [RemoveEntranceResponse](#mruv.estates.RemoveEntranceResponse)
    - [UpdateEstateRequest](#mruv.estates.UpdateEstateRequest)
    - [UpdateEstateResponse](#mruv.estates.UpdateEstateResponse)
  
  
  
    - [MruVEstateService](#mruv.estates.MruVEstateService)
  

- [estates/gates.proto](#estates/gates.proto)
    - [CloseRequest](#mruv.gates.CloseRequest)
    - [CloseResponse](#mruv.gates.CloseResponse)
    - [CreateGateRequest](#mruv.gates.CreateGateRequest)
    - [CreateGateResponse](#mruv.gates.CreateGateResponse)
    - [DeleteGateRequest](#mruv.gates.DeleteGateRequest)
    - [DeleteGateResponse](#mruv.gates.DeleteGateResponse)
    - [FindNearestGateRequest](#mruv.gates.FindNearestGateRequest)
    - [FindNearestGateResponse](#mruv.gates.FindNearestGateResponse)
    - [Gate](#mruv.gates.Gate)
    - [GetGateRequest](#mruv.gates.GetGateRequest)
    - [GetGateResponse](#mruv.gates.GetGateResponse)
    - [LockRequest](#mruv.gates.LockRequest)
    - [LockResponse](#mruv.gates.LockResponse)
    - [OpenRequest](#mruv.gates.OpenRequest)
    - [OpenResponse](#mruv.gates.OpenResponse)
    - [UnlockRequest](#mruv.gates.UnlockRequest)
    - [UnlockResponse](#mruv.gates.UnlockResponse)
    - [UpdateGateRequest](#mruv.gates.UpdateGateRequest)
    - [UpdateGateResponse](#mruv.gates.UpdateGateResponse)
  
  
  
    - [MruVGatesService](#mruv.gates.MruVGatesService)
  

- [groups/groups.proto](#groups/groups.proto)
    - [AddGroupMemberRequest](#mruv.AddGroupMemberRequest)
    - [AddGroupMemberResponse](#mruv.AddGroupMemberResponse)
    - [GetGroupsRequest](#mruv.GetGroupsRequest)
    - [GetGroupsResponse](#mruv.GetGroupsResponse)
    - [Group](#mruv.Group)
    - [GroupID](#mruv.GroupID)
    - [Permission](#mruv.Permission)
    - [PermissionID](#mruv.PermissionID)
    - [RemoveGroupMemberRequest](#mruv.RemoveGroupMemberRequest)
    - [RemoveGroupMemberResponse](#mruv.RemoveGroupMemberResponse)
  
  
  
    - [MruVGroupsService](#mruv.MruVGroupsService)
  

- [houses/houses.proto](#houses/houses.proto)
    - [CreateHouseRequest](#mruv.houses.CreateHouseRequest)
    - [CreateHouseResponse](#mruv.houses.CreateHouseResponse)
    - [DeleteHouseRequest](#mruv.houses.DeleteHouseRequest)
    - [DeleteHouseResponse](#mruv.houses.DeleteHouseResponse)
    - [GetHouseRequest](#mruv.houses.GetHouseRequest)
    - [GetHouseResponse](#mruv.houses.GetHouseResponse)
    - [UpdateHouseRequest](#mruv.houses.UpdateHouseRequest)
    - [UpdateHouseResponse](#mruv.houses.UpdateHouseResponse)
  
  
  
    - [MruVHousesService](#mruv.houses.MruVHousesService)
  

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
  
  
  

- [jobs/jobs.proto](#jobs/jobs.proto)
    - [CreateJobRequest](#mruv.jobs.CreateJobRequest)
    - [CreateJobResponse](#mruv.jobs.CreateJobResponse)
    - [DeleteJobRequest](#mruv.jobs.DeleteJobRequest)
    - [DeleteJobResponse](#mruv.jobs.DeleteJobResponse)
    - [GetJobRequest](#mruv.jobs.GetJobRequest)
    - [GetJobResponse](#mruv.jobs.GetJobResponse)
    - [UpdateJobRequest](#mruv.jobs.UpdateJobRequest)
    - [UpdateJobResponse](#mruv.jobs.UpdateJobResponse)
  
  
  
    - [MruVJobsService](#mruv.jobs.MruVJobsService)
  

- [offers/offers.proto](#offers/offers.proto)
    - [AcceptOfferRequest](#mruv.offers.AcceptOfferRequest)
    - [AcceptOfferResponse](#mruv.offers.AcceptOfferResponse)
    - [CreateOfferRequest](#mruv.offers.CreateOfferRequest)
    - [CreateOfferResponse](#mruv.offers.CreateOfferResponse)
    - [DeleteOfferRequest](#mruv.offers.DeleteOfferRequest)
    - [DeleteOfferResponse](#mruv.offers.DeleteOfferResponse)
    - [GetOfferRequest](#mruv.offers.GetOfferRequest)
    - [GetOfferResponse](#mruv.offers.GetOfferResponse)
    - [UpdateOfferRequest](#mruv.offers.UpdateOfferRequest)
    - [UpdateOfferResponse](#mruv.offers.UpdateOfferResponse)
  
    - [OfferType](#mruv.offers.OfferType)
  
  
    - [MruVOffersService](#mruv.offers.MruVOffersService)
  

- [organizations/organizations.proto](#organizations/organizations.proto)
    - [AssignLeaderRequest](#mruv.organizations.AssignLeaderRequest)
    - [AssignLeaderResponse](#mruv.organizations.AssignLeaderResponse)
    - [CreateOrganizationRequest](#mruv.organizations.CreateOrganizationRequest)
    - [CreateOrganizationResponse](#mruv.organizations.CreateOrganizationResponse)
    - [DeleteOrganizationRequest](#mruv.organizations.DeleteOrganizationRequest)
    - [DeleteOrganizationResponse](#mruv.organizations.DeleteOrganizationResponse)
    - [GetOrganizationRequest](#mruv.organizations.GetOrganizationRequest)
    - [GetOrganizationResponse](#mruv.organizations.GetOrganizationResponse)
    - [UnassignLeaderRequest](#mruv.organizations.UnassignLeaderRequest)
    - [UnassignLeaderResponse](#mruv.organizations.UnassignLeaderResponse)
    - [UpdateOrganizationRequest](#mruv.organizations.UpdateOrganizationRequest)
    - [UpdateOrganizationResponse](#mruv.organizations.UpdateOrganizationResponse)
  
  
  
    - [MruVOrganizationsService](#mruv.organizations.MruVOrganizationsService)
  

- [punishments/punishments.proto](#punishments/punishments.proto)
    - [AdminJailMessage](#mruv.economy.AdminJailMessage)
    - [AdminJailRequest](#mruv.economy.AdminJailRequest)
    - [AdminJailResponse](#mruv.economy.AdminJailResponse)
    - [BanMessage](#mruv.economy.BanMessage)
    - [BanRequest](#mruv.economy.BanRequest)
    - [BanResponse](#mruv.economy.BanResponse)
    - [BlockMessage](#mruv.economy.BlockMessage)
    - [BlockRequest](#mruv.economy.BlockRequest)
    - [BlockResponse](#mruv.economy.BlockResponse)
    - [GetBanRequest](#mruv.economy.GetBanRequest)
    - [GetBlockRequest](#mruv.economy.GetBlockRequest)
    - [GetPlayerAdminJailRequest](#mruv.economy.GetPlayerAdminJailRequest)
    - [GetPlayerAdminJailResponse](#mruv.economy.GetPlayerAdminJailResponse)
    - [GetPlayerBansRequest](#mruv.economy.GetPlayerBansRequest)
    - [GetPlayerBansResponse](#mruv.economy.GetPlayerBansResponse)
    - [GetPlayerWarnsRequest](#mruv.economy.GetPlayerWarnsRequest)
    - [GetPlayerWarnsResponse](#mruv.economy.GetPlayerWarnsResponse)
    - [GetWarnRequest](#mruv.economy.GetWarnRequest)
    - [IsCharacterBlockedRequest](#mruv.economy.IsCharacterBlockedRequest)
    - [IsCharacterBlockedResponse](#mruv.economy.IsCharacterBlockedResponse)
    - [IsCharacterJailedRequest](#mruv.economy.IsCharacterJailedRequest)
    - [IsCharacterJailedResponse](#mruv.economy.IsCharacterJailedResponse)
    - [IsPlayerBannedRequest](#mruv.economy.IsPlayerBannedRequest)
    - [IsPlayerBannedResponse](#mruv.economy.IsPlayerBannedResponse)
    - [MuteGlobalChatsRequest](#mruv.economy.MuteGlobalChatsRequest)
    - [MuteGlobalChatsResponse](#mruv.economy.MuteGlobalChatsResponse)
    - [UnAdminJailMessage](#mruv.economy.UnAdminJailMessage)
    - [UnAdminJailRequest](#mruv.economy.UnAdminJailRequest)
    - [UnAdminJailResponse](#mruv.economy.UnAdminJailResponse)
    - [UnBanMessage](#mruv.economy.UnBanMessage)
    - [UnBanRequest](#mruv.economy.UnBanRequest)
    - [UnBanResponse](#mruv.economy.UnBanResponse)
    - [UnBlockMessage](#mruv.economy.UnBlockMessage)
    - [UnMuteGlobalChatsRequest](#mruv.economy.UnMuteGlobalChatsRequest)
    - [UnMuteGlobalChatsResponse](#mruv.economy.UnMuteGlobalChatsResponse)
    - [UnWarnMessage](#mruv.economy.UnWarnMessage)
    - [UnWarnRequest](#mruv.economy.UnWarnRequest)
    - [UnWarnResponse](#mruv.economy.UnWarnResponse)
    - [WarnMessage](#mruv.economy.WarnMessage)
    - [WarnRequest](#mruv.economy.WarnRequest)
    - [WarnResponse](#mruv.economy.WarnResponse)
    - [WatchAdminJailsRequest](#mruv.economy.WatchAdminJailsRequest)
    - [WatchBansRequest](#mruv.economy.WatchBansRequest)
    - [WatchBlocksRequest](#mruv.economy.WatchBlocksRequest)
    - [WatchPlayerAcquittalsRequest](#mruv.economy.WatchPlayerAcquittalsRequest)
    - [WatchPlayerAcquittalsResponse](#mruv.economy.WatchPlayerAcquittalsResponse)
    - [WatchPlayerPunishmentsRequest](#mruv.economy.WatchPlayerPunishmentsRequest)
    - [WatchPlayerPunishmentsResponse](#mruv.economy.WatchPlayerPunishmentsResponse)
    - [WatchPunishmentsRequest](#mruv.economy.WatchPunishmentsRequest)
    - [WatchPunishmentsResponse](#mruv.economy.WatchPunishmentsResponse)
    - [WatchUnAdminJailsRequest](#mruv.economy.WatchUnAdminJailsRequest)
    - [WatchUnBansRequest](#mruv.economy.WatchUnBansRequest)
    - [WatchUnBlocksRequest](#mruv.economy.WatchUnBlocksRequest)
    - [WatchUnWarnsRequest](#mruv.economy.WatchUnWarnsRequest)
    - [WatchWarnsRequest](#mruv.economy.WatchWarnsRequest)
  
    - [AcquittalsType](#mruv.economy.AcquittalsType)
    - [PunishmentType](#mruv.economy.PunishmentType)
  
  
    - [MruVPunishmentsService](#mruv.economy.MruVPunishmentsService)
  

- [server/server.proto](#server/server.proto)
    - [GetRegisteredServersRequest](#mruv.server.GetRegisteredServersRequest)
    - [GetRegisteredServersResponse](#mruv.server.GetRegisteredServersResponse)
    - [ServerEvent](#mruv.server.ServerEvent)
    - [ServerEventsStreamRequest](#mruv.server.ServerEventsStreamRequest)
    - [UpdateServerStatusRequest](#mruv.server.UpdateServerStatusRequest)
    - [UpdateServerStatusResponse](#mruv.server.UpdateServerStatusResponse)
  
    - [ServerEvent.ServerEventType](#mruv.server.ServerEvent.ServerEventType)
  
  
    - [MruVServerService](#mruv.server.MruVServerService)
  

- [server/server_model.proto](#server/server_model.proto)
    - [ServerID](#mruv.server.ServerID)
    - [ServerInfo](#mruv.server.ServerInfo)
  
    - [ServerStatus](#mruv.server.ServerStatus)
  
  
  

- [vehicles/vehicles.proto](#vehicles/vehicles.proto)
    - [CreateVehicleRequest](#mruv.vehicles.CreateVehicleRequest)
    - [CreateVehicleResponse](#mruv.vehicles.CreateVehicleResponse)
    - [DeleteVehicleRequest](#mruv.vehicles.DeleteVehicleRequest)
    - [DeleteVehicleResponse](#mruv.vehicles.DeleteVehicleResponse)
    - [GetVehicleRequest](#mruv.vehicles.GetVehicleRequest)
    - [GetVehicleResponse](#mruv.vehicles.GetVehicleResponse)
    - [UpdateVehicleRequest](#mruv.vehicles.UpdateVehicleRequest)
    - [UpdateVehicleResponse](#mruv.vehicles.UpdateVehicleResponse)
  
  
  
    - [MruVVehiclesService](#mruv.vehicles.MruVVehiclesService)
  

- [Scalar Value Types](#scalar-value-types)



<a name="accounts/accounts.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## accounts/accounts.proto



<a name="mruv.Account"></a>

### Account



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| login | [string](#string) |  |  |
| nick | [string](#string) |  |  |
| email | [string](#string) |  |  |






<a name="mruv.AccountID"></a>

### AccountID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.GetAccountCharactersResponse"></a>

### GetAccountCharactersResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| characters | [Character](#mruv.Character) | repeated |  |






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
| account_id | [uint32](#uint32) |  |  |






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
| account_id | [uint32](#uint32) |  |  |





 

 

 


<a name="mruv.MruVAccountsService"></a>

### MruVAccountsService
The MruV accounts service provides procedures for managing players accounts.
This service is an additional/intermediary service between the ORY Kratos &amp; ORY Hydra service.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| RegisterAccount | [RegisterAccountRequest](#mruv.RegisterAccountRequest) | [RegisterAccountResponse](#mruv.RegisterAccountResponse) |  |
| LogIn | [LogInRequest](#mruv.LogInRequest) | [LogInResponse](#mruv.LogInResponse) |  |
| GetAccount | [AccountID](#mruv.AccountID) | [Account](#mruv.Account) |  |
| GetAccountCharacters | [AccountID](#mruv.AccountID) | [GetAccountCharactersResponse](#mruv.GetAccountCharactersResponse) |  |

 



<a name="business/business.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## business/business.proto



<a name="mruv.business.AssignEstateRequest"></a>

### AssignEstateRequest
Request message for rpc `AssignEstate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| business_id | [uint32](#uint32) |  |  |
| estate_id | [uint32](#uint32) |  |  |






<a name="mruv.business.AssignEstateResponse"></a>

### AssignEstateResponse
Response message for rpc `AssignEstate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| estate_count | [uint32](#uint32) |  |  |






<a name="mruv.business.AssignOwnerRequest"></a>

### AssignOwnerRequest
Request message for rpc `AssignOwner`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.business.AssignOwnerResponse"></a>

### AssignOwnerResponse
Response message for rpc `AssignOwner`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| owner_type | [OwnerType](#mruv.business.OwnerType) |  |  |
| owner_id | [uint32](#uint32) |  |  |






<a name="mruv.business.Business"></a>

### Business
Business data structure.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |
| estate_ids | [int64](#int64) | repeated | Estates that belongs to a business. |
| product_id | [uint32](#uint32) |  | Purchase price in economy system. |
| owner_type | [OwnerType](#mruv.business.OwnerType) |  | Owner type of the business. |
| owner_id | [uint32](#uint32) |  | Owner of the business. |
| business_items | [uint32](#uint32) | repeated | Items that belongs to business. |
| business_group | [uint32](#uint32) |  | Business group |






<a name="mruv.business.BuyBusinessRequest"></a>

### BuyBusinessRequest
Request message for rpc `BuyBusiness`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| buyer_type | [OwnerType](#mruv.business.OwnerType) |  |  |
| buyer_id | [uint32](#uint32) |  |  |






<a name="mruv.business.BuyBusinessResponse"></a>

### BuyBusinessResponse
Response message for rpc `BuyBusiness`.






<a name="mruv.business.CreateBusinessRequest"></a>

### CreateBusinessRequest
Request message for rpc `CreateBusiness`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |
| product_id | [uint32](#uint32) |  | Purchase price in economy system. |






<a name="mruv.business.CreateBusinessResponse"></a>

### CreateBusinessResponse
Response message for rpc `CreateBusiness`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.business.DeleteBusinessRequest"></a>

### DeleteBusinessRequest
Request message for rpc `DeleteBusiness`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.business.DeleteBusinessResponse"></a>

### DeleteBusinessResponse
Response message for rpc `DeleteBusiness`.






<a name="mruv.business.GetBusinessRequest"></a>

### GetBusinessRequest
Request message for rpc `GetBusiness`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.business.GetBusinessResponse"></a>

### GetBusinessResponse
Response message for rpc `GetBusiness`.






<a name="mruv.business.UnassignEstateRequest"></a>

### UnassignEstateRequest
Request message for rpc `UnassignEstate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| business_id | [uint32](#uint32) |  |  |
| estate_id | [uint32](#uint32) |  |  |






<a name="mruv.business.UnassignEstateResponse"></a>

### UnassignEstateResponse
Response message for rpc `UnassignEstate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| estate_count | [uint32](#uint32) |  |  |






<a name="mruv.business.UpdateBusinessRequest"></a>

### UpdateBusinessRequest
Request message for rpc `UpdateBusiness`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.business.UpdateBusinessResponse"></a>

### UpdateBusinessResponse
Response message for rpc `UpdateBusiness`.






<a name="mruv.business.WatchBusinessRequest"></a>

### WatchBusinessRequest
Request message for rpc `WatchBusiness`.






<a name="mruv.business.WatchBusinessResponse"></a>

### WatchBusinessResponse
Response message for rpc `WatchBusiness`.






<a name="mruv.business.WatchBusinessesRequest"></a>

### WatchBusinessesRequest
Request message for rpc `WatchBusinesses`.






<a name="mruv.business.WatchBusinessesResponse"></a>

### WatchBusinessesResponse
Response message for rpc `WatchBusinesses`.





 


<a name="mruv.business.OwnerType"></a>

### OwnerType
Owner type.

| Name | Number | Description |
| ---- | ------ | ----------- |
| UNKNOWN | 0 |  |
| PLAYER | 1 |  |
| GROUP | 2 |  |
| SYSTEM | 3 |  |


 

 


<a name="mruv.business.MruVBusinessService"></a>

### MruVBusinessService
The MruV business service provides procedures for managing businesses.
Business can be owned by a player or organisation. Every business have it&#39;s own group and products to sell.
Business can have rights to an estates.
Every business has its own type and depends on it, business provides different services.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateBusiness | [CreateBusinessRequest](#mruv.business.CreateBusinessRequest) | [CreateBusinessResponse](#mruv.business.CreateBusinessResponse) | Create a business. |
| GetBusiness | [GetBusinessRequest](#mruv.business.GetBusinessRequest) | [Business](#mruv.business.Business) | Get a business. |
| UpdateBusiness | [UpdateBusinessRequest](#mruv.business.UpdateBusinessRequest) | [Business](#mruv.business.Business) | Update a business. |
| DeleteBusiness | [DeleteBusinessRequest](#mruv.business.DeleteBusinessRequest) | [DeleteBusinessResponse](#mruv.business.DeleteBusinessResponse) | Delete a business. |
| AssignOwner | [AssignOwnerRequest](#mruv.business.AssignOwnerRequest) | [AssignOwnerResponse](#mruv.business.AssignOwnerResponse) | Assign a business owner. |
| AssignEstate | [AssignEstateRequest](#mruv.business.AssignEstateRequest) | [AssignEstateResponse](#mruv.business.AssignEstateResponse) | Assign an estate to a business. |
| UnassignEstate | [UnassignEstateRequest](#mruv.business.UnassignEstateRequest) | [UnassignEstateResponse](#mruv.business.UnassignEstateResponse) |  |
| BuyBusiness | [BuyBusinessRequest](#mruv.business.BuyBusinessRequest) | [BuyBusinessResponse](#mruv.business.BuyBusinessResponse) | Buy a business. |
| WatchBusiness | [WatchBusinessRequest](#mruv.business.WatchBusinessRequest) | [WatchBusinessResponse](#mruv.business.WatchBusinessResponse) stream | Subscribe to business events. |
| WatchBusinesses | [WatchBusinessesRequest](#mruv.business.WatchBusinessesRequest) | [WatchBusinessesResponse](#mruv.business.WatchBusinessesResponse) stream | Subscribe to all businesses events. |

 



<a name="characters/characters.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## characters/characters.proto



<a name="mruv.Character"></a>

### Character



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| owner_id | [uint32](#uint32) |  |  |
| first_name | [string](#string) |  |  |
| second_name | [string](#string) |  |  |
| age | [uint32](#uint32) |  |  |
| sex | [uint32](#uint32) |  |  |
| position | [Position](#mruv.Position) |  |  |






<a name="mruv.CharacterID"></a>

### CharacterID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.CreateCharacterRequest"></a>

### CreateCharacterRequest
Request message for rpc `CreateCharacter`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| owner_id | [uint32](#uint32) |  |  |
| first_name | [string](#string) |  |  |
| second_name | [string](#string) |  |  |
| age | [uint32](#uint32) |  |  |
| sex | [uint32](#uint32) |  |  |






<a name="mruv.CreateCharacterResponse"></a>

### CreateCharacterResponse
Response message for rpc `CreateCharacter`.






<a name="mruv.DeathStreamRequest"></a>

### DeathStreamRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| death_types | [DeathType](#mruv.DeathType) | repeated |  |






<a name="mruv.DeathStreamResponse"></a>

### DeathStreamResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [Character](#mruv.Character) |  |  |
| death_type | [DeathType](#mruv.DeathType) |  |  |






<a name="mruv.DeleteCharacterRequest"></a>

### DeleteCharacterRequest
Request message for rpc `DeleteCharacter`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.DeleteCharacterResponse"></a>

### DeleteCharacterResponse
Response message for rpc `DeleteCharacter`.






<a name="mruv.GetCharacterRequest"></a>

### GetCharacterRequest
Request message for rpc `GetCharacter`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.GetCharacterResponse"></a>

### GetCharacterResponse
Response message for rpc `GetCharacter`.






<a name="mruv.UpdateCharacterRequest"></a>

### UpdateCharacterRequest
Request message for rpc `UpdateCharacter`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.UpdateCharacterResponse"></a>

### UpdateCharacterResponse
Response message for rpc `UpdateCharacter`.





 


<a name="mruv.DeathType"></a>

### DeathType


| Name | Number | Description |
| ---- | ------ | ----------- |
| DEATH_TYPE_NONE | 0 |  |
| DEATH_TYPE_BW | 1 |  |
| DEATH_TYPE_BW_KILL | 2 |  |
| DEATH_TYPE_CK | 3 |  |


 

 


<a name="mruv.MruVCharactersService"></a>

### MruVCharactersService


| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateCharacter | [CreateCharacterRequest](#mruv.CreateCharacterRequest) | [CreateCharacterResponse](#mruv.CreateCharacterResponse) | Create a character. |
| GetCharacter | [GetCharacterRequest](#mruv.GetCharacterRequest) | [GetCharacterResponse](#mruv.GetCharacterResponse) | Get a character. |
| UpdateCharacter | [UpdateCharacterRequest](#mruv.UpdateCharacterRequest) | [UpdateCharacterResponse](#mruv.UpdateCharacterResponse) | Update a character. |
| DeleteCharacter | [DeleteCharacterRequest](#mruv.DeleteCharacterRequest) | [DeleteCharacterResponse](#mruv.DeleteCharacterResponse) | Delete a character. |
| PermanentCharacterKill | [CharacterID](#mruv.CharacterID) | [CharacterID](#mruv.CharacterID) | Kill a character. A character that is killed cannot be played anymore. |
| DeathsStream | [DeathStreamRequest](#mruv.DeathStreamRequest) | [DeathStreamResponse](#mruv.DeathStreamResponse) stream | Stream of deaths. |
| GetServiceStatus | [ServiceStatusRequest](#mruv.ServiceStatusRequest) | [ServiceStatusResponse](#mruv.ServiceStatusResponse) | Service status |
| GetServiceVersion | [VersionRequest](#mruv.VersionRequest) | [VersionResponse](#mruv.VersionResponse) |  |

 



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





 

 

 

 



<a name="devtools/devtools.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## devtools/devtools.proto



<a name="mruv.devtools.DeletePositionRequest"></a>

### DeletePositionRequest
Delete position request message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| position | [Position](#mruv.devtools.Position) |  |  |






<a name="mruv.devtools.DeletePositionResponse"></a>

### DeletePositionResponse
Delete position response message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| success | [bool](#bool) |  |  |






<a name="mruv.devtools.GetAnimationRequest"></a>

### GetAnimationRequest
Get animations request message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| dict | [string](#string) |  |  |
| name | [string](#string) |  |  |






<a name="mruv.devtools.GetAnimationResponse"></a>

### GetAnimationResponse
Get animation response message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| animation | [Animation](#mruv.devtools.Animation) |  |  |
| author | [Player](#mruv.devtools.Player) |  |  |






<a name="mruv.devtools.GetAnimationsRequest"></a>

### GetAnimationsRequest
Get animations request message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [uint32](#uint32) |  |  |
| dict | [string](#string) |  |  |
| name | [string](#string) |  |  |






<a name="mruv.devtools.GetAnimationsResponse"></a>

### GetAnimationsResponse
Get animations response message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| animations | [GetAnimationsResponse.Row](#mruv.devtools.GetAnimationsResponse.Row) | repeated |  |






<a name="mruv.devtools.GetAnimationsResponse.Row"></a>

### GetAnimationsResponse.Row



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| animation | [Animation](#mruv.devtools.Animation) |  |  |
| author | [Player](#mruv.devtools.Player) |  |  |






<a name="mruv.devtools.GetOutfitsRequest"></a>

### GetOutfitsRequest
Get outfits request message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| category | [string](#string) |  |  |
| author | [string](#string) |  |  |






<a name="mruv.devtools.GetOutfitsResponse"></a>

### GetOutfitsResponse
Get outfits response message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| outfits | [GetOutfitsResponse.Row](#mruv.devtools.GetOutfitsResponse.Row) | repeated |  |






<a name="mruv.devtools.GetOutfitsResponse.Row"></a>

### GetOutfitsResponse.Row



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| outfit | [Outfit](#mruv.devtools.Outfit) |  |  |
| author | [Player](#mruv.devtools.Player) |  |  |






<a name="mruv.devtools.GetPositionsRequest"></a>

### GetPositionsRequest
Get position request message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [uint32](#uint32) |  |  |
| category | [string](#string) |  |  |
| author | [Player](#mruv.devtools.Player) |  |  |






<a name="mruv.devtools.GetPositionsResponse"></a>

### GetPositionsResponse
Get position response message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| positions | [GetPositionsResponse.Row](#mruv.devtools.GetPositionsResponse.Row) | repeated |  |






<a name="mruv.devtools.GetPositionsResponse.Row"></a>

### GetPositionsResponse.Row



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| position | [Position](#mruv.devtools.Position) |  |  |
| author | [Player](#mruv.devtools.Player) |  |  |






<a name="mruv.devtools.SaveAnimationRequest"></a>

### SaveAnimationRequest
Save animation request message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| animation | [Animation](#mruv.devtools.Animation) |  |  |






<a name="mruv.devtools.SaveAnimationResponse"></a>

### SaveAnimationResponse
Save animation response message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| success | [bool](#bool) |  |  |






<a name="mruv.devtools.SaveOutfitRequest"></a>

### SaveOutfitRequest
Save outfit request message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| outfit | [Outfit](#mruv.devtools.Outfit) |  |  |






<a name="mruv.devtools.SaveOutfitResponse"></a>

### SaveOutfitResponse
Save outfit response message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| success | [bool](#bool) |  |  |






<a name="mruv.devtools.SavePositionRequest"></a>

### SavePositionRequest
Save position request message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| position | [Position](#mruv.devtools.Position) |  |  |






<a name="mruv.devtools.SavePositionResponse"></a>

### SavePositionResponse
Save position response message.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| success | [bool](#bool) |  |  |





 

 

 


<a name="mruv.devtools.MruVDevToolsService"></a>

### MruVDevToolsService
The MruV developer tools service for mruv-devtools package.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| GetPositions | [GetPositionsRequest](#mruv.devtools.GetPositionsRequest) | [GetPositionsResponse](#mruv.devtools.GetPositionsResponse) | Get saved positions. |
| SavePosition | [SavePositionRequest](#mruv.devtools.SavePositionRequest) | [SavePositionResponse](#mruv.devtools.SavePositionResponse) | Save position. |
| DeletePosition | [DeletePositionRequest](#mruv.devtools.DeletePositionRequest) | [DeletePositionResponse](#mruv.devtools.DeletePositionResponse) | Delete position. |
| GetOutfits | [GetOutfitsRequest](#mruv.devtools.GetOutfitsRequest) | [GetOutfitsResponse](#mruv.devtools.GetOutfitsResponse) | Get saved outfit. |
| SaveOutfit | [SaveOutfitRequest](#mruv.devtools.SaveOutfitRequest) | [SaveOutfitResponse](#mruv.devtools.SaveOutfitResponse) | Save outfit. |
| GetAnimations | [GetAnimationsRequest](#mruv.devtools.GetAnimationsRequest) | [GetAnimationsResponse](#mruv.devtools.GetAnimationsResponse) | Get all saved animations. |
| GetAnimation | [GetAnimationRequest](#mruv.devtools.GetAnimationRequest) | [GetAnimationResponse](#mruv.devtools.GetAnimationResponse) | Get saved animation by name. |
| SaveAnimation | [SaveAnimationRequest](#mruv.devtools.SaveAnimationRequest) | [SaveAnimationResponse](#mruv.devtools.SaveAnimationResponse) | Save animation. |
| GetServiceStatus | [.mruv.ServiceStatusRequest](#mruv.ServiceStatusRequest) | [.mruv.ServiceStatusResponse](#mruv.ServiceStatusResponse) | Get service status. |
| GetServiceVersion | [.mruv.VersionRequest](#mruv.VersionRequest) | [.mruv.VersionResponse](#mruv.VersionResponse) | Get service version. |

 



<a name="devtools/devtools_model.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## devtools/devtools_model.proto



<a name="mruv.devtools.Animation"></a>

### Animation
GTA V animation structure.
You can find more information about RageMP outfits [here](https://wiki.rage.mp/index.php?title=Animations &#34;RageMP Animations&#34;)


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| dict | [string](#string) |  | Animation dictionary name. |
| name | [string](#string) |  | Animation name. |
| readable_category | [string](#string) |  | Animation category, specified by author. |
| category | [string](#string) |  |  |






<a name="mruv.devtools.Outfit"></a>

### Outfit
GTA V player outfit structure.
You can find more information about RageMP outfits [here](https://wiki.rage.mp/index.php?title=Clothes &#34;RageMP Clothes&#34;)


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  | Name of the outfit. |
| category | [string](#string) |  | Category of the outfit. |






<a name="mruv.devtools.Player"></a>

### Player
Player structure for storing authors of devtools saved records.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  | Unique id. |
| name | [string](#string) |  | Unique name. |
| hash | [string](#string) |  | Password hash. |






<a name="mruv.devtools.Position"></a>

### Position
Position structure.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| x | [double](#double) |  |  |
| y | [double](#double) |  |  |
| z | [double](#double) |  |  |
| name | [string](#string) |  | Short position name. |
| description | [string](#string) |  | Description of the place which the position indicates. |





 

 

 

 



<a name="economy/economy.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## economy/economy.proto



<a name="mruv.economy.BuyProductRequest"></a>

### BuyProductRequest
Request message for rpc `BuyProduct`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |






<a name="mruv.economy.BuyProductResponse"></a>

### BuyProductResponse
Response message for rpc `BuyProduct`.






<a name="mruv.economy.DeleteProductRequest"></a>

### DeleteProductRequest
Request message for rpc `DeleteProduct`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |






<a name="mruv.economy.DeleteProductResponse"></a>

### DeleteProductResponse
Response message for rpc `DeleteProduct`.






<a name="mruv.economy.GetPriceRequest"></a>

### GetPriceRequest
Request message for rpc `GetPrice`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |






<a name="mruv.economy.GetPriceResponse"></a>

### GetPriceResponse
Response message for rpc `GetPrice`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| price | [uint32](#uint32) |  |  |






<a name="mruv.economy.GetProductRequest"></a>

### GetProductRequest
Request message for rpc `GetProduct`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |






<a name="mruv.economy.GetProductResponse"></a>

### GetProductResponse
Response message for rpc `GetProduct`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| full_name | [string](#string) |  |  |
| description | [string](#string) |  |  |
| price_class | [uint32](#uint32) |  |  |
| price_ratio | [float](#float) |  |  |
| starting_price | [uint32](#uint32) |  |  |
| price | [uint32](#uint32) |  |  |






<a name="mruv.economy.RegisterProductRequest"></a>

### RegisterProductRequest
Request message for rpc `RegisterProduct`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| full_name | [string](#string) |  |  |
| description | [string](#string) |  |  |
| price_class | [uint32](#uint32) |  |  |
| price_ratio | [float](#float) |  |  |
| starting_price | [uint32](#uint32) |  |  |






<a name="mruv.economy.RegisterProductResponse"></a>

### RegisterProductResponse
Response message for rpc `RegisterProduct`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.economy.UpdatePriceRequest"></a>

### UpdatePriceRequest
Request message for rpc `UpdatePrice`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |
| new_price | [uint32](#uint32) |  |  |






<a name="mruv.economy.UpdatePriceResponse"></a>

### UpdatePriceResponse
Response message for rpc `UpdatePrice`.






<a name="mruv.economy.UpdateProductRequest"></a>

### UpdateProductRequest
Request message for rpc `UpdateProduct`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |
| full_name | [string](#string) |  |  |
| description | [string](#string) |  |  |
| price_class | [uint32](#uint32) |  |  |
| price_ratio | [float](#float) |  |  |






<a name="mruv.economy.UpdateProductResponse"></a>

### UpdateProductResponse
Response message for rpc `UpdateProduct`.






<a name="mruv.economy.WatchPriceRequest"></a>

### WatchPriceRequest
Request message for rpc `WatchPrice`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |






<a name="mruv.economy.WatchPriceResponse"></a>

### WatchPriceResponse
Response message for rpc `WatchPrice`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| price | [uint32](#uint32) |  |  |






<a name="mruv.economy.WatchProductRequest"></a>

### WatchProductRequest
Request message for rpc `WatchProduct`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |






<a name="mruv.economy.WatchProductResponse"></a>

### WatchProductResponse
Response message for rpc `WatchProduct`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| event | [WatchProductResponse.ProductEvent](#mruv.economy.WatchProductResponse.ProductEvent) |  |  |





 


<a name="mruv.economy.WatchProductResponse.ProductEvent"></a>

### WatchProductResponse.ProductEvent


| Name | Number | Description |
| ---- | ------ | ----------- |
| UNKNOWN | 0 |  |
| PRICE_CHANGED | 1 |  |
| PRODUCT_BOUGHT | 2 |  |
| PRODUCT_INFO_UPDATED | 3 |  |
| PRODUCT_DELETED | 4 |  |


 

 


<a name="mruv.economy.MruVEconomyService"></a>

### MruVEconomyService
The MruV economy service provides procedures for managing prices and economy.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| RegisterProduct | [RegisterProductRequest](#mruv.economy.RegisterProductRequest) | [RegisterProductResponse](#mruv.economy.RegisterProductResponse) | Register price in economy system. |
| GetProduct | [GetProductRequest](#mruv.economy.GetProductRequest) | [GetProductResponse](#mruv.economy.GetProductResponse) | Get product information. |
| UpdateProduct | [UpdateProductRequest](#mruv.economy.UpdateProductRequest) | [UpdateProductResponse](#mruv.economy.UpdateProductResponse) | Update product information. |
| DeleteProduct | [DeleteProductRequest](#mruv.economy.DeleteProductRequest) | [DeleteProductResponse](#mruv.economy.DeleteProductResponse) |  |
| UpdatePrice | [UpdatePriceRequest](#mruv.economy.UpdatePriceRequest) | [UpdatePriceResponse](#mruv.economy.UpdatePriceResponse) | Update product price. |
| GetPrice | [GetPriceRequest](#mruv.economy.GetPriceRequest) | [GetPriceResponse](#mruv.economy.GetPriceResponse) | Get current value for registered price. |
| BuyProduct | [BuyProductRequest](#mruv.economy.BuyProductRequest) | [BuyProductResponse](#mruv.economy.BuyProductResponse) | Send information to the system, that the product has been purchased. This rpc call can affect a product price. |
| WatchProduct | [WatchProductRequest](#mruv.economy.WatchProductRequest) | [WatchProductResponse](#mruv.economy.WatchProductResponse) stream | Subscribe to events related to a product. |
| WatchPrice | [WatchPriceRequest](#mruv.economy.WatchPriceRequest) | [WatchPriceResponse](#mruv.economy.WatchPriceResponse) stream | Subscribe to product price changes. |

 



<a name="estates/elevators.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## estates/elevators.proto



<a name="mruv.elevators.CreateElevatorRequest"></a>

### CreateElevatorRequest
Request message for rpc `CreateElevator`.






<a name="mruv.elevators.CreateElevatorResponse"></a>

### CreateElevatorResponse
Response message for rpc `CreateElevator`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.elevators.DeleteElevatorRequest"></a>

### DeleteElevatorRequest
Request message for rpc `DeleteElevator`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.elevators.DeleteElevatorResponse"></a>

### DeleteElevatorResponse
Response message for rpc `DeleteElevator`.






<a name="mruv.elevators.GetElevatorFloorsRequest"></a>

### GetElevatorFloorsRequest
Request message for rpc `GetElevatorFloors`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.elevators.GetElevatorFloorsResponse"></a>

### GetElevatorFloorsResponse
Response message for rpc `GetElevatorFloors`.






<a name="mruv.elevators.GetElevatorRequest"></a>

### GetElevatorRequest
Request message for rpc `GetElevator`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.elevators.GetElevatorResponse"></a>

### GetElevatorResponse
Response message for rpc `GetElevator`.






<a name="mruv.elevators.UpdateElevatorRequest"></a>

### UpdateElevatorRequest
Request message for rpc `UpdateElevator`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.elevators.UpdateElevatorResponse"></a>

### UpdateElevatorResponse
Response message for rpc `UpdateElevator`.





 

 

 


<a name="mruv.elevators.MruVElevatorsService"></a>

### MruVElevatorsService
The MruV entrances service provides procedures for managing an elevators.
Elevators allow all players in the elevator area to move between building floors.
Floor change is processed in following steps:
1. Someone chooses a floor
1. Doors closing event is fired
2. Doors closed event is fired.
3. Everyone in a elevator are registered as players, that will be teleported to chosen floor.
4. X seconds delay (elevator is moving)
5. Teleport players to other floor elevator
6. Doors opening
7. Doors opened - end
You can define a one-man pseudo-elevator where only point 5 is executed.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateElevator | [CreateElevatorRequest](#mruv.elevators.CreateElevatorRequest) | [CreateElevatorResponse](#mruv.elevators.CreateElevatorResponse) | Create an elevator. |
| GetElevator | [GetElevatorRequest](#mruv.elevators.GetElevatorRequest) | [GetElevatorResponse](#mruv.elevators.GetElevatorResponse) | Get an elevator. |
| UpdateElevator | [UpdateElevatorRequest](#mruv.elevators.UpdateElevatorRequest) | [UpdateElevatorResponse](#mruv.elevators.UpdateElevatorResponse) | Update an elevator. |
| DeleteElevator | [DeleteElevatorRequest](#mruv.elevators.DeleteElevatorRequest) | [DeleteElevatorResponse](#mruv.elevators.DeleteElevatorResponse) | Delete an elevator. |
| GetElevatorFloors | [GetElevatorFloorsRequest](#mruv.elevators.GetElevatorFloorsRequest) | [GetElevatorFloorsResponse](#mruv.elevators.GetElevatorFloorsResponse) | Get available elevator floors. |

 



<a name="estates/entrances.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## estates/entrances.proto



<a name="mruv.entrances.CreateEntranceRequest"></a>

### CreateEntranceRequest
Request message for rpc `CreateEntrance`.






<a name="mruv.entrances.CreateEntranceResponse"></a>

### CreateEntranceResponse
Response message for rpc `CreateEntrance`.






<a name="mruv.entrances.DeleteEntranceRequest"></a>

### DeleteEntranceRequest
Request message for rpc `DeleteEntrance`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.entrances.DeleteEntranceResponse"></a>

### DeleteEntranceResponse
Response message for rpc `DeleteEntrance`.






<a name="mruv.entrances.EnterRequest"></a>

### EnterRequest
Request message for rpc `Enter`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.entrances.EnterResponse"></a>

### EnterResponse
Response message for rpc `Enter`.






<a name="mruv.entrances.Entrance"></a>

### Entrance



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| estate_id | [uint32](#uint32) |  |  |
| out | [Entrance.EntranceDoor](#mruv.entrances.Entrance.EntranceDoor) |  |  |
| in | [Entrance.EntranceDoor](#mruv.entrances.Entrance.EntranceDoor) |  |  |






<a name="mruv.entrances.Entrance.EntranceDoor"></a>

### Entrance.EntranceDoor



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| message | [string](#string) |  |  |
| icon | [int32](#int32) |  |  |
| marker | [int32](#int32) |  |  |
| x | [float](#float) |  |  |
| y | [float](#float) |  |  |
| z | [float](#float) |  |  |
| vw | [int32](#int32) |  |  |
| int | [int32](#int32) |  |  |
| estate_id | [uint32](#uint32) |  |  |






<a name="mruv.entrances.FindNearestEntranceRequest"></a>

### FindNearestEntranceRequest
Request message for rpc `FindNearestEntrance`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| x | [float](#float) |  |  |
| y | [float](#float) |  |  |
| z | [float](#float) |  |  |
| max_distance | [float](#float) |  |  |






<a name="mruv.entrances.FindNearestEntranceResponse"></a>

### FindNearestEntranceResponse
Response message for rpc `FindNearestEntrance`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| distance | [float](#float) |  |  |






<a name="mruv.entrances.GetEntranceRequest"></a>

### GetEntranceRequest
Request message for rpc `GetEntrance`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.entrances.GetEntranceResponse"></a>

### GetEntranceResponse
Response message for rpc `GetEntrance`.






<a name="mruv.entrances.LockRequest"></a>

### LockRequest
Request message for rpc `Lock`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.entrances.LockResponse"></a>

### LockResponse
Response message for rpc `Lock`.






<a name="mruv.entrances.UnlockRequest"></a>

### UnlockRequest
Request message for rpc `Unlock`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.entrances.UnlockResponse"></a>

### UnlockResponse
Response message for rpc `Unlock`.






<a name="mruv.entrances.UpdateEntranceRequest"></a>

### UpdateEntranceRequest
Request message for rpc `UpdateEntrance`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.entrances.UpdateEntranceResponse"></a>

### UpdateEntranceResponse
Response message for rpc `UpdateEntrance`.





 

 

 


<a name="mruv.entrances.MruVEntrancesService"></a>

### MruVEntrancesService
The MruV entrances service provides procedures for managing an entrances to estates and teleportation to locations.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateEntrance | [CreateEntranceRequest](#mruv.entrances.CreateEntranceRequest) | [CreateEntranceResponse](#mruv.entrances.CreateEntranceResponse) | Create an entrance to building or teleport to location. |
| GetEntrance | [GetEntranceRequest](#mruv.entrances.GetEntranceRequest) | [GetEntranceResponse](#mruv.entrances.GetEntranceResponse) | Get an entrance to building or a teleport to location. |
| UpdateEntrance | [UpdateEntranceRequest](#mruv.entrances.UpdateEntranceRequest) | [UpdateEntranceResponse](#mruv.entrances.UpdateEntranceResponse) | Update an entrance to building or a teleport to location. |
| DeleteEntrance | [DeleteEntranceRequest](#mruv.entrances.DeleteEntranceRequest) | [DeleteEntranceResponse](#mruv.entrances.DeleteEntranceResponse) | Delete an entrance to building or a teleport to location. |
| Lock | [LockRequest](#mruv.entrances.LockRequest) | [LockResponse](#mruv.entrances.LockResponse) | Lock entrance. |
| Unlock | [UnlockRequest](#mruv.entrances.UnlockRequest) | [UnlockResponse](#mruv.entrances.UnlockResponse) | Unload entrance. |
| FindNearestEntrance | [FindNearestEntranceRequest](#mruv.entrances.FindNearestEntranceRequest) | [FindNearestEntranceResponse](#mruv.entrances.FindNearestEntranceResponse) | Find gate that is closest to a specific position. |
| Enter | [EnterRequest](#mruv.entrances.EnterRequest) | [EnterResponse](#mruv.entrances.EnterResponse) | Enter an entrance |

 



<a name="estates/estates.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## estates/estates.proto



<a name="mruv.estates.AddEntranceRequest"></a>

### AddEntranceRequest
Request message for rpc `AddEntrance`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| estate_id | [uint32](#uint32) |  |  |
| entrance_id | [uint32](#uint32) |  |  |






<a name="mruv.estates.AddEntranceResponse"></a>

### AddEntranceResponse
Response message for rpc `AddEntrance`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| entrance_count | [uint32](#uint32) |  |  |






<a name="mruv.estates.AddGateRequest"></a>

### AddGateRequest
Request message for rpc `AddGate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| estate_id | [uint32](#uint32) |  |  |
| gate_id | [uint32](#uint32) |  |  |






<a name="mruv.estates.AddGateResponse"></a>

### AddGateResponse
Response message for rpc `AddGate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| gate_count | [uint32](#uint32) |  |  |






<a name="mruv.estates.CreateEstateRequest"></a>

### CreateEstateRequest
Request message for rpc `CreateEstate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |






<a name="mruv.estates.CreateEstateResponse"></a>

### CreateEstateResponse
Response message for rpc `CreateEstate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.estates.DeleteEstateRequest"></a>

### DeleteEstateRequest
Request message for rpc `DeleteEstate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.estates.DeleteEstateResponse"></a>

### DeleteEstateResponse
Response message for rpc `DeleteEstate`.






<a name="mruv.estates.DeleteGateRequest"></a>

### DeleteGateRequest
Request message for rpc `DeleteGate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| estate_id | [uint32](#uint32) |  |  |
| gate_id | [uint32](#uint32) |  |  |






<a name="mruv.estates.DeleteGateResponse"></a>

### DeleteGateResponse
Response message for rpc `DeleteGate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| gate_count | [uint32](#uint32) |  |  |






<a name="mruv.estates.Estate"></a>

### Estate



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |
| entrances | [uint32](#uint32) | repeated |  |
| gates | [uint32](#uint32) | repeated |  |
| rooms | [uint32](#uint32) | repeated |  |






<a name="mruv.estates.GetEstateEntrancesRequest"></a>

### GetEstateEntrancesRequest
Request message for rpc `GetEstateEntrances`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| estate_id | [uint32](#uint32) |  |  |






<a name="mruv.estates.GetEstateEntrancesResponse"></a>

### GetEstateEntrancesResponse
Response message for rpc `GetEstateEntrances`.






<a name="mruv.estates.GetEstateGatesRequest"></a>

### GetEstateGatesRequest
Request message for rpc `GetEstateGates`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| estate_id | [uint32](#uint32) |  |  |






<a name="mruv.estates.GetEstateGatesResponse"></a>

### GetEstateGatesResponse
Response message for rpc `GetEstateGates`.






<a name="mruv.estates.GetEstateRequest"></a>

### GetEstateRequest
Request message for rpc `GetEstate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.estates.GetEstatesRequest"></a>

### GetEstatesRequest
Request message for rpc `GetEstates`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.estates.GetEstatesResponse"></a>

### GetEstatesResponse
Response message for rpc `GetEstates`.






<a name="mruv.estates.RemoveEntranceRequest"></a>

### RemoveEntranceRequest
Request message for rpc `RemoveEntrance`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| estate_id | [uint32](#uint32) |  |  |
| entrance_id | [uint32](#uint32) |  |  |






<a name="mruv.estates.RemoveEntranceResponse"></a>

### RemoveEntranceResponse
Response message for rpc `RemoveEntrance`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| entrance_count | [uint32](#uint32) |  |  |






<a name="mruv.estates.UpdateEstateRequest"></a>

### UpdateEstateRequest
Request message for rpc `UpdateEstate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |






<a name="mruv.estates.UpdateEstateResponse"></a>

### UpdateEstateResponse
Response message for rpc `UpdateEstate`.





 

 

 


<a name="mruv.estates.MruVEstateService"></a>

### MruVEstateService
The MruV estate service provides procedures for managing buildings and other estates.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateEstate | [CreateEstateRequest](#mruv.estates.CreateEstateRequest) | [CreateEstateResponse](#mruv.estates.CreateEstateResponse) | Create real estate. |
| GetEstate | [GetEstateRequest](#mruv.estates.GetEstateRequest) | [Estate](#mruv.estates.Estate) | Get real estate. |
| UpdateEstate | [UpdateEstateRequest](#mruv.estates.UpdateEstateRequest) | [UpdateEstateResponse](#mruv.estates.UpdateEstateResponse) | Update real estate. |
| DeleteEstate | [DeleteEstateRequest](#mruv.estates.DeleteEstateRequest) | [DeleteEstateResponse](#mruv.estates.DeleteEstateResponse) | Delete real estate. |
| GetEstates | [GetEstatesRequest](#mruv.estates.GetEstatesRequest) | [GetEstatesResponse](#mruv.estates.GetEstatesResponse) | Get all created real estates. |
| AddGate | [AddGateRequest](#mruv.estates.AddGateRequest) | [AddGateResponse](#mruv.estates.AddGateResponse) | Add a gate to an estate. |
| DeleteGate | [DeleteGateRequest](#mruv.estates.DeleteGateRequest) | [DeleteGateResponse](#mruv.estates.DeleteGateResponse) | Delete a gate from estate. |
| GetEstateGates | [GetEstateGatesRequest](#mruv.estates.GetEstateGatesRequest) | [GetEstateGatesResponse](#mruv.estates.GetEstateGatesResponse) | Get all estate gates. |
| AddEntrance | [AddEntranceRequest](#mruv.estates.AddEntranceRequest) | [AddEntranceResponse](#mruv.estates.AddEntranceResponse) | Add an entrance to estate. |
| RemoveEntrance | [RemoveEntranceRequest](#mruv.estates.RemoveEntranceRequest) | [RemoveEntranceResponse](#mruv.estates.RemoveEntranceResponse) | Remove an entrance from estate. |
| GetEstateEntrances | [GetEstateEntrancesRequest](#mruv.estates.GetEstateEntrancesRequest) | [GetEstateEntrancesResponse](#mruv.estates.GetEstateEntrancesResponse) | Get all estate entrances. |

 



<a name="estates/gates.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## estates/gates.proto



<a name="mruv.gates.CloseRequest"></a>

### CloseRequest
Request message for rpc `Close`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.gates.CloseResponse"></a>

### CloseResponse
Response message for rpc `Close`.






<a name="mruv.gates.CreateGateRequest"></a>

### CreateGateRequest
Request message for rpc `CreateGate`.






<a name="mruv.gates.CreateGateResponse"></a>

### CreateGateResponse
Response message for rpc `CreateGate`.






<a name="mruv.gates.DeleteGateRequest"></a>

### DeleteGateRequest
Request message for rpc `DeleteGate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.gates.DeleteGateResponse"></a>

### DeleteGateResponse
Response message for rpc `DeleteGate`.






<a name="mruv.gates.FindNearestGateRequest"></a>

### FindNearestGateRequest
Request message for rpc `FindNearestGate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| x | [float](#float) |  |  |
| y | [float](#float) |  |  |
| z | [float](#float) |  |  |
| max_distance | [float](#float) |  |  |






<a name="mruv.gates.FindNearestGateResponse"></a>

### FindNearestGateResponse
Response message for rpc `FindNearestGate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| distance | [float](#float) |  |  |






<a name="mruv.gates.Gate"></a>

### Gate



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| estate_id | [uint32](#uint32) |  |  |






<a name="mruv.gates.GetGateRequest"></a>

### GetGateRequest
Request message for rpc `GetGate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.gates.GetGateResponse"></a>

### GetGateResponse
Response message for rpc `GetGate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.gates.LockRequest"></a>

### LockRequest
Request message for rpc `Lock`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.gates.LockResponse"></a>

### LockResponse
Response message for rpc `Lock`.






<a name="mruv.gates.OpenRequest"></a>

### OpenRequest
Request message for rpc `Open`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.gates.OpenResponse"></a>

### OpenResponse
Response message for rpc `Open`.






<a name="mruv.gates.UnlockRequest"></a>

### UnlockRequest
Request message for rpc `Unlock`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.gates.UnlockResponse"></a>

### UnlockResponse
Response message for rpc `Unlock`.






<a name="mruv.gates.UpdateGateRequest"></a>

### UpdateGateRequest
Request message for rpc `UpdateGate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.gates.UpdateGateResponse"></a>

### UpdateGateResponse
Response message for rpc `UpdateGate`.





 

 

 


<a name="mruv.gates.MruVGatesService"></a>

### MruVGatesService
The MruV gates service provides procedures for managing gates and moving objects groups.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateGate | [CreateGateRequest](#mruv.gates.CreateGateRequest) | [CreateGateResponse](#mruv.gates.CreateGateResponse) | Create a gate or a moving objects objects group. |
| GetGate | [GetGateRequest](#mruv.gates.GetGateRequest) | [GetGateResponse](#mruv.gates.GetGateResponse) | Get a gate or a moving objects objects group. |
| UpdateGate | [UpdateGateRequest](#mruv.gates.UpdateGateRequest) | [UpdateGateResponse](#mruv.gates.UpdateGateResponse) | Update a gate or a moving objects objects group. |
| DeleteGate | [DeleteGateRequest](#mruv.gates.DeleteGateRequest) | [DeleteGateResponse](#mruv.gates.DeleteGateResponse) | Delete a gate or a moving objects objects group. |
| Lock | [LockRequest](#mruv.gates.LockRequest) | [LockResponse](#mruv.gates.LockResponse) | Lock a gate. Locked gate cannot be opened. |
| Unlock | [UnlockRequest](#mruv.gates.UnlockRequest) | [UnlockResponse](#mruv.gates.UnlockResponse) | Unload a gate, so it can be open. |
| Open | [OpenRequest](#mruv.gates.OpenRequest) | [OpenResponse](#mruv.gates.OpenResponse) | Opens a gate. |
| Close | [CloseRequest](#mruv.gates.CloseRequest) | [CloseResponse](#mruv.gates.CloseResponse) | Close a gate. |
| FindNearestGate | [FindNearestGateRequest](#mruv.gates.FindNearestGateRequest) | [FindNearestGateResponse](#mruv.gates.FindNearestGateResponse) | Find gate that is closest to a specific position. |

 



<a name="groups/groups.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## groups/groups.proto



<a name="mruv.AddGroupMemberRequest"></a>

### AddGroupMemberRequest







<a name="mruv.AddGroupMemberResponse"></a>

### AddGroupMemberResponse







<a name="mruv.GetGroupsRequest"></a>

### GetGroupsRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [uint32](#uint32) |  |  |






<a name="mruv.GetGroupsResponse"></a>

### GetGroupsResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| groups | [Group](#mruv.Group) | repeated |  |






<a name="mruv.Group"></a>

### Group



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |
| permissions | [Permission](#mruv.Permission) | repeated |  |
| members | [uint32](#uint32) | repeated |  |






<a name="mruv.GroupID"></a>

### GroupID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.Permission"></a>

### Permission



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |
| role | [string](#string) |  |  |






<a name="mruv.PermissionID"></a>

### PermissionID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.RemoveGroupMemberRequest"></a>

### RemoveGroupMemberRequest







<a name="mruv.RemoveGroupMemberResponse"></a>

### RemoveGroupMemberResponse






 

 

 


<a name="mruv.MruVGroupsService"></a>

### MruVGroupsService
The MruV groups service provides procedures for managing groups.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateGroup | [Group](#mruv.Group) | [GroupID](#mruv.GroupID) | CRUD |
| GetGroup | [GroupID](#mruv.GroupID) | [Group](#mruv.Group) |  |
| DeleteGroup | [GroupID](#mruv.GroupID) | [GroupID](#mruv.GroupID) |  |
| GetGroups | [GetGroupsRequest](#mruv.GetGroupsRequest) | [GetGroupsResponse](#mruv.GetGroupsResponse) |  |
| AddGroupMember | [AddGroupMemberRequest](#mruv.AddGroupMemberRequest) | [AddGroupMemberResponse](#mruv.AddGroupMemberResponse) |  |
| RemoveGroupMember | [RemoveGroupMemberRequest](#mruv.RemoveGroupMemberRequest) | [RemoveGroupMemberResponse](#mruv.RemoveGroupMemberResponse) |  |
| GetServiceStatus | [ServiceStatusRequest](#mruv.ServiceStatusRequest) | [ServiceStatusResponse](#mruv.ServiceStatusResponse) | Service status |
| GetServiceVersion | [VersionRequest](#mruv.VersionRequest) | [VersionResponse](#mruv.VersionResponse) |  |

 



<a name="houses/houses.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## houses/houses.proto



<a name="mruv.houses.CreateHouseRequest"></a>

### CreateHouseRequest
Request message for rpc `CreateHouse`.






<a name="mruv.houses.CreateHouseResponse"></a>

### CreateHouseResponse
Response message for rpc `CreateHouse`.






<a name="mruv.houses.DeleteHouseRequest"></a>

### DeleteHouseRequest
Request message for rpc `DeleteHouse`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.houses.DeleteHouseResponse"></a>

### DeleteHouseResponse
Response message for rpc `DeleteHouse`.






<a name="mruv.houses.GetHouseRequest"></a>

### GetHouseRequest
Request message for rpc `GetHouse`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.houses.GetHouseResponse"></a>

### GetHouseResponse
Response message for rpc `GetHouse`.






<a name="mruv.houses.UpdateHouseRequest"></a>

### UpdateHouseRequest
Request message for rpc `UpdateHouse`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.houses.UpdateHouseResponse"></a>

### UpdateHouseResponse
Response message for rpc `UpdateHouse`.





 

 

 


<a name="mruv.houses.MruVHousesService"></a>

### MruVHousesService
The MruV houses service provides procedures for managing houses.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateHouse | [CreateHouseRequest](#mruv.houses.CreateHouseRequest) | [CreateHouseResponse](#mruv.houses.CreateHouseResponse) | Create a house. |
| GetHouse | [GetHouseRequest](#mruv.houses.GetHouseRequest) | [GetHouseResponse](#mruv.houses.GetHouseResponse) | Get a house. |
| UpdateHouse | [UpdateHouseRequest](#mruv.houses.UpdateHouseRequest) | [UpdateHouseResponse](#mruv.houses.UpdateHouseResponse) | Update a house. |
| DeleteHouse | [DeleteHouseRequest](#mruv.houses.DeleteHouseRequest) | [DeleteHouseResponse](#mruv.houses.DeleteHouseResponse) | Delete a house. |

 



<a name="items/items.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## items/items.proto



<a name="mruv.GetContainerItemsRequest"></a>

### GetContainerItemsRequest
Request message for `MruVItemsService.GetContainerItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [uint32](#uint32) |  | ID of container with items. |
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
| container_id | [uint32](#uint32) |  | ID of container that contains items. |
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
| container_id | [uint32](#uint32) |  | ID of the container from which we pull out a item. |
| item_id | [uint32](#uint32) |  | ID of the item we want to pull out. That item must be inside the container. |






<a name="mruv.PutItemRequest"></a>

### PutItemRequest
Request message for `MruVItemsService.PutItem`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [uint32](#uint32) |  | ID of container where to put item. |
| item_id | [uint32](#uint32) |  | ID of item we wan to put in. |
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
| container_id | [uint32](#uint32) |  | ID of the container which contain items. |
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
| item_id | [uint32](#uint32) |  |  |






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
| CreateContainerType | [ContainerType](#mruv.ContainerType) | [ContainerTypeID](#mruv.ContainerTypeID) | Create a container type. |
| GetContainerType | [ContainerTypeID](#mruv.ContainerTypeID) | [ContainerType](#mruv.ContainerType) | Get a container type by id. |
| DeleteContainerType | [ContainerTypeID](#mruv.ContainerTypeID) | [ContainerTypeID](#mruv.ContainerTypeID) | Delete a container type by id. |
| GetContainerTypes | [GetContainerTypesRequest](#mruv.GetContainerTypesRequest) | [GetContainerTypesResponse](#mruv.GetContainerTypesResponse) | Get all container types. |
| GetContainerItems | [GetContainerItemsRequest](#mruv.GetContainerItemsRequest) | [GetContainerItemsResponse](#mruv.GetContainerItemsResponse) | Get items inside a container. |
| PullItem | [PullItemRequest](#mruv.PullItemRequest) | [Item](#mruv.Item) | Pull an item from container. |
| PutItem | [PutItemRequest](#mruv.PutItemRequest) | [PutItemResponse](#mruv.PutItemResponse) | Put an item into container. |
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
| id | [uint32](#uint32) |  |  |
| type_id | [uint32](#uint32) |  | ID of an container type. |
| item_id | [uint32](#uint32) |  | ID of container item representing container. |
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
| id | [uint32](#uint32) |  |  |
| container_item_type_id | [uint32](#uint32) |  | ID of an item type. |
| max_number | [uint32](#uint32) |  | Max items in the container. |
| max_volume | [float](#float) |  | Max volume of items in the container. |
| max_weight | [float](#float) |  | Max weight of items in the container. |
| valid_item_types | [int64](#int64) | repeated |  |






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
| container_id | [uint32](#uint32) |  | ID of container containing the item. |
| item_id | [uint32](#uint32) |  |  |
| item | [Item](#mruv.Item) |  |  |
| position | [int32](#int32) |  | Position representing order in container. In ascending manner. |






<a name="mruv.Item"></a>

### Item
Item data structure.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| item_type_id | [uint32](#uint32) |  | ID of an item type. |
| weight | [float](#float) |  | Current weight of the item. |
| volume | [float](#float) |  | Current volume of the item. |






<a name="mruv.ItemID"></a>

### ItemID
Item ID.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.ItemType"></a>

### ItemType
Item type data structure


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
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


 

 

 



<a name="jobs/jobs.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## jobs/jobs.proto



<a name="mruv.jobs.CreateJobRequest"></a>

### CreateJobRequest
Request message for rpc `CreateJob`.






<a name="mruv.jobs.CreateJobResponse"></a>

### CreateJobResponse
Response message for rpc `CreateJob`.






<a name="mruv.jobs.DeleteJobRequest"></a>

### DeleteJobRequest
Request message for rpc `DeleteJob`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.jobs.DeleteJobResponse"></a>

### DeleteJobResponse
Response message for rpc `DeleteJob`.






<a name="mruv.jobs.GetJobRequest"></a>

### GetJobRequest
Request message for rpc `GetJob`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.jobs.GetJobResponse"></a>

### GetJobResponse
Response message for rpc `GetJob`.






<a name="mruv.jobs.UpdateJobRequest"></a>

### UpdateJobRequest
Request message for rpc `UpdateJob`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.jobs.UpdateJobResponse"></a>

### UpdateJobResponse
Response message for rpc `UpdateJob`.





 

 

 


<a name="mruv.jobs.MruVJobsService"></a>

### MruVJobsService
The MruV jobs service provides procedures for managing jobs.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateJob | [CreateJobRequest](#mruv.jobs.CreateJobRequest) | [CreateJobResponse](#mruv.jobs.CreateJobResponse) | Create a job. |
| GetJob | [GetJobRequest](#mruv.jobs.GetJobRequest) | [GetJobResponse](#mruv.jobs.GetJobResponse) | Get a job. |
| UpdateJob | [UpdateJobRequest](#mruv.jobs.UpdateJobRequest) | [UpdateJobResponse](#mruv.jobs.UpdateJobResponse) | Update a job. |
| DeleteJob | [DeleteJobRequest](#mruv.jobs.DeleteJobRequest) | [DeleteJobResponse](#mruv.jobs.DeleteJobResponse) | Delete a job. |

 



<a name="offers/offers.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## offers/offers.proto



<a name="mruv.offers.AcceptOfferRequest"></a>

### AcceptOfferRequest
Request message for rpc `AcceptOffer`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.offers.AcceptOfferResponse"></a>

### AcceptOfferResponse
Response message for rpc `AcceptOffer`.






<a name="mruv.offers.CreateOfferRequest"></a>

### CreateOfferRequest
Request message for rpc `CreateOffer`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |
| offer | [string](#string) |  |  |
| end_date | [int64](#int64) |  |  |
| price | [uint32](#uint32) |  |  |
| offer_type | [OfferType](#mruv.offers.OfferType) |  |  |
| offer_entity_id | [uint32](#uint32) |  |  |






<a name="mruv.offers.CreateOfferResponse"></a>

### CreateOfferResponse
Response message for rpc `CreateOffer`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.offers.DeleteOfferRequest"></a>

### DeleteOfferRequest
Request message for rpc `DeleteOffer`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.offers.DeleteOfferResponse"></a>

### DeleteOfferResponse
Response message for rpc `DeleteOffer`.






<a name="mruv.offers.GetOfferRequest"></a>

### GetOfferRequest
Request message for rpc `GetOffer`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.offers.GetOfferResponse"></a>

### GetOfferResponse
Response message for rpc `GetOffer`.






<a name="mruv.offers.UpdateOfferRequest"></a>

### UpdateOfferRequest
Request message for rpc `UpdateOffer`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.offers.UpdateOfferResponse"></a>

### UpdateOfferResponse
Response message for rpc `UpdateOffer`.





 


<a name="mruv.offers.OfferType"></a>

### OfferType


| Name | Number | Description |
| ---- | ------ | ----------- |
| UNKNOWN | 0 |  |


 

 


<a name="mruv.offers.MruVOffersService"></a>

### MruVOffersService
The MruV offers service.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateOffer | [CreateOfferRequest](#mruv.offers.CreateOfferRequest) | [CreateOfferResponse](#mruv.offers.CreateOfferResponse) | Create an offer. |
| GetOffer | [GetOfferRequest](#mruv.offers.GetOfferRequest) | [GetOfferResponse](#mruv.offers.GetOfferResponse) | Get an offer. |
| UpdateOffer | [UpdateOfferRequest](#mruv.offers.UpdateOfferRequest) | [UpdateOfferResponse](#mruv.offers.UpdateOfferResponse) | Update an offer. |
| DeleteOffer | [DeleteOfferRequest](#mruv.offers.DeleteOfferRequest) | [DeleteOfferResponse](#mruv.offers.DeleteOfferResponse) | Delete an offer. |
| AcceptOffer | [AcceptOfferRequest](#mruv.offers.AcceptOfferRequest) | [AcceptOfferResponse](#mruv.offers.AcceptOfferResponse) | Accept an offer and proceed transaction. |

 



<a name="organizations/organizations.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## organizations/organizations.proto



<a name="mruv.organizations.AssignLeaderRequest"></a>

### AssignLeaderRequest
Request message for rpc `AssignLeader`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.organizations.AssignLeaderResponse"></a>

### AssignLeaderResponse
Response message for rpc `AssignLeader`.






<a name="mruv.organizations.CreateOrganizationRequest"></a>

### CreateOrganizationRequest
Request message for rpc `CreateOrganization`.






<a name="mruv.organizations.CreateOrganizationResponse"></a>

### CreateOrganizationResponse
Response message for rpc `CreateOrganization`.






<a name="mruv.organizations.DeleteOrganizationRequest"></a>

### DeleteOrganizationRequest
Request message for rpc `DeleteOrganization`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.organizations.DeleteOrganizationResponse"></a>

### DeleteOrganizationResponse
Response message for rpc `DeleteOrganization`.






<a name="mruv.organizations.GetOrganizationRequest"></a>

### GetOrganizationRequest
Request message for rpc `GetOrganization`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.organizations.GetOrganizationResponse"></a>

### GetOrganizationResponse
Response message for rpc `GetOrganization`.






<a name="mruv.organizations.UnassignLeaderRequest"></a>

### UnassignLeaderRequest
Request message for rpc `UnassignLeader`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.organizations.UnassignLeaderResponse"></a>

### UnassignLeaderResponse
Response message for rpc `UnassignLeader`.






<a name="mruv.organizations.UpdateOrganizationRequest"></a>

### UpdateOrganizationRequest
Request message for rpc `UpdateOrganization`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.organizations.UpdateOrganizationResponse"></a>

### UpdateOrganizationResponse
Response message for rpc `UpdateOrganization`.





 

 

 


<a name="mruv.organizations.MruVOrganizationsService"></a>

### MruVOrganizationsService
The MruV jobs service provides procedures for managing organizations and fractions.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateOrganization | [CreateOrganizationRequest](#mruv.organizations.CreateOrganizationRequest) | [CreateOrganizationResponse](#mruv.organizations.CreateOrganizationResponse) | Create a organization. |
| GetOrganization | [GetOrganizationRequest](#mruv.organizations.GetOrganizationRequest) | [GetOrganizationResponse](#mruv.organizations.GetOrganizationResponse) | Get organization. |
| UpdateOrganization | [UpdateOrganizationRequest](#mruv.organizations.UpdateOrganizationRequest) | [UpdateOrganizationResponse](#mruv.organizations.UpdateOrganizationResponse) | Update organization. |
| DeleteOrganization | [DeleteOrganizationRequest](#mruv.organizations.DeleteOrganizationRequest) | [DeleteOrganizationResponse](#mruv.organizations.DeleteOrganizationResponse) | Delete organization. |
| AssignLeader | [AssignLeaderRequest](#mruv.organizations.AssignLeaderRequest) | [AssignLeaderResponse](#mruv.organizations.AssignLeaderResponse) | Assign an organization leader. Leader is a main administrator of a organization, have all rights to manage organization. If the organization leader already exists, the leader will be overwritten. |
| UnassignLeader | [UnassignLeaderRequest](#mruv.organizations.UnassignLeaderRequest) | [UnassignLeaderResponse](#mruv.organizations.UnassignLeaderResponse) |  |

 



<a name="punishments/punishments.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## punishments/punishments.proto



<a name="mruv.economy.AdminJailMessage"></a>

### AdminJailMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  | A player, that owns a jailed character. |
| character | [uint32](#uint32) |  | Character that has been jailed. |
| reason | [string](#string) |  | An admin jail reason. |
| admin | [uint32](#uint32) |  | Admin that jail a player. 0 = system jail. |
| aj_date | [int64](#int64) |  | Date on which an admin jail was issued in Unix time. |
| jail_time | [uint32](#uint32) |  | Time of admin jail in seconds. |






<a name="mruv.economy.AdminJailRequest"></a>

### AdminJailRequest
Request message for rpc `AdminJail`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [uint32](#uint32) |  |  |
| time | [uint32](#uint32) |  | Admin jail time. |
| reason | [string](#string) |  | Admin jail reason. |
| admin | [uint32](#uint32) |  | Admin that gave an admin jail to a player. |






<a name="mruv.economy.AdminJailResponse"></a>

### AdminJailResponse
Response message for rpc `AdminJail`.






<a name="mruv.economy.BanMessage"></a>

### BanMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| character | [uint32](#uint32) |  |  |
| ip | [string](#string) |  |  |
| expiration_date | [int64](#int64) |  | Expiration date in Unix time. |
| reason | [string](#string) |  | A ban reason. |
| admin | [uint32](#uint32) |  | Admin that banned a player. 0 = system ban. |
| ban_date | [int64](#int64) |  | Date on which a ban was issued in Unix time. |
| active | [bool](#bool) |  | Ban status. True = active, false = deactivated. |
| unban_date | [int64](#int64) |  | Date of unban in Unix time. This field is set only when ban was deactivated. |
| unban_admin | [uint32](#uint32) |  | Admin that deactivated this ban. This field is set only when ban was deactivated. |






<a name="mruv.economy.BanRequest"></a>

### BanRequest
Request message for rpc `Ban`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| character | [uint32](#uint32) |  | Player character that was accused. Optional. |
| ip | [string](#string) |  |  |
| time | [uint32](#uint32) |  | Ban expiration time in days. 0 = permanent ban. |
| reason | [string](#string) |  | Ban reason. |
| admin | [uint32](#uint32) |  | Admin that banned a player. 0 = system ban. |






<a name="mruv.economy.BanResponse"></a>

### BanResponse
Response message for rpc `Ban`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| ban_id | [uint32](#uint32) |  |  |






<a name="mruv.economy.BlockMessage"></a>

### BlockMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  | A player, that owns a blocked character. |
| character | [uint32](#uint32) |  | Blocked character. |
| reason | [string](#string) |  | A block reason. |
| admin | [uint32](#uint32) |  | Admin that blocked a player. 0 = system block. |
| block_date | [int64](#int64) |  | Date on which a block was issued in Unix time. |
| active | [bool](#bool) |  |  |
| unblock_date | [int64](#int64) |  | Date of unblock in Unix time. This field is set only when a block was deactivated. |
| unblock_admin | [uint32](#uint32) |  | An admin that unblocked a player. This field is set only when a block was deactivated. |






<a name="mruv.economy.BlockRequest"></a>

### BlockRequest
Request message for rpc `Block`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [uint32](#uint32) |  |  |
| reason | [string](#string) |  | Block reason. |
| admin | [uint32](#uint32) |  | Admin that blocked a player. 0 = system ban. |






<a name="mruv.economy.BlockResponse"></a>

### BlockResponse
Response message for rpc `Block`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| block_id | [uint32](#uint32) |  |  |






<a name="mruv.economy.GetBanRequest"></a>

### GetBanRequest
Request message for rpc `GetBan`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.economy.GetBlockRequest"></a>

### GetBlockRequest
Request message for rpc `GetBlock`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.economy.GetPlayerAdminJailRequest"></a>

### GetPlayerAdminJailRequest
Request message for rpc `GetPlayerAdminJail`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [uint32](#uint32) |  |  |






<a name="mruv.economy.GetPlayerAdminJailResponse"></a>

### GetPlayerAdminJailResponse
Response message for rpc `GetPlayerAdminJail`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| jail_time | [uint32](#uint32) |  | Time of admin jail in seconds. |
| reason | [string](#string) |  | Admin jail reason. |
| admin | [uint32](#uint32) |  | An admin that put a player in the admin jail. |
| date | [int64](#int64) |  | Date when the player was thrown into admin jail in Unix time. |






<a name="mruv.economy.GetPlayerBansRequest"></a>

### GetPlayerBansRequest
Request message for rpc `GetPlayerBans`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| ip | [string](#string) |  |  |






<a name="mruv.economy.GetPlayerBansResponse"></a>

### GetPlayerBansResponse
Response message for rpc `GetPlayerBans`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| bans | [BanMessage](#mruv.economy.BanMessage) | repeated |  |






<a name="mruv.economy.GetPlayerWarnsRequest"></a>

### GetPlayerWarnsRequest
Request message for rpc `GetPlayerWarns`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |






<a name="mruv.economy.GetPlayerWarnsResponse"></a>

### GetPlayerWarnsResponse
Response message for rpc `GetPlayerWarns`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| warns | [WarnMessage](#mruv.economy.WarnMessage) | repeated |  |






<a name="mruv.economy.GetWarnRequest"></a>

### GetWarnRequest
Request message for rpc `GetWarn`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.economy.IsCharacterBlockedRequest"></a>

### IsCharacterBlockedRequest
Request message for rpc `IsCharacterBlocked`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [uint32](#uint32) |  |  |






<a name="mruv.economy.IsCharacterBlockedResponse"></a>

### IsCharacterBlockedResponse
Response message for rpc `IsCharacterBlocked`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| blocked | [bool](#bool) |  |  |
| block_id | [uint32](#uint32) |  |  |






<a name="mruv.economy.IsCharacterJailedRequest"></a>

### IsCharacterJailedRequest
Request message for rpc `IsCharacterJailed`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [uint32](#uint32) |  |  |






<a name="mruv.economy.IsCharacterJailedResponse"></a>

### IsCharacterJailedResponse
Response message for rpc `IsCharacterJailed`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| jailed | [bool](#bool) |  |  |
| jail_time | [uint32](#uint32) |  |  |






<a name="mruv.economy.IsPlayerBannedRequest"></a>

### IsPlayerBannedRequest
Request message for rpc `IsPlayerBanned`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| ip | [string](#string) |  |  |






<a name="mruv.economy.IsPlayerBannedResponse"></a>

### IsPlayerBannedResponse
Response message for rpc `IsPlayerBanned`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| banned | [bool](#bool) |  |  |
| ban_id | [uint32](#uint32) |  |  |






<a name="mruv.economy.MuteGlobalChatsRequest"></a>

### MuteGlobalChatsRequest
Request message for rpc `MuteGlobalChats`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| account | [uint32](#uint32) |  |  |






<a name="mruv.economy.MuteGlobalChatsResponse"></a>

### MuteGlobalChatsResponse
Response message for rpc `MuteGlobalChats`.






<a name="mruv.economy.UnAdminJailMessage"></a>

### UnAdminJailMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| character | [uint32](#uint32) |  |  |






<a name="mruv.economy.UnAdminJailRequest"></a>

### UnAdminJailRequest
Request message for rpc `UnAdminJail`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [uint32](#uint32) |  |  |






<a name="mruv.economy.UnAdminJailResponse"></a>

### UnAdminJailResponse
Response message for rpc `UnAdminJail`.






<a name="mruv.economy.UnBanMessage"></a>

### UnBanMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| ban_id | [uint32](#uint32) |  |  |






<a name="mruv.economy.UnBanRequest"></a>

### UnBanRequest
Request message for rpc `UnBan`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| ban_id | [uint32](#uint32) |  |  |






<a name="mruv.economy.UnBanResponse"></a>

### UnBanResponse
Response message for rpc `UnBan`.






<a name="mruv.economy.UnBlockMessage"></a>

### UnBlockMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| block_id | [uint32](#uint32) |  |  |






<a name="mruv.economy.UnMuteGlobalChatsRequest"></a>

### UnMuteGlobalChatsRequest
Request message for rpc `UnMuteGlobalChats`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| account | [uint32](#uint32) |  |  |






<a name="mruv.economy.UnMuteGlobalChatsResponse"></a>

### UnMuteGlobalChatsResponse
Response message for rpc `UnMuteGlobalChats`.






<a name="mruv.economy.UnWarnMessage"></a>

### UnWarnMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| warn_id | [uint32](#uint32) |  |  |






<a name="mruv.economy.UnWarnRequest"></a>

### UnWarnRequest
Request message for rpc `UnWarn`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| warn_id | [uint32](#uint32) |  |  |






<a name="mruv.economy.UnWarnResponse"></a>

### UnWarnResponse
Response message for rpc `UnWarn`.






<a name="mruv.economy.WarnMessage"></a>

### WarnMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| character | [uint32](#uint32) |  | A character, that was given a warning. |
| expiration_date | [int64](#int64) |  | Expiration date in Unix time. |
| reason | [string](#string) |  | A warn reason. |
| admin | [uint32](#uint32) |  | Admin that warned a player. 0 = system warn. |
| warn_date | [int64](#int64) |  | Date on which a warn was issued in Unix time. |
| active | [bool](#bool) |  | Warn status. True = active, false = deactivated. |
| unwarn_date | [int64](#int64) |  | Date of unwarn in Unix time. This field is set only when warn was deactivated. |
| unwarn_admin | [uint32](#uint32) |  | Admin that deactivated a warn. This field is set only when warn was deactivated. |






<a name="mruv.economy.WarnRequest"></a>

### WarnRequest
Request message for rpc `Warn`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| character | [uint32](#uint32) |  | Player character that was accused. Optional. |
| time | [uint32](#uint32) |  | Warn expiration time in days. 0 = permanent warn. |
| reason | [string](#string) |  | Warn reason. |
| admin | [uint32](#uint32) |  | Admin that warned player. 0 = system warn. |






<a name="mruv.economy.WarnResponse"></a>

### WarnResponse
Response message for rpc `Warn`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| warn_id | [uint32](#uint32) |  |  |






<a name="mruv.economy.WatchAdminJailsRequest"></a>

### WatchAdminJailsRequest
Request message for rpc `WatchAdminJails`.






<a name="mruv.economy.WatchBansRequest"></a>

### WatchBansRequest
Request message for rpc `WatchBans`.






<a name="mruv.economy.WatchBlocksRequest"></a>

### WatchBlocksRequest
Request message for rpc `WatchBlocks`.






<a name="mruv.economy.WatchPlayerAcquittalsRequest"></a>

### WatchPlayerAcquittalsRequest
Request message for rpc `WatchPlayerAcquittals`.






<a name="mruv.economy.WatchPlayerAcquittalsResponse"></a>

### WatchPlayerAcquittalsResponse
Response message for rpc `WatchPlayerAcquittals`.






<a name="mruv.economy.WatchPlayerPunishmentsRequest"></a>

### WatchPlayerPunishmentsRequest
Request message for rpc `WatchPlayerPunishments`.






<a name="mruv.economy.WatchPlayerPunishmentsResponse"></a>

### WatchPlayerPunishmentsResponse
Response message for rpc `WatchPlayerPunishments`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| type | [PunishmentType](#mruv.economy.PunishmentType) |  |  |
| punishment_id | [uint32](#uint32) |  |  |






<a name="mruv.economy.WatchPunishmentsRequest"></a>

### WatchPunishmentsRequest
Request message for rpc `WatchPunishments`.






<a name="mruv.economy.WatchPunishmentsResponse"></a>

### WatchPunishmentsResponse
Response message for rpc `WatchPunishments`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| type | [PunishmentType](#mruv.economy.PunishmentType) |  |  |
| punishment_id | [uint32](#uint32) |  |  |
| player | [uint32](#uint32) |  |  |
| character | [uint32](#uint32) |  |  |






<a name="mruv.economy.WatchUnAdminJailsRequest"></a>

### WatchUnAdminJailsRequest
Request message for rpc `WatchUnAdminJails`.






<a name="mruv.economy.WatchUnBansRequest"></a>

### WatchUnBansRequest
Request message for rpc `WatchUnBans`.






<a name="mruv.economy.WatchUnBlocksRequest"></a>

### WatchUnBlocksRequest
Request message for rpc `WatchUnBlocks`.






<a name="mruv.economy.WatchUnWarnsRequest"></a>

### WatchUnWarnsRequest
Request message for rpc `WatchUnWarns`.






<a name="mruv.economy.WatchWarnsRequest"></a>

### WatchWarnsRequest
Request message for rpc `WatchWarns`.





 


<a name="mruv.economy.AcquittalsType"></a>

### AcquittalsType


| Name | Number | Description |
| ---- | ------ | ----------- |
| UNKNOWN_ACQUITAL | 0 |  |
| UNBAN | 1 |  |
| UNBLOCK | 2 |  |
| UNWARN | 3 |  |
| UN_ADMIN_JAIL | 4 |  |



<a name="mruv.economy.PunishmentType"></a>

### PunishmentType


| Name | Number | Description |
| ---- | ------ | ----------- |
| UNKNOWN_PUNISHMENT | 0 |  |
| BAN | 1 |  |
| BLOCK | 2 |  |
| WARN | 3 |  |
| ADMIN_JAIL | 4 |  |


 

 


<a name="mruv.economy.MruVPunishmentsService"></a>

### MruVPunishmentsService
This service provides interface for managing punishments for players.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| Ban | [BanRequest](#mruv.economy.BanRequest) | [BanResponse](#mruv.economy.BanResponse) | Ban player on account and/or ip. If ban_time is 0, ban will never expire. |
| Block | [BlockRequest](#mruv.economy.BlockRequest) | [BlockResponse](#mruv.economy.BlockResponse) | Block player character. |
| Warn | [WarnRequest](#mruv.economy.WarnRequest) | [WarnResponse](#mruv.economy.WarnResponse) | Warn player. If warn_time is 0, warn will never expire. |
| AdminJail | [AdminJailRequest](#mruv.economy.AdminJailRequest) | [AdminJailResponse](#mruv.economy.AdminJailResponse) | Put player in an admin jail. |
| MuteGlobalChats | [MuteGlobalChatsRequest](#mruv.economy.MuteGlobalChatsRequest) | [MuteGlobalChatsResponse](#mruv.economy.MuteGlobalChatsResponse) | Mute player global chats. |
| UnBan | [UnBanRequest](#mruv.economy.UnBanRequest) | [UnBanResponse](#mruv.economy.UnBanResponse) | Deactivate a specific player ban. |
| UnWarn | [UnWarnRequest](#mruv.economy.UnWarnRequest) | [UnWarnResponse](#mruv.economy.UnWarnResponse) | Deactivate a specific player warning. If a player was banned by reaching the warning limit, a player will be unbanned. |
| UnAdminJail | [UnAdminJailRequest](#mruv.economy.UnAdminJailRequest) | [UnAdminJailResponse](#mruv.economy.UnAdminJailResponse) | Remove player from admin jail. |
| UnMuteGlobalChats | [UnMuteGlobalChatsRequest](#mruv.economy.UnMuteGlobalChatsRequest) | [UnMuteGlobalChatsResponse](#mruv.economy.UnMuteGlobalChatsResponse) |  |
| GetPlayerBans | [GetPlayerBansRequest](#mruv.economy.GetPlayerBansRequest) | [GetPlayerBansResponse](#mruv.economy.GetPlayerBansResponse) | Get all player bans. |
| GetPlayerWarns | [GetPlayerWarnsRequest](#mruv.economy.GetPlayerWarnsRequest) | [GetPlayerWarnsResponse](#mruv.economy.GetPlayerWarnsResponse) | Get all player warns. |
| GetPlayerAdminJail | [GetPlayerAdminJailRequest](#mruv.economy.GetPlayerAdminJailRequest) | [GetPlayerAdminJailResponse](#mruv.economy.GetPlayerAdminJailResponse) | Get player admin jail time. |
| GetBan | [GetBanRequest](#mruv.economy.GetBanRequest) | [BanMessage](#mruv.economy.BanMessage) | Get ban info. |
| GetWarn | [GetWarnRequest](#mruv.economy.GetWarnRequest) | [WarnMessage](#mruv.economy.WarnMessage) | Get warn info. |
| GetBlock | [GetBlockRequest](#mruv.economy.GetBlockRequest) | [BlockMessage](#mruv.economy.BlockMessage) | Get block info. |
| IsPlayerBanned | [IsPlayerBannedRequest](#mruv.economy.IsPlayerBannedRequest) | [IsPlayerBannedResponse](#mruv.economy.IsPlayerBannedResponse) | Check is player or ip banned. |
| IsCharacterBlocked | [IsCharacterBlockedRequest](#mruv.economy.IsCharacterBlockedRequest) | [IsCharacterBlockedResponse](#mruv.economy.IsCharacterBlockedResponse) | Check is character is blocked. |
| IsCharacterJailed | [IsCharacterJailedRequest](#mruv.economy.IsCharacterJailedRequest) | [IsCharacterJailedResponse](#mruv.economy.IsCharacterJailedResponse) |  |
| WatchBans | [WatchBansRequest](#mruv.economy.WatchBansRequest) | [BanMessage](#mruv.economy.BanMessage) stream | Subscribe to ban events. |
| WatchBlocks | [WatchBlocksRequest](#mruv.economy.WatchBlocksRequest) | [BlockMessage](#mruv.economy.BlockMessage) stream | Subscribe to block events. |
| WatchWarns | [WatchWarnsRequest](#mruv.economy.WatchWarnsRequest) | [WarnMessage](#mruv.economy.WarnMessage) stream | Subscribe to warn events. |
| WatchAdminJails | [WatchAdminJailsRequest](#mruv.economy.WatchAdminJailsRequest) | [AdminJailMessage](#mruv.economy.AdminJailMessage) stream | Subscribe to admin jail events. |
| WatchUnBans | [WatchUnBansRequest](#mruv.economy.WatchUnBansRequest) | [UnBanMessage](#mruv.economy.UnBanMessage) stream | Subscribe to unban events. |
| WatchUnBlocks | [WatchUnBlocksRequest](#mruv.economy.WatchUnBlocksRequest) | [UnBlockMessage](#mruv.economy.UnBlockMessage) stream | Subscribe to unblock events. |
| WatchUnWarns | [WatchUnWarnsRequest](#mruv.economy.WatchUnWarnsRequest) | [UnWarnMessage](#mruv.economy.UnWarnMessage) stream | Subscribe to unwarn events. |
| WatchUnAdminJails | [WatchUnAdminJailsRequest](#mruv.economy.WatchUnAdminJailsRequest) | [UnAdminJailMessage](#mruv.economy.UnAdminJailMessage) stream | Subscribe to admin jail release events. |
| WatchPlayerPunishments | [WatchPlayerPunishmentsRequest](#mruv.economy.WatchPlayerPunishmentsRequest) | [WatchPlayerPunishmentsResponse](#mruv.economy.WatchPlayerPunishmentsResponse) stream | Subscribe to player punishments. |
| WatchPlayerAcquittals | [WatchPlayerAcquittalsRequest](#mruv.economy.WatchPlayerAcquittalsRequest) | [WatchPlayerAcquittalsResponse](#mruv.economy.WatchPlayerAcquittalsResponse) stream | Subscribe to player acquittals. |
| WatchPunishments | [WatchPunishmentsRequest](#mruv.economy.WatchPunishmentsRequest) | [WatchPunishmentsResponse](#mruv.economy.WatchPunishmentsResponse) stream | Subscribe to all punishments and acquittals events. |

 



<a name="server/server.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## server/server.proto



<a name="mruv.server.GetRegisteredServersRequest"></a>

### GetRegisteredServersRequest
Request message for `MruVServerService.GetRegisteredServers`.






<a name="mruv.server.GetRegisteredServersResponse"></a>

### GetRegisteredServersResponse
Response message for `MruVServerService.GetRegisteredServers`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| servers | [ServerInfo](#mruv.server.ServerInfo) | repeated |  |






<a name="mruv.server.ServerEvent"></a>

### ServerEvent
Server event.
Response message for `MruVServerService.ServerEventsStream`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| type | [ServerEvent.ServerEventType](#mruv.server.ServerEvent.ServerEventType) |  | Type of a server event. |






<a name="mruv.server.ServerEventsStreamRequest"></a>

### ServerEventsStreamRequest
Request message for `MruVServerService.ServerEventsStream`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  | The ID of the server from which we want to receive events. |






<a name="mruv.server.UpdateServerStatusRequest"></a>

### UpdateServerStatusRequest
Request message for `MruVServerService.UpdateServerStatus`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  | Id of the server. |
| status | [ServerStatus](#mruv.server.ServerStatus) |  | Status of the server. |
| players | [uint32](#uint32) |  | How many players are registered on that server. |






<a name="mruv.server.UpdateServerStatusResponse"></a>

### UpdateServerStatusResponse
Response message for `MruVServerService.UpdateServerStatus`.





 


<a name="mruv.server.ServerEvent.ServerEventType"></a>

### ServerEvent.ServerEventType
Types of server events.

| Name | Number | Description |
| ---- | ------ | ----------- |
| UNKNOWN | 0 |  |
| REGISTERED | 1 |  |
| SERVER_DOWN | 2 |  |
| SERVER_UP | 3 |  |
| PLAYERS_CHANGED | 4 |  |


 

 


<a name="mruv.server.MruVServerService"></a>

### MruVServerService
The MruV server service provides procedures for managing game platform server actions.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| RegisterServer | [ServerInfo](#mruv.server.ServerInfo) | [ServerID](#mruv.server.ServerID) | Register instance of server for further managing. |
| GetRegisteredServers | [GetRegisteredServersRequest](#mruv.server.GetRegisteredServersRequest) | [GetRegisteredServersResponse](#mruv.server.GetRegisteredServersResponse) | Get all registered servers. |
| GetServerInfo | [ServerID](#mruv.server.ServerID) | [ServerInfo](#mruv.server.ServerInfo) | Get game server status. |
| UpdateServerStatus | [UpdateServerStatusRequest](#mruv.server.UpdateServerStatusRequest) | [UpdateServerStatusResponse](#mruv.server.UpdateServerStatusResponse) | Update game server status. |
| ServerEventsStream | [ServerEventsStreamRequest](#mruv.server.ServerEventsStreamRequest) | [ServerEvent](#mruv.server.ServerEvent) stream | Stream of server events. Events are streamed back in real-time for chosen server. TODO: Change name to: SubscribeServerEvents |

 



<a name="server/server_model.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## server/server_model.proto



<a name="mruv.server.ServerID"></a>

### ServerID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.server.ServerInfo"></a>

### ServerInfo
Data that describe server.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  | Id of the server. |
| name | [string](#string) |  | Short name of the server. |
| host | [string](#string) |  | Host (ip) of the server. |
| port | [string](#string) |  | Port of the server. |
| platform | [string](#string) |  | Platform of the server. |
| status | [ServerStatus](#mruv.server.ServerStatus) |  | Status of the server. |
| players | [uint32](#uint32) |  | How many players are playing on the server. |





 


<a name="mruv.server.ServerStatus"></a>

### ServerStatus


| Name | Number | Description |
| ---- | ------ | ----------- |
| UNKNOWN | 0 |  |
| ON | 1 |  |
| OFF | 2 |  |


 

 

 



<a name="vehicles/vehicles.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## vehicles/vehicles.proto



<a name="mruv.vehicles.CreateVehicleRequest"></a>

### CreateVehicleRequest
Request message for rpc `CreateVehicle`.






<a name="mruv.vehicles.CreateVehicleResponse"></a>

### CreateVehicleResponse
Response message for rpc `CreateVehicle`.






<a name="mruv.vehicles.DeleteVehicleRequest"></a>

### DeleteVehicleRequest
Request message for rpc `DeleteVehicle`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.vehicles.DeleteVehicleResponse"></a>

### DeleteVehicleResponse
Response message for rpc `DeleteVehicle`.






<a name="mruv.vehicles.GetVehicleRequest"></a>

### GetVehicleRequest
Request message for rpc `GetVehicle`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.vehicles.GetVehicleResponse"></a>

### GetVehicleResponse
Response message for rpc `GetVehicle`.






<a name="mruv.vehicles.UpdateVehicleRequest"></a>

### UpdateVehicleRequest
Request message for rpc `UpdateVehicle`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.vehicles.UpdateVehicleResponse"></a>

### UpdateVehicleResponse
Response message for rpc `UpdateVehicle`.





 

 

 


<a name="mruv.vehicles.MruVVehiclesService"></a>

### MruVVehiclesService
The MruV vehicles service provides procedures for managing vehicles.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateVehicle | [CreateVehicleRequest](#mruv.vehicles.CreateVehicleRequest) | [CreateVehicleResponse](#mruv.vehicles.CreateVehicleResponse) | Create a vehicle. |
| GetVehicle | [GetVehicleRequest](#mruv.vehicles.GetVehicleRequest) | [GetVehicleResponse](#mruv.vehicles.GetVehicleResponse) | Get a vehicle. |
| UpdateVehicle | [UpdateVehicleRequest](#mruv.vehicles.UpdateVehicleRequest) | [UpdateVehicleResponse](#mruv.vehicles.UpdateVehicleResponse) | Update a vehicle. |
| DeleteVehicle | [DeleteVehicleRequest](#mruv.vehicles.DeleteVehicleRequest) | [DeleteVehicleResponse](#mruv.vehicles.DeleteVehicleResponse) | Delete a vehicle. |

 



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

