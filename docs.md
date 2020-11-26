# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [accounts/accounts.proto](#accounts/accounts.proto)
    - [GetAccountCharactersRequest](#mruv.accounts.GetAccountCharactersRequest)
    - [GetAccountCharactersResponse](#mruv.accounts.GetAccountCharactersResponse)
    - [GetAccountRequest](#mruv.accounts.GetAccountRequest)
    - [GetAccountResponse](#mruv.accounts.GetAccountResponse)
    - [IsAccountExistRequest](#mruv.accounts.IsAccountExistRequest)
    - [IsAccountExistResponse](#mruv.accounts.IsAccountExistResponse)
    - [LogInRequest](#mruv.accounts.LogInRequest)
    - [LogInResponse](#mruv.accounts.LogInResponse)
    - [RegisterAccountRequest](#mruv.accounts.RegisterAccountRequest)
    - [RegisterAccountResponse](#mruv.accounts.RegisterAccountResponse)
  
  
  
    - [MruVAccountsService](#mruv.accounts.MruVAccountsService)
  

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
    - [ChangeClothesRequest](#mruv.characters.ChangeClothesRequest)
    - [ChangeClothesResponse](#mruv.characters.ChangeClothesResponse)
    - [Character](#mruv.characters.Character)
    - [CharacterID](#mruv.characters.CharacterID)
    - [CreateCharacterRequest](#mruv.characters.CreateCharacterRequest)
    - [CreateCharacterResponse](#mruv.characters.CreateCharacterResponse)
    - [DeathStreamRequest](#mruv.characters.DeathStreamRequest)
    - [DeathStreamResponse](#mruv.characters.DeathStreamResponse)
    - [DeleteCharacterRequest](#mruv.characters.DeleteCharacterRequest)
    - [DeleteCharacterResponse](#mruv.characters.DeleteCharacterResponse)
    - [GetCharacterRequest](#mruv.characters.GetCharacterRequest)
    - [GetCharacterResponse](#mruv.characters.GetCharacterResponse)
    - [UpdateCharacterRequest](#mruv.characters.UpdateCharacterRequest)
    - [UpdateCharacterResponse](#mruv.characters.UpdateCharacterResponse)
  
    - [DeathType](#mruv.characters.DeathType)
  
  
    - [MruVCharactersService](#mruv.characters.MruVCharactersService)
  

- [common/health.proto](#common/health.proto)
    - [ServiceStatusRequest](#mruv.common.ServiceStatusRequest)
    - [ServiceStatusResponse](#mruv.common.ServiceStatusResponse)
    - [VersionRequest](#mruv.common.VersionRequest)
    - [VersionResponse](#mruv.common.VersionResponse)
  
  
  
  

- [common/spatial.proto](#common/spatial.proto)
    - [Position](#mruv.common.Position)
    - [Rotation](#mruv.common.Rotation)
  
  
  
  

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
  

- [elevators/elevators.proto](#elevators/elevators.proto)
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
  

- [entrances/entrances.proto](#entrances/entrances.proto)
    - [CreateEntranceRequest](#mruv.entrances.CreateEntranceRequest)
    - [CreateEntranceResponse](#mruv.entrances.CreateEntranceResponse)
    - [DeleteEntranceRequest](#mruv.entrances.DeleteEntranceRequest)
    - [DeleteEntranceResponse](#mruv.entrances.DeleteEntranceResponse)
    - [EnterRequest](#mruv.entrances.EnterRequest)
    - [EnterResponse](#mruv.entrances.EnterResponse)
    - [Entrance](#mruv.entrances.Entrance)
    - [ExitRequest](#mruv.entrances.ExitRequest)
    - [ExitResponse](#mruv.entrances.ExitResponse)
    - [FetchAllEntrancesRequest](#mruv.entrances.FetchAllEntrancesRequest)
    - [FetchAllEntrancesResponse](#mruv.entrances.FetchAllEntrancesResponse)
    - [FetchAllEntrancesResponse.EntrancesEntry](#mruv.entrances.FetchAllEntrancesResponse.EntrancesEntry)
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
    - [Estate](#mruv.estates.Estate)
    - [FetchAllEstatesRequest](#mruv.estates.FetchAllEstatesRequest)
    - [FetchAllEstatesResponse](#mruv.estates.FetchAllEstatesResponse)
    - [FullEstate](#mruv.estates.FullEstate)
    - [FullEstate.EntrancesEntry](#mruv.estates.FullEstate.EntrancesEntry)
    - [FullEstate.GatesEntry](#mruv.estates.FullEstate.GatesEntry)
    - [FullEstate.ObjectsEntry](#mruv.estates.FullEstate.ObjectsEntry)
    - [FullEstate.RemovedBuildingsEntry](#mruv.estates.FullEstate.RemovedBuildingsEntry)
    - [GetEstateEntrancesRequest](#mruv.estates.GetEstateEntrancesRequest)
    - [GetEstateEntrancesResponse](#mruv.estates.GetEstateEntrancesResponse)
    - [GetEstateGatesRequest](#mruv.estates.GetEstateGatesRequest)
    - [GetEstateGatesResponse](#mruv.estates.GetEstateGatesResponse)
    - [GetEstateRequest](#mruv.estates.GetEstateRequest)
    - [GetEstatesRequest](#mruv.estates.GetEstatesRequest)
    - [GetEstatesResponse](#mruv.estates.GetEstatesResponse)
    - [RemoveEntranceRequest](#mruv.estates.RemoveEntranceRequest)
    - [RemoveEntranceResponse](#mruv.estates.RemoveEntranceResponse)
    - [RemoveGateRequest](#mruv.estates.RemoveGateRequest)
    - [RemoveGateResponse](#mruv.estates.RemoveGateResponse)
    - [UpdateEstateRequest](#mruv.estates.UpdateEstateRequest)
    - [UpdateEstateResponse](#mruv.estates.UpdateEstateResponse)
  
  
  
    - [MruVEstateService](#mruv.estates.MruVEstateService)
  

- [gates/gates.proto](#gates/gates.proto)
    - [CloseRequest](#mruv.gates.CloseRequest)
    - [CloseResponse](#mruv.gates.CloseResponse)
    - [CreateGateRequest](#mruv.gates.CreateGateRequest)
    - [CreateGateResponse](#mruv.gates.CreateGateResponse)
    - [DeleteGateRequest](#mruv.gates.DeleteGateRequest)
    - [DeleteGateResponse](#mruv.gates.DeleteGateResponse)
    - [FetchAllGatesRequest](#mruv.gates.FetchAllGatesRequest)
    - [FetchAllGatesResponse](#mruv.gates.FetchAllGatesResponse)
    - [FetchAllGatesResponse.GatesEntry](#mruv.gates.FetchAllGatesResponse.GatesEntry)
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
    - [AddMemberRequest](#mruv.groups.AddMemberRequest)
    - [AddMemberResponse](#mruv.groups.AddMemberResponse)
    - [AddPermissionRequest](#mruv.groups.AddPermissionRequest)
    - [AddPermissionResponse](#mruv.groups.AddPermissionResponse)
    - [AddSubgroupRequest](#mruv.groups.AddSubgroupRequest)
    - [AddSubgroupResponse](#mruv.groups.AddSubgroupResponse)
    - [AssignOwnerRequest](#mruv.groups.AssignOwnerRequest)
    - [AssignOwnerResponse](#mruv.groups.AssignOwnerResponse)
    - [CreateGroupRequest](#mruv.groups.CreateGroupRequest)
    - [CreateGroupResponse](#mruv.groups.CreateGroupResponse)
    - [DeleteGroupRequest](#mruv.groups.DeleteGroupRequest)
    - [DeleteGroupResponse](#mruv.groups.DeleteGroupResponse)
    - [GetGroupRequest](#mruv.groups.GetGroupRequest)
    - [GetGroupResponse](#mruv.groups.GetGroupResponse)
    - [GetGroupsRequest](#mruv.groups.GetGroupsRequest)
    - [GetGroupsResponse](#mruv.groups.GetGroupsResponse)
    - [GetGroupsResponse.Group](#mruv.groups.GetGroupsResponse.Group)
    - [GetMembersRequest](#mruv.groups.GetMembersRequest)
    - [GetMembersResponse](#mruv.groups.GetMembersResponse)
    - [GetOwnerRequest](#mruv.groups.GetOwnerRequest)
    - [GetOwnerResponse](#mruv.groups.GetOwnerResponse)
    - [GetPermissionsRequest](#mruv.groups.GetPermissionsRequest)
    - [GetPermissionsResponse](#mruv.groups.GetPermissionsResponse)
    - [GetPermissionsResponse.Permission](#mruv.groups.GetPermissionsResponse.Permission)
    - [GetSubgroupsRequest](#mruv.groups.GetSubgroupsRequest)
    - [GetSubgroupsResponse](#mruv.groups.GetSubgroupsResponse)
    - [IsPermittedRequest](#mruv.groups.IsPermittedRequest)
    - [IsPermittedResponse](#mruv.groups.IsPermittedResponse)
    - [RemoveMemberRequest](#mruv.groups.RemoveMemberRequest)
    - [RemoveMemberResponse](#mruv.groups.RemoveMemberResponse)
    - [RemovePermissionRequest](#mruv.groups.RemovePermissionRequest)
    - [RemovePermissionResponse](#mruv.groups.RemovePermissionResponse)
    - [RemoveSubgroupRequest](#mruv.groups.RemoveSubgroupRequest)
    - [RemoveSubgroupResponse](#mruv.groups.RemoveSubgroupResponse)
    - [UpdateGroupRequest](#mruv.groups.UpdateGroupRequest)
    - [UpdateGroupResponse](#mruv.groups.UpdateGroupResponse)
  
    - [MemberType](#mruv.groups.MemberType)
    - [OwnerType](#mruv.groups.OwnerType)
  
  
    - [MruVGroupsService](#mruv.groups.MruVGroupsService)
  

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
    - [GetContainerItemsRequest](#mruv.items.GetContainerItemsRequest)
    - [GetContainerItemsResponse](#mruv.items.GetContainerItemsResponse)
    - [GetContainerTypesRequest](#mruv.items.GetContainerTypesRequest)
    - [GetContainerTypesResponse](#mruv.items.GetContainerTypesResponse)
    - [GetContainersRequest](#mruv.items.GetContainersRequest)
    - [GetContainersResponse](#mruv.items.GetContainersResponse)
    - [GetItemTypesRequest](#mruv.items.GetItemTypesRequest)
    - [GetItemTypesResponse](#mruv.items.GetItemTypesResponse)
    - [GetItemsRequest](#mruv.items.GetItemsRequest)
    - [GetItemsResponse](#mruv.items.GetItemsResponse)
    - [GetNearestItemsRequest](#mruv.items.GetNearestItemsRequest)
    - [GetNearestItemsResponse](#mruv.items.GetNearestItemsResponse)
    - [PullItemRequest](#mruv.items.PullItemRequest)
    - [PutItemRequest](#mruv.items.PutItemRequest)
    - [PutItemResponse](#mruv.items.PutItemResponse)
    - [SortItemsRequest](#mruv.items.SortItemsRequest)
    - [SortItemsResponse](#mruv.items.SortItemsResponse)
    - [UseItemRequest](#mruv.items.UseItemRequest)
    - [UseItemResponse](#mruv.items.UseItemResponse)
  
  
  
    - [MruVItemService](#mruv.items.MruVItemService)
  

- [items/items_model.proto](#items/items_model.proto)
    - [Container](#mruv.items.Container)
    - [ContainerID](#mruv.items.ContainerID)
    - [ContainerType](#mruv.items.ContainerType)
    - [ContainerTypeID](#mruv.items.ContainerTypeID)
    - [InsideItem](#mruv.items.InsideItem)
    - [Item](#mruv.items.Item)
    - [ItemID](#mruv.items.ItemID)
    - [ItemType](#mruv.items.ItemType)
    - [ItemTypeID](#mruv.items.ItemTypeID)
  
    - [SortingMode](#mruv.items.SortingMode)
  
  
  

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
  

- [objects/models.proto](#objects/models.proto)
    - [CreateObjectModelRequest](#mruv.objects.CreateObjectModelRequest)
    - [CreateObjectModelResponse](#mruv.objects.CreateObjectModelResponse)
    - [DeleteObjectModelRequest](#mruv.objects.DeleteObjectModelRequest)
    - [DeleteObjectModelResponse](#mruv.objects.DeleteObjectModelResponse)
    - [FetchAllModelsRequest](#mruv.objects.FetchAllModelsRequest)
    - [FetchAllModelsResponse](#mruv.objects.FetchAllModelsResponse)
    - [FetchAllModelsResponse.ModelsEntry](#mruv.objects.FetchAllModelsResponse.ModelsEntry)
    - [GetObjectModelRequest](#mruv.objects.GetObjectModelRequest)
    - [GetObjectModelResponse](#mruv.objects.GetObjectModelResponse)
    - [ObjectModel](#mruv.objects.ObjectModel)
    - [UpdateObjectModelRequest](#mruv.objects.UpdateObjectModelRequest)
    - [UpdateObjectModelResponse](#mruv.objects.UpdateObjectModelResponse)
  
  
  
    - [MruVObjectModelsService](#mruv.objects.MruVObjectModelsService)
  

- [objects/movable.proto](#objects/movable.proto)
    - [CreateMovableObjectRequest](#mruv.objects.CreateMovableObjectRequest)
    - [CreateMovableObjectResponse](#mruv.objects.CreateMovableObjectResponse)
    - [DeleteMovableObjectRequest](#mruv.objects.DeleteMovableObjectRequest)
    - [DeleteMovableObjectResponse](#mruv.objects.DeleteMovableObjectResponse)
    - [FetchAllMovableObjectsRequest](#mruv.objects.FetchAllMovableObjectsRequest)
    - [FetchAllMovableObjectsResponse](#mruv.objects.FetchAllMovableObjectsResponse)
    - [FetchAllMovableObjectsResponse.MovableObjectsEntry](#mruv.objects.FetchAllMovableObjectsResponse.MovableObjectsEntry)
    - [GetMovableObjectRequest](#mruv.objects.GetMovableObjectRequest)
    - [GetMovableObjectResponse](#mruv.objects.GetMovableObjectResponse)
    - [MovableObject](#mruv.objects.MovableObject)
    - [MoveObjectNextRequest](#mruv.objects.MoveObjectNextRequest)
    - [MoveObjectNextResponse](#mruv.objects.MoveObjectNextResponse)
    - [MoveObjectPreviousRequest](#mruv.objects.MoveObjectPreviousRequest)
    - [MoveObjectPreviousResponse](#mruv.objects.MoveObjectPreviousResponse)
    - [MoveObjectRequest](#mruv.objects.MoveObjectRequest)
    - [MoveObjectResponse](#mruv.objects.MoveObjectResponse)
    - [State](#mruv.objects.State)
    - [UpdateMovableObjectRequest](#mruv.objects.UpdateMovableObjectRequest)
    - [UpdateMovableObjectResponse](#mruv.objects.UpdateMovableObjectResponse)
  
  
  
    - [MruVMovableObjectsService](#mruv.objects.MruVMovableObjectsService)
  

- [objects/objects.proto](#objects/objects.proto)
    - [AddObjectMaterialRequest](#mruv.objects.AddObjectMaterialRequest)
    - [AddObjectMaterialResponse](#mruv.objects.AddObjectMaterialResponse)
    - [AddObjectMaterialTextRequest](#mruv.objects.AddObjectMaterialTextRequest)
    - [AddObjectMaterialTextResponse](#mruv.objects.AddObjectMaterialTextResponse)
    - [AddRemoveBuildingRequest](#mruv.objects.AddRemoveBuildingRequest)
    - [AddRemoveBuildingResponse](#mruv.objects.AddRemoveBuildingResponse)
    - [CreateObjectRequest](#mruv.objects.CreateObjectRequest)
    - [CreateObjectResponse](#mruv.objects.CreateObjectResponse)
    - [DeleteObjectMaterialRequest](#mruv.objects.DeleteObjectMaterialRequest)
    - [DeleteObjectMaterialResponse](#mruv.objects.DeleteObjectMaterialResponse)
    - [DeleteObjectMaterialTextRequest](#mruv.objects.DeleteObjectMaterialTextRequest)
    - [DeleteObjectMaterialTextResponse](#mruv.objects.DeleteObjectMaterialTextResponse)
    - [DeleteObjectRequest](#mruv.objects.DeleteObjectRequest)
    - [DeleteObjectResponse](#mruv.objects.DeleteObjectResponse)
    - [DeleteRemoveBuildingRequest](#mruv.objects.DeleteRemoveBuildingRequest)
    - [DeleteRemoveBuildingResponse](#mruv.objects.DeleteRemoveBuildingResponse)
    - [FetchAllObjectsRequest](#mruv.objects.FetchAllObjectsRequest)
    - [FetchAllObjectsResponse](#mruv.objects.FetchAllObjectsResponse)
    - [FetchAllObjectsResponse.ObjectsEntry](#mruv.objects.FetchAllObjectsResponse.ObjectsEntry)
    - [GetObjectMaterialTextsRequest](#mruv.objects.GetObjectMaterialTextsRequest)
    - [GetObjectMaterialTextsResponse](#mruv.objects.GetObjectMaterialTextsResponse)
    - [GetObjectMaterialTextsResponse.MaterialTextsEntry](#mruv.objects.GetObjectMaterialTextsResponse.MaterialTextsEntry)
    - [GetObjectMaterialsRequest](#mruv.objects.GetObjectMaterialsRequest)
    - [GetObjectMaterialsResponse](#mruv.objects.GetObjectMaterialsResponse)
    - [GetObjectMaterialsResponse.MaterialsEntry](#mruv.objects.GetObjectMaterialsResponse.MaterialsEntry)
    - [GetObjectRequest](#mruv.objects.GetObjectRequest)
    - [GetObjectResponse](#mruv.objects.GetObjectResponse)
    - [GetRemovedBuildingsRequest](#mruv.objects.GetRemovedBuildingsRequest)
    - [GetRemovedBuildingsResponse](#mruv.objects.GetRemovedBuildingsResponse)
    - [Material](#mruv.objects.Material)
    - [MaterialText](#mruv.objects.MaterialText)
    - [Object](#mruv.objects.Object)
    - [Object.MaterialTextsEntry](#mruv.objects.Object.MaterialTextsEntry)
    - [Object.MaterialsEntry](#mruv.objects.Object.MaterialsEntry)
    - [RemovedBuilding](#mruv.objects.RemovedBuilding)
    - [UpdateObjectRequest](#mruv.objects.UpdateObjectRequest)
    - [UpdateObjectResponse](#mruv.objects.UpdateObjectResponse)
  
    - [MaterialSize](#mruv.objects.MaterialSize)
  
  
    - [MruVObjectsService](#mruv.objects.MruVObjectsService)
  

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
  

- [plots/plots.proto](#plots/plots.proto)
    - [CreatePlotRequest](#mruv.plots.CreatePlotRequest)
    - [CreatePlotResponse](#mruv.plots.CreatePlotResponse)
    - [DeletePlotRequest](#mruv.plots.DeletePlotRequest)
    - [DeletePlotResponse](#mruv.plots.DeletePlotResponse)
    - [GetPlotRequest](#mruv.plots.GetPlotRequest)
    - [GetPlotResponse](#mruv.plots.GetPlotResponse)
    - [Plot](#mruv.plots.Plot)
    - [UpdatePlotRequest](#mruv.plots.UpdatePlotRequest)
    - [UpdatePlotResponse](#mruv.plots.UpdatePlotResponse)
  
  
  
    - [MruVPlotsService](#mruv.plots.MruVPlotsService)
  

- [punishments/punishments.proto](#punishments/punishments.proto)
    - [AdminJailMessage](#mruv.punishments.AdminJailMessage)
    - [AdminJailRequest](#mruv.punishments.AdminJailRequest)
    - [AdminJailResponse](#mruv.punishments.AdminJailResponse)
    - [BanMessage](#mruv.punishments.BanMessage)
    - [BanRequest](#mruv.punishments.BanRequest)
    - [BanResponse](#mruv.punishments.BanResponse)
    - [BlockMessage](#mruv.punishments.BlockMessage)
    - [BlockRequest](#mruv.punishments.BlockRequest)
    - [BlockResponse](#mruv.punishments.BlockResponse)
    - [GetBanRequest](#mruv.punishments.GetBanRequest)
    - [GetBlockRequest](#mruv.punishments.GetBlockRequest)
    - [GetPlayerAdminJailRequest](#mruv.punishments.GetPlayerAdminJailRequest)
    - [GetPlayerAdminJailResponse](#mruv.punishments.GetPlayerAdminJailResponse)
    - [GetPlayerBansRequest](#mruv.punishments.GetPlayerBansRequest)
    - [GetPlayerBansResponse](#mruv.punishments.GetPlayerBansResponse)
    - [GetPlayerWarnsRequest](#mruv.punishments.GetPlayerWarnsRequest)
    - [GetPlayerWarnsResponse](#mruv.punishments.GetPlayerWarnsResponse)
    - [GetWarnRequest](#mruv.punishments.GetWarnRequest)
    - [IsCharacterBlockedRequest](#mruv.punishments.IsCharacterBlockedRequest)
    - [IsCharacterBlockedResponse](#mruv.punishments.IsCharacterBlockedResponse)
    - [IsCharacterJailedRequest](#mruv.punishments.IsCharacterJailedRequest)
    - [IsCharacterJailedResponse](#mruv.punishments.IsCharacterJailedResponse)
    - [IsPlayerBannedRequest](#mruv.punishments.IsPlayerBannedRequest)
    - [IsPlayerBannedResponse](#mruv.punishments.IsPlayerBannedResponse)
    - [MuteGlobalChatsRequest](#mruv.punishments.MuteGlobalChatsRequest)
    - [MuteGlobalChatsResponse](#mruv.punishments.MuteGlobalChatsResponse)
    - [UnAdminJailMessage](#mruv.punishments.UnAdminJailMessage)
    - [UnAdminJailRequest](#mruv.punishments.UnAdminJailRequest)
    - [UnAdminJailResponse](#mruv.punishments.UnAdminJailResponse)
    - [UnBanMessage](#mruv.punishments.UnBanMessage)
    - [UnBanRequest](#mruv.punishments.UnBanRequest)
    - [UnBanResponse](#mruv.punishments.UnBanResponse)
    - [UnBlockMessage](#mruv.punishments.UnBlockMessage)
    - [UnBlockRequest](#mruv.punishments.UnBlockRequest)
    - [UnBlockResponse](#mruv.punishments.UnBlockResponse)
    - [UnMuteGlobalChatsRequest](#mruv.punishments.UnMuteGlobalChatsRequest)
    - [UnMuteGlobalChatsResponse](#mruv.punishments.UnMuteGlobalChatsResponse)
    - [UnWarnMessage](#mruv.punishments.UnWarnMessage)
    - [UnWarnRequest](#mruv.punishments.UnWarnRequest)
    - [UnWarnResponse](#mruv.punishments.UnWarnResponse)
    - [WarnMessage](#mruv.punishments.WarnMessage)
    - [WarnRequest](#mruv.punishments.WarnRequest)
    - [WarnResponse](#mruv.punishments.WarnResponse)
    - [WatchAdminJailsRequest](#mruv.punishments.WatchAdminJailsRequest)
    - [WatchBansRequest](#mruv.punishments.WatchBansRequest)
    - [WatchBlocksRequest](#mruv.punishments.WatchBlocksRequest)
    - [WatchPlayerAcquittalsRequest](#mruv.punishments.WatchPlayerAcquittalsRequest)
    - [WatchPlayerAcquittalsResponse](#mruv.punishments.WatchPlayerAcquittalsResponse)
    - [WatchPlayerPunishmentsRequest](#mruv.punishments.WatchPlayerPunishmentsRequest)
    - [WatchPlayerPunishmentsResponse](#mruv.punishments.WatchPlayerPunishmentsResponse)
    - [WatchPunishmentsRequest](#mruv.punishments.WatchPunishmentsRequest)
    - [WatchPunishmentsResponse](#mruv.punishments.WatchPunishmentsResponse)
    - [WatchUnAdminJailsRequest](#mruv.punishments.WatchUnAdminJailsRequest)
    - [WatchUnBansRequest](#mruv.punishments.WatchUnBansRequest)
    - [WatchUnBlocksRequest](#mruv.punishments.WatchUnBlocksRequest)
    - [WatchUnWarnsRequest](#mruv.punishments.WatchUnWarnsRequest)
    - [WatchWarnsRequest](#mruv.punishments.WatchWarnsRequest)
  
    - [AcquittalsType](#mruv.punishments.AcquittalsType)
    - [PunishmentType](#mruv.punishments.PunishmentType)
  
  
    - [MruVPunishmentsService](#mruv.punishments.MruVPunishmentsService)
  

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
  
  
  

- [spots/spots.proto](#spots/spots.proto)
    - [CreateSpotRequest](#mruv.spots.CreateSpotRequest)
    - [CreateSpotResponse](#mruv.spots.CreateSpotResponse)
    - [DeleteSpotRequest](#mruv.spots.DeleteSpotRequest)
    - [DeleteSpotResponse](#mruv.spots.DeleteSpotResponse)
    - [FetchAllSpotsRequest](#mruv.spots.FetchAllSpotsRequest)
    - [FetchAllSpotsResponse](#mruv.spots.FetchAllSpotsResponse)
    - [FetchAllSpotsResponse.SpotsEntry](#mruv.spots.FetchAllSpotsResponse.SpotsEntry)
    - [GetSpotRequest](#mruv.spots.GetSpotRequest)
    - [GetSpotResponse](#mruv.spots.GetSpotResponse)
    - [Spot](#mruv.spots.Spot)
    - [UpdateSpotRequest](#mruv.spots.UpdateSpotRequest)
    - [UpdateSpotResponse](#mruv.spots.UpdateSpotResponse)
  
  
  
    - [MruVSpotsService](#mruv.spots.MruVSpotsService)
  

- [texturestudio/texturestudio_manage.proto](#texturestudio/texturestudio_manage.proto)
    - [CreateServerRequest](#texture_studio.CreateServerRequest)
    - [CreateServerResponse](#texture_studio.CreateServerResponse)
    - [DeleteServerRequest](#texture_studio.DeleteServerRequest)
    - [DeleteServerResponse](#texture_studio.DeleteServerResponse)
    - [GetServersRequest](#texture_studio.GetServersRequest)
    - [GetServersResponse](#texture_studio.GetServersResponse)
    - [MyServerRequest](#texture_studio.MyServerRequest)
    - [MyServerResponse](#texture_studio.MyServerResponse)
    - [TransferOwnershipRequest](#texture_studio.TransferOwnershipRequest)
    - [TransferOwnershipResponse](#texture_studio.TransferOwnershipResponse)
  
  
  
    - [TextureStudioManagerService](#texture_studio.TextureStudioManagerService)
  

- [texturestudio/texturestudio_server.proto](#texturestudio/texturestudio_server.proto)
    - [GetProjectRequest](#texture_studio.GetProjectRequest)
    - [GetProjectResponse](#texture_studio.GetProjectResponse)
    - [GetProjectsRequest](#texture_studio.GetProjectsRequest)
    - [GetProjectsResponse](#texture_studio.GetProjectsResponse)
    - [RestartServerRequest](#texture_studio.RestartServerRequest)
    - [RestartServerResponse](#texture_studio.RestartServerResponse)
    - [ServerStatusRequest](#texture_studio.ServerStatusRequest)
    - [ServerStatusResponse](#texture_studio.ServerStatusResponse)
    - [StartServerRequest](#texture_studio.StartServerRequest)
    - [StartServerResponse](#texture_studio.StartServerResponse)
    - [StopServerRequest](#texture_studio.StopServerRequest)
    - [StopServerResponse](#texture_studio.StopServerResponse)
    - [SubscribeToProjectsChangesRequest](#texture_studio.SubscribeToProjectsChangesRequest)
    - [SubscribeToProjectsChangesResponse](#texture_studio.SubscribeToProjectsChangesResponse)
    - [UploadProjectRequest](#texture_studio.UploadProjectRequest)
    - [UploadProjectResponse](#texture_studio.UploadProjectResponse)
  
    - [ServerStatus](#texture_studio.ServerStatus)
  
  
    - [TextureStudioServerService](#texture_studio.TextureStudioServerService)
  

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



<a name="mruv.accounts.GetAccountCharactersRequest"></a>

### GetAccountCharactersRequest
Request message for rpc `GetAccountCharacters`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| login | [string](#string) |  |  |






<a name="mruv.accounts.GetAccountCharactersResponse"></a>

### GetAccountCharactersResponse
Response message for rpc `GetAccountCharacters`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character_ids | [uint32](#uint32) | repeated |  |






<a name="mruv.accounts.GetAccountRequest"></a>

### GetAccountRequest
Request message for rpc `GetAccount`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| login | [string](#string) |  |  |






<a name="mruv.accounts.GetAccountResponse"></a>

### GetAccountResponse
Response message for rpc `GetAccount`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| login | [string](#string) |  |  |
| email | [string](#string) |  |  |






<a name="mruv.accounts.IsAccountExistRequest"></a>

### IsAccountExistRequest
Request message for rpc `IsAccountExist`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| login | [string](#string) |  |  |






<a name="mruv.accounts.IsAccountExistResponse"></a>

### IsAccountExistResponse
Response message for rpc `IsAccountExist`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| exists | [bool](#bool) |  |  |
| id | [uint32](#uint32) |  |  |






<a name="mruv.accounts.LogInRequest"></a>

### LogInRequest
Request message for rpc `LogIn`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| login | [string](#string) |  |  |
| password | [string](#string) |  |  |






<a name="mruv.accounts.LogInResponse"></a>

### LogInResponse
Response message for rpc `LogIn`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| success | [bool](#bool) |  |  |
| account_id | [uint32](#uint32) |  |  |






<a name="mruv.accounts.RegisterAccountRequest"></a>

### RegisterAccountRequest
Request message for rpc `RegisterAccount`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| login | [string](#string) |  |  |
| password | [string](#string) |  |  |
| email | [string](#string) |  |  |






<a name="mruv.accounts.RegisterAccountResponse"></a>

### RegisterAccountResponse
Response message for rpc `RegisterAccount`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| success | [bool](#bool) |  |  |
| account_id | [uint32](#uint32) |  |  |





 

 

 


<a name="mruv.accounts.MruVAccountsService"></a>

### MruVAccountsService
The MruV accounts service provides procedures for managing players accounts.
This service is an additional/intermediary service between the ORY Kratos &amp; ORY Hydra service.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| RegisterAccount | [RegisterAccountRequest](#mruv.accounts.RegisterAccountRequest) | [RegisterAccountResponse](#mruv.accounts.RegisterAccountResponse) | Register a new account. |
| LogIn | [LogInRequest](#mruv.accounts.LogInRequest) | [LogInResponse](#mruv.accounts.LogInResponse) | Sign into an existing account. |
| IsAccountExist | [IsAccountExistRequest](#mruv.accounts.IsAccountExistRequest) | [IsAccountExistResponse](#mruv.accounts.IsAccountExistResponse) | Check, is account with specified login exist. If yes, it returns account id. |
| GetAccount | [GetAccountRequest](#mruv.accounts.GetAccountRequest) | [GetAccountResponse](#mruv.accounts.GetAccountResponse) | Get an account. |
| GetAccountCharacters | [GetAccountCharactersRequest](#mruv.accounts.GetAccountCharactersRequest) | [GetAccountCharactersResponse](#mruv.accounts.GetAccountCharactersResponse) | Get an account characters. |

 



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



<a name="mruv.characters.ChangeClothesRequest"></a>

### ChangeClothesRequest
Request message for rpc `ChangeClothes`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| clothes_id | [uint32](#uint32) |  |  |






<a name="mruv.characters.ChangeClothesResponse"></a>

### ChangeClothesResponse
Response message for rpc `ChangeClothes`.






<a name="mruv.characters.Character"></a>

### Character



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| owner_id | [uint32](#uint32) |  |  |
| first_name | [string](#string) |  |  |
| second_name | [string](#string) |  |  |
| age | [uint32](#uint32) |  |  |
| sex | [uint32](#uint32) |  |  |
| clothes_id | [uint32](#uint32) |  | TODO: create clothes api |
| x | [float](#float) |  |  |
| y | [float](#float) |  |  |
| z | [float](#float) |  |  |






<a name="mruv.characters.CharacterID"></a>

### CharacterID



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.characters.CreateCharacterRequest"></a>

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






<a name="mruv.characters.CreateCharacterResponse"></a>

### CreateCharacterResponse
Response message for rpc `CreateCharacter`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.characters.DeathStreamRequest"></a>

### DeathStreamRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| death_types | [DeathType](#mruv.characters.DeathType) | repeated |  |






<a name="mruv.characters.DeathStreamResponse"></a>

### DeathStreamResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [Character](#mruv.characters.Character) |  |  |
| death_type | [DeathType](#mruv.characters.DeathType) |  |  |






<a name="mruv.characters.DeleteCharacterRequest"></a>

### DeleteCharacterRequest
Request message for rpc `DeleteCharacter`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.characters.DeleteCharacterResponse"></a>

### DeleteCharacterResponse
Response message for rpc `DeleteCharacter`.






<a name="mruv.characters.GetCharacterRequest"></a>

### GetCharacterRequest
Request message for rpc `GetCharacter`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.characters.GetCharacterResponse"></a>

### GetCharacterResponse
Response message for rpc `GetCharacter`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| owner_id | [uint32](#uint32) |  |  |
| first_name | [string](#string) |  |  |
| second_name | [string](#string) |  |  |
| age | [uint32](#uint32) |  |  |
| sex | [uint32](#uint32) |  |  |
| clothes_id | [uint32](#uint32) |  |  |
| x | [float](#float) |  |  |
| y | [float](#float) |  |  |
| z | [float](#float) |  |  |






<a name="mruv.characters.UpdateCharacterRequest"></a>

### UpdateCharacterRequest
Request message for rpc `UpdateCharacter`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.characters.UpdateCharacterResponse"></a>

### UpdateCharacterResponse
Response message for rpc `UpdateCharacter`.





 


<a name="mruv.characters.DeathType"></a>

### DeathType


| Name | Number | Description |
| ---- | ------ | ----------- |
| DEATH_TYPE_NONE | 0 |  |
| DEATH_TYPE_BW | 1 |  |
| DEATH_TYPE_BW_KILL | 2 |  |
| DEATH_TYPE_CK | 3 |  |


 

 


<a name="mruv.characters.MruVCharactersService"></a>

### MruVCharactersService


| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateCharacter | [CreateCharacterRequest](#mruv.characters.CreateCharacterRequest) | [CreateCharacterResponse](#mruv.characters.CreateCharacterResponse) | Create a character. |
| GetCharacter | [GetCharacterRequest](#mruv.characters.GetCharacterRequest) | [GetCharacterResponse](#mruv.characters.GetCharacterResponse) | Get a character. |
| UpdateCharacter | [UpdateCharacterRequest](#mruv.characters.UpdateCharacterRequest) | [UpdateCharacterResponse](#mruv.characters.UpdateCharacterResponse) | Update a character. |
| DeleteCharacter | [DeleteCharacterRequest](#mruv.characters.DeleteCharacterRequest) | [DeleteCharacterResponse](#mruv.characters.DeleteCharacterResponse) | Delete a character. |
| PermanentCharacterKill | [CharacterID](#mruv.characters.CharacterID) | [CharacterID](#mruv.characters.CharacterID) | Kill a character. A character that is killed cannot be played anymore. |
| ChangeClothes | [ChangeClothesRequest](#mruv.characters.ChangeClothesRequest) | [ChangeClothesResponse](#mruv.characters.ChangeClothesResponse) | Change player clothes. |
| DeathsStream | [DeathStreamRequest](#mruv.characters.DeathStreamRequest) | [DeathStreamResponse](#mruv.characters.DeathStreamResponse) stream | Stream of deaths. |
| GetServiceStatus | [.mruv.common.ServiceStatusRequest](#mruv.common.ServiceStatusRequest) | [.mruv.common.ServiceStatusResponse](#mruv.common.ServiceStatusResponse) | Service status |
| GetServiceVersion | [.mruv.common.VersionRequest](#mruv.common.VersionRequest) | [.mruv.common.VersionResponse](#mruv.common.VersionResponse) |  |

 



<a name="common/health.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## common/health.proto



<a name="mruv.common.ServiceStatusRequest"></a>

### ServiceStatusRequest







<a name="mruv.common.ServiceStatusResponse"></a>

### ServiceStatusResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| status | [string](#string) |  |  |






<a name="mruv.common.VersionRequest"></a>

### VersionRequest







<a name="mruv.common.VersionResponse"></a>

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



<a name="mruv.common.Position"></a>

### Position



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| x | [double](#double) |  |  |
| y | [double](#double) |  |  |
| z | [double](#double) |  |  |






<a name="mruv.common.Rotation"></a>

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
| GetServiceStatus | [.mruv.common.ServiceStatusRequest](#mruv.common.ServiceStatusRequest) | [.mruv.common.ServiceStatusResponse](#mruv.common.ServiceStatusResponse) | Get service status. |
| GetServiceVersion | [.mruv.common.VersionRequest](#mruv.common.VersionRequest) | [.mruv.common.VersionResponse](#mruv.common.VersionResponse) | Get service version. |

 



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

 



<a name="elevators/elevators.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## elevators/elevators.proto



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

 



<a name="entrances/entrances.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## entrances/entrances.proto



<a name="mruv.entrances.CreateEntranceRequest"></a>

### CreateEntranceRequest
Request message for rpc `CreateEntrance`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| out | [mruv.spots.Spot](#mruv.spots.Spot) |  |  |
| in | [mruv.spots.Spot](#mruv.spots.Spot) |  |  |






<a name="mruv.entrances.CreateEntranceResponse"></a>

### CreateEntranceResponse
Response message for rpc `CreateEntrance`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






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
| name | [string](#string) |  |  |
| out | [mruv.spots.Spot](#mruv.spots.Spot) |  |  |
| in | [mruv.spots.Spot](#mruv.spots.Spot) |  |  |






<a name="mruv.entrances.ExitRequest"></a>

### ExitRequest
Request message for rpc `Exit`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.entrances.ExitResponse"></a>

### ExitResponse
Response message for rpc `Exit`.






<a name="mruv.entrances.FetchAllEntrancesRequest"></a>

### FetchAllEntrancesRequest
Request message for rpc `FetchAllEntrances`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| chunk_size | [uint32](#uint32) |  |  |






<a name="mruv.entrances.FetchAllEntrancesResponse"></a>

### FetchAllEntrancesResponse
Response message for rpc `FetchAllEntrances`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| entrances | [FetchAllEntrancesResponse.EntrancesEntry](#mruv.entrances.FetchAllEntrancesResponse.EntrancesEntry) | repeated |  |






<a name="mruv.entrances.FetchAllEntrancesResponse.EntrancesEntry"></a>

### FetchAllEntrancesResponse.EntrancesEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [Entrance](#mruv.entrances.Entrance) |  |  |






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
| inside | [bool](#bool) |  | Is found entrance position is in spot (out spot otherwise) |






<a name="mruv.entrances.GetEntranceRequest"></a>

### GetEntranceRequest
Request message for rpc `GetEntrance`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.entrances.GetEntranceResponse"></a>

### GetEntranceResponse
Response message for rpc `GetEntrance`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| in_spot | [mruv.spots.Spot](#mruv.spots.Spot) |  |  |
| out_spot | [mruv.spots.Spot](#mruv.spots.Spot) |  |  |






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
| in_spot_id | [uint32](#uint32) |  |  |
| out_spot_id | [uint32](#uint32) |  |  |






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
| Enter | [EnterRequest](#mruv.entrances.EnterRequest) | [EnterResponse](#mruv.entrances.EnterResponse) | Enter an entrance (player teleport from in spot position to out spot position). |
| Exit | [ExitRequest](#mruv.entrances.ExitRequest) | [ExitResponse](#mruv.entrances.ExitResponse) | Exit from entrance (player teleport from out spot position to in spot position). |
| FetchAll | [FetchAllEntrancesRequest](#mruv.entrances.FetchAllEntrancesRequest) | [FetchAllEntrancesResponse](#mruv.entrances.FetchAllEntrancesResponse) stream |  |

 



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
| product_id | [uint32](#uint32) |  |  |






<a name="mruv.estates.FetchAllEstatesRequest"></a>

### FetchAllEstatesRequest
Request message for rpc `FetchAll`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| chunk_size | [uint32](#uint32) |  |  |






<a name="mruv.estates.FetchAllEstatesResponse"></a>

### FetchAllEstatesResponse
Response message for rpc `FetchAll`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| estates | [FullEstate](#mruv.estates.FullEstate) | repeated |  |






<a name="mruv.estates.FullEstate"></a>

### FullEstate



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |
| objects | [FullEstate.ObjectsEntry](#mruv.estates.FullEstate.ObjectsEntry) | repeated |  |
| removed_buildings | [FullEstate.RemovedBuildingsEntry](#mruv.estates.FullEstate.RemovedBuildingsEntry) | repeated |  |
| entrances | [FullEstate.EntrancesEntry](#mruv.estates.FullEstate.EntrancesEntry) | repeated |  |
| gates | [FullEstate.GatesEntry](#mruv.estates.FullEstate.GatesEntry) | repeated | TODO: map&lt;uint32, mruv.plots.Plot&gt; rooms = 8; |






<a name="mruv.estates.FullEstate.EntrancesEntry"></a>

### FullEstate.EntrancesEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [mruv.entrances.Entrance](#mruv.entrances.Entrance) |  |  |






<a name="mruv.estates.FullEstate.GatesEntry"></a>

### FullEstate.GatesEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [mruv.gates.Gate](#mruv.gates.Gate) |  |  |






<a name="mruv.estates.FullEstate.ObjectsEntry"></a>

### FullEstate.ObjectsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [mruv.objects.Object](#mruv.objects.Object) |  |  |






<a name="mruv.estates.FullEstate.RemovedBuildingsEntry"></a>

### FullEstate.RemovedBuildingsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [mruv.objects.RemovedBuilding](#mruv.objects.RemovedBuilding) |  |  |






<a name="mruv.estates.GetEstateEntrancesRequest"></a>

### GetEstateEntrancesRequest
Request message for rpc `GetEstateEntrances`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| estate_id | [uint32](#uint32) |  |  |






<a name="mruv.estates.GetEstateEntrancesResponse"></a>

### GetEstateEntrancesResponse
Response message for rpc `GetEstateEntrances`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| entrances | [mruv.entrances.Entrance](#mruv.entrances.Entrance) | repeated |  |






<a name="mruv.estates.GetEstateGatesRequest"></a>

### GetEstateGatesRequest
Request message for rpc `GetEstateGates`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| estate_id | [uint32](#uint32) |  |  |






<a name="mruv.estates.GetEstateGatesResponse"></a>

### GetEstateGatesResponse
Response message for rpc `GetEstateGates`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| gates | [mruv.gates.Gate](#mruv.gates.Gate) | repeated |  |






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
| from | [uint32](#uint32) |  |  |
| limit | [uint32](#uint32) |  |  |






<a name="mruv.estates.GetEstatesResponse"></a>

### GetEstatesResponse
Response message for rpc `GetEstates`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| estates | [Estate](#mruv.estates.Estate) | repeated |  |






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






<a name="mruv.estates.RemoveGateRequest"></a>

### RemoveGateRequest
Request message for rpc `RemoveGate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| estate_id | [uint32](#uint32) |  |  |
| gate_id | [uint32](#uint32) |  |  |






<a name="mruv.estates.RemoveGateResponse"></a>

### RemoveGateResponse
Response message for rpc `RemoveGate`.






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
| RemoveGate | [RemoveGateRequest](#mruv.estates.RemoveGateRequest) | [RemoveGateResponse](#mruv.estates.RemoveGateResponse) | Delete a gate from estate. |
| GetEstateGates | [GetEstateGatesRequest](#mruv.estates.GetEstateGatesRequest) | [GetEstateGatesResponse](#mruv.estates.GetEstateGatesResponse) | Get all estate gates. |
| AddEntrance | [AddEntranceRequest](#mruv.estates.AddEntranceRequest) | [AddEntranceResponse](#mruv.estates.AddEntranceResponse) | Add an entrance to estate. |
| RemoveEntrance | [RemoveEntranceRequest](#mruv.estates.RemoveEntranceRequest) | [RemoveEntranceResponse](#mruv.estates.RemoveEntranceResponse) | Remove an entrance from estate. |
| GetEstateEntrances | [GetEstateEntrancesRequest](#mruv.estates.GetEstateEntrancesRequest) | [GetEstateEntrancesResponse](#mruv.estates.GetEstateEntrancesResponse) | Get all estate entrances. |
| FetchAll | [FetchAllEstatesRequest](#mruv.estates.FetchAllEstatesRequest) | [FetchAllEstatesResponse](#mruv.estates.FetchAllEstatesResponse) stream | Get full estates data |

 



<a name="gates/gates.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## gates/gates.proto



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


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| gate_objects | [mruv.objects.MovableObject](#mruv.objects.MovableObject) | repeated | List of objects to move on gate close/open. Every object should have only 2 states: opened, closed. |
| spot | [mruv.spots.Spot](#mruv.spots.Spot) |  | Gate spot. This spot define gate position. |






<a name="mruv.gates.CreateGateResponse"></a>

### CreateGateResponse
Response message for rpc `CreateGate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.gates.DeleteGateRequest"></a>

### DeleteGateRequest
Request message for rpc `DeleteGate`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.gates.DeleteGateResponse"></a>

### DeleteGateResponse
Response message for rpc `DeleteGate`.






<a name="mruv.gates.FetchAllGatesRequest"></a>

### FetchAllGatesRequest
Request message for rpc `FetchAllGates`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| chunk_size | [uint32](#uint32) |  |  |






<a name="mruv.gates.FetchAllGatesResponse"></a>

### FetchAllGatesResponse
Response message for rpc `FetchAllGates`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| gates | [FetchAllGatesResponse.GatesEntry](#mruv.gates.FetchAllGatesResponse.GatesEntry) | repeated |  |






<a name="mruv.gates.FetchAllGatesResponse.GatesEntry"></a>

### FetchAllGatesResponse.GatesEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [Gate](#mruv.gates.Gate) |  |  |






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
| name | [string](#string) |  |  |
| gate_objects | [mruv.objects.MovableObject](#mruv.objects.MovableObject) | repeated |  |
| spot | [mruv.spots.Spot](#mruv.spots.Spot) |  |  |
| opened | [bool](#bool) |  |  |
| locked | [bool](#bool) |  |  |






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
| name | [string](#string) |  |  |
| movable_objects | [mruv.objects.MovableObject](#mruv.objects.MovableObject) | repeated | List of objects to move on gate close/open. Every object should have only 2 states: opened, closed. |
| spot | [mruv.spots.Spot](#mruv.spots.Spot) |  |  |
| opened | [bool](#bool) |  |  |
| locked | [bool](#bool) |  |  |






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
| name | [string](#string) |  |  |
| spot_id | [uint32](#uint32) |  |  |
| gate_movable_objects | [uint32](#uint32) | repeated |  |






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
| FetchAll | [FetchAllGatesRequest](#mruv.gates.FetchAllGatesRequest) | [FetchAllGatesResponse](#mruv.gates.FetchAllGatesResponse) stream |  |

 



<a name="groups/groups.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## groups/groups.proto



<a name="mruv.groups.AddMemberRequest"></a>

### AddMemberRequest
Request message for rpc `AddMember`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |
| member_id | [uint32](#uint32) |  |  |






<a name="mruv.groups.AddMemberResponse"></a>

### AddMemberResponse
Response message for rpc `AddMember`.






<a name="mruv.groups.AddPermissionRequest"></a>

### AddPermissionRequest
Request message for rpc `AddPermission`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |
| definition | [string](#string) |  |  |






<a name="mruv.groups.AddPermissionResponse"></a>

### AddPermissionResponse
Response message for rpc `AddPermission`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| permission_id | [uint32](#uint32) |  |  |






<a name="mruv.groups.AddSubgroupRequest"></a>

### AddSubgroupRequest
Request message for rpc `AddSubgroup`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |
| subgroup_id | [uint32](#uint32) |  |  |






<a name="mruv.groups.AddSubgroupResponse"></a>

### AddSubgroupResponse
Response message for rpc `AddSubgroup`.






<a name="mruv.groups.AssignOwnerRequest"></a>

### AssignOwnerRequest
Request message for rpc `AssignOwner`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |
| owner_type | [OwnerType](#mruv.groups.OwnerType) |  |  |
| owner_id | [uint32](#uint32) |  |  |






<a name="mruv.groups.AssignOwnerResponse"></a>

### AssignOwnerResponse
Response message for rpc `AssignOwner`.






<a name="mruv.groups.CreateGroupRequest"></a>

### CreateGroupRequest
Request message for rpc `CreateGroup`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |






<a name="mruv.groups.CreateGroupResponse"></a>

### CreateGroupResponse
Response message for rpc `CreateGroup`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |






<a name="mruv.groups.DeleteGroupRequest"></a>

### DeleteGroupRequest
Request message for rpc `DeleteGroup`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |






<a name="mruv.groups.DeleteGroupResponse"></a>

### DeleteGroupResponse
Response message for rpc `DeleteGroup`.






<a name="mruv.groups.GetGroupRequest"></a>

### GetGroupRequest
Request message for rpc `GetGroup`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |






<a name="mruv.groups.GetGroupResponse"></a>

### GetGroupResponse
Response message for rpc `GetGroup`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |






<a name="mruv.groups.GetGroupsRequest"></a>

### GetGroupsRequest
Request message for rpc `GetGroups`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [uint32](#uint32) |  |  |
| begin_from | [uint32](#uint32) |  |  |






<a name="mruv.groups.GetGroupsResponse"></a>

### GetGroupsResponse
Response message for rpc `GetGroups`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| groups | [GetGroupsResponse.Group](#mruv.groups.GetGroupsResponse.Group) | repeated |  |






<a name="mruv.groups.GetGroupsResponse.Group"></a>

### GetGroupsResponse.Group



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |






<a name="mruv.groups.GetMembersRequest"></a>

### GetMembersRequest
Request message for rpc `GetMembers`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |






<a name="mruv.groups.GetMembersResponse"></a>

### GetMembersResponse
Response message for rpc `GetMembers`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| member_type | [MemberType](#mruv.groups.MemberType) |  |  |
| member_ids | [uint32](#uint32) | repeated |  |






<a name="mruv.groups.GetOwnerRequest"></a>

### GetOwnerRequest
Request message for rpc `GetOwner`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |






<a name="mruv.groups.GetOwnerResponse"></a>

### GetOwnerResponse
Response message for rpc `GetOwner`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| owner_id | [uint32](#uint32) |  |  |
| owner_type | [OwnerType](#mruv.groups.OwnerType) |  |  |






<a name="mruv.groups.GetPermissionsRequest"></a>

### GetPermissionsRequest
Request message for rpc `GetPermissions`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |






<a name="mruv.groups.GetPermissionsResponse"></a>

### GetPermissionsResponse
Response message for rpc `GetPermissions`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| permissions | [GetPermissionsResponse.Permission](#mruv.groups.GetPermissionsResponse.Permission) | repeated |  |






<a name="mruv.groups.GetPermissionsResponse.Permission"></a>

### GetPermissionsResponse.Permission



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |
| definition | [string](#string) |  |  |






<a name="mruv.groups.GetSubgroupsRequest"></a>

### GetSubgroupsRequest
Request message for rpc `GetSubgroups`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |






<a name="mruv.groups.GetSubgroupsResponse"></a>

### GetSubgroupsResponse
Response message for rpc `GetSubgroups`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| subgroup_ids | [uint32](#uint32) | repeated |  |






<a name="mruv.groups.IsPermittedRequest"></a>

### IsPermittedRequest
Request message for rpc `IsPermitted`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| member_id | [uint32](#uint32) |  |  |
| member_type | [MemberType](#mruv.groups.MemberType) |  |  |
| action | [string](#string) |  |  |






<a name="mruv.groups.IsPermittedResponse"></a>

### IsPermittedResponse
Response message for rpc `IsPermitted`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| permitted | [bool](#bool) |  |  |






<a name="mruv.groups.RemoveMemberRequest"></a>

### RemoveMemberRequest
Request message for rpc `RemoveMember`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |
| member_id | [uint32](#uint32) |  |  |






<a name="mruv.groups.RemoveMemberResponse"></a>

### RemoveMemberResponse
Response message for rpc `RemoveMember`.






<a name="mruv.groups.RemovePermissionRequest"></a>

### RemovePermissionRequest
Request message for rpc `RemovePermission`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |
| permission_id | [uint32](#uint32) |  |  |






<a name="mruv.groups.RemovePermissionResponse"></a>

### RemovePermissionResponse
Response message for rpc `RemovePermission`.






<a name="mruv.groups.RemoveSubgroupRequest"></a>

### RemoveSubgroupRequest
Request message for rpc `RemoveSubgroup`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |
| subgroup_id | [uint32](#uint32) |  |  |






<a name="mruv.groups.RemoveSubgroupResponse"></a>

### RemoveSubgroupResponse
Response message for rpc `RemoveSubgroup`.






<a name="mruv.groups.UpdateGroupRequest"></a>

### UpdateGroupRequest
Request message for rpc `UpdateGroup`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| group_id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |






<a name="mruv.groups.UpdateGroupResponse"></a>

### UpdateGroupResponse
Response message for rpc `UpdateGroup`.





 


<a name="mruv.groups.MemberType"></a>

### MemberType
Member type.

| Name | Number | Description |
| ---- | ------ | ----------- |
| MEMBER_TYPE_UNKNOWN | 0 |  |
| MEMBER_TYPE_ACCOUNT | 1 |  |
| MEMBER_TYPE_CHARACTER | 2 |  |



<a name="mruv.groups.OwnerType"></a>

### OwnerType
Owner types.

| Name | Number | Description |
| ---- | ------ | ----------- |
| OWNER_TYPE_UNKNOWN | 0 |  |
| OWNER_TYPE_ACCOUNT | 1 |  |
| OWNER_TYPE_CHARACTER | 2 |  |
| OWNER_TYPE_GROUP | 3 |  |


 

 


<a name="mruv.groups.MruVGroupsService"></a>

### MruVGroupsService
The MruV groups service provides procedures for managing groups.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateGroup | [CreateGroupRequest](#mruv.groups.CreateGroupRequest) | [CreateGroupResponse](#mruv.groups.CreateGroupResponse) | Create a group. |
| GetGroup | [GetGroupRequest](#mruv.groups.GetGroupRequest) | [GetGroupResponse](#mruv.groups.GetGroupResponse) | Get a group. |
| UpdateGroup | [UpdateGroupRequest](#mruv.groups.UpdateGroupRequest) | [UpdateGroupResponse](#mruv.groups.UpdateGroupResponse) | Update a group. |
| DeleteGroup | [DeleteGroupRequest](#mruv.groups.DeleteGroupRequest) | [DeleteGroupResponse](#mruv.groups.DeleteGroupResponse) | Delete a group. |
| GetGroups | [GetGroupsRequest](#mruv.groups.GetGroupsRequest) | [GetGroupsResponse](#mruv.groups.GetGroupsResponse) | Get all groups. |
| AssignOwner | [AssignOwnerRequest](#mruv.groups.AssignOwnerRequest) | [AssignOwnerResponse](#mruv.groups.AssignOwnerResponse) | Assign an owner. Group can have only one owner. Owner can be a player, a group or an account. |
| GetOwner | [GetOwnerRequest](#mruv.groups.GetOwnerRequest) | [GetOwnerResponse](#mruv.groups.GetOwnerResponse) | Get group owner. |
| AddMember | [AddMemberRequest](#mruv.groups.AddMemberRequest) | [AddMemberResponse](#mruv.groups.AddMemberResponse) | Add a group member. |
| GetMembers | [GetMembersRequest](#mruv.groups.GetMembersRequest) | [GetMembersResponse](#mruv.groups.GetMembersResponse) | Get a group member. |
| RemoveMember | [RemoveMemberRequest](#mruv.groups.RemoveMemberRequest) | [RemoveMemberResponse](#mruv.groups.RemoveMemberResponse) | Remove a group member. |
| AddPermission | [AddPermissionRequest](#mruv.groups.AddPermissionRequest) | [AddPermissionResponse](#mruv.groups.AddPermissionResponse) | Add a permission to a group. |
| GetPermissions | [GetPermissionsRequest](#mruv.groups.GetPermissionsRequest) | [GetPermissionsResponse](#mruv.groups.GetPermissionsResponse) | Get all group permissions. |
| RemovePermission | [RemovePermissionRequest](#mruv.groups.RemovePermissionRequest) | [RemovePermissionResponse](#mruv.groups.RemovePermissionResponse) | Remove group permission. |
| AddSubgroup | [AddSubgroupRequest](#mruv.groups.AddSubgroupRequest) | [AddSubgroupResponse](#mruv.groups.AddSubgroupResponse) | Add a subgroup to a group. |
| GetSubgroups | [GetSubgroupsRequest](#mruv.groups.GetSubgroupsRequest) | [GetSubgroupsResponse](#mruv.groups.GetSubgroupsResponse) | Get all subgroups. |
| RemoveSubgroup | [RemoveSubgroupRequest](#mruv.groups.RemoveSubgroupRequest) | [RemoveSubgroupResponse](#mruv.groups.RemoveSubgroupResponse) | Remove a subgroup from group. |
| IsPermitted | [IsPermittedRequest](#mruv.groups.IsPermittedRequest) | [IsPermittedResponse](#mruv.groups.IsPermittedResponse) | Check is member of a group is permitted to do specific action. |
| GetServiceStatus | [.mruv.common.ServiceStatusRequest](#mruv.common.ServiceStatusRequest) | [.mruv.common.ServiceStatusResponse](#mruv.common.ServiceStatusResponse) | Service status |
| GetServiceVersion | [.mruv.common.VersionRequest](#mruv.common.VersionRequest) | [.mruv.common.VersionResponse](#mruv.common.VersionResponse) |  |

 



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



<a name="mruv.items.GetContainerItemsRequest"></a>

### GetContainerItemsRequest
Request message for `MruVItemsService.GetContainerItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [uint32](#uint32) |  | ID of container with items. |
| limit | [uint32](#uint32) |  | Limit of the returned items. |






<a name="mruv.items.GetContainerItemsResponse"></a>

### GetContainerItemsResponse
Request message for `MruVItemsService.GetContainerItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| items | [InsideItem](#mruv.items.InsideItem) | repeated | List of items inside containers. |






<a name="mruv.items.GetContainerTypesRequest"></a>

### GetContainerTypesRequest
Request message for `MruVItemsService.GetContainerTypes`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [uint32](#uint32) |  | Limit of the returned container types. |






<a name="mruv.items.GetContainerTypesResponse"></a>

### GetContainerTypesResponse
Response message for `MruVItemsService.GetContainers`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_types | [ContainerType](#mruv.items.ContainerType) | repeated | List of container types. |






<a name="mruv.items.GetContainersRequest"></a>

### GetContainersRequest
Request message for `MruVItemsService.GetContainers`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [uint32](#uint32) |  | Limit of the returned containers. |






<a name="mruv.items.GetContainersResponse"></a>

### GetContainersResponse
Response message for `MruVItemsService.GetContainers`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| containers | [Container](#mruv.items.Container) | repeated | List of containers. |






<a name="mruv.items.GetItemTypesRequest"></a>

### GetItemTypesRequest
Request message for `MruVItemsService.GetItemTypes`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [uint32](#uint32) |  | Limit of the returned item types. |






<a name="mruv.items.GetItemTypesResponse"></a>

### GetItemTypesResponse
Response message for `MruVItemsService.GetItemTypes`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| item_types | [ItemType](#mruv.items.ItemType) | repeated | List of item types. |






<a name="mruv.items.GetItemsRequest"></a>

### GetItemsRequest
Request message for `MruVItemsService.GetItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| limit | [uint32](#uint32) |  | Limit of the returned items. |






<a name="mruv.items.GetItemsResponse"></a>

### GetItemsResponse
Response message for `MruVItemsService.GetItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| items | [Item](#mruv.items.Item) | repeated | List of items. |






<a name="mruv.items.GetNearestItemsRequest"></a>

### GetNearestItemsRequest
Request message for `MruVItemsService.GetNearestItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| position | [mruv.common.Position](#mruv.common.Position) |  | Position from which to calculate the distance |
| container_id | [uint32](#uint32) |  | ID of container that contains items. |
| distance_limit | [double](#double) |  | The distance over which the items are ignored. |






<a name="mruv.items.GetNearestItemsResponse"></a>

### GetNearestItemsResponse
Response message for `MruVItemsService.GetNearestItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| item | [InsideItem](#mruv.items.InsideItem) | repeated | List of items sorted from nearest to farthest. |






<a name="mruv.items.PullItemRequest"></a>

### PullItemRequest
Request message for `MruVItemsService.PullItem`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [uint32](#uint32) |  | ID of the container from which we pull out a item. |
| item_id | [uint32](#uint32) |  | ID of the item we want to pull out. That item must be inside the container. |






<a name="mruv.items.PutItemRequest"></a>

### PutItemRequest
Request message for `MruVItemsService.PutItem`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [uint32](#uint32) |  | ID of container where to put item. |
| item_id | [uint32](#uint32) |  | ID of item we wan to put in. |
| slot | [int32](#int32) |  | Position used for sorting items |






<a name="mruv.items.PutItemResponse"></a>

### PutItemResponse
Response message for `MruVItemsService.PutItem`


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| inside_item | [InsideItem](#mruv.items.InsideItem) |  | Container with items inside. |






<a name="mruv.items.SortItemsRequest"></a>

### SortItemsRequest
Request message for `MruVItemsService.SortItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [uint32](#uint32) |  | ID of the container which contain items. |
| sort_by | [SortingMode](#mruv.items.SortingMode) |  | Sorting mode. |






<a name="mruv.items.SortItemsResponse"></a>

### SortItemsResponse
Response message for `MruVItemsService.SortItems`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container | [Container](#mruv.items.Container) |  | Container with sorted items inside. |






<a name="mruv.items.UseItemRequest"></a>

### UseItemRequest
Request message for `MruVItemsService.UseItem`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| item_id | [uint32](#uint32) |  |  |






<a name="mruv.items.UseItemResponse"></a>

### UseItemResponse
Response message for `MruVItemsService.UseItem`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| success | [bool](#bool) |  | Is item usage was successful. |





 

 

 


<a name="mruv.items.MruVItemService"></a>

### MruVItemService
The MruV items service provides procedures for managing items and containers

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateItem | [Item](#mruv.items.Item) | [ItemID](#mruv.items.ItemID) | Create new item. |
| GetItem | [ItemID](#mruv.items.ItemID) | [Item](#mruv.items.Item) | Get item by id. |
| DeleteItem | [ItemID](#mruv.items.ItemID) | [ItemID](#mruv.items.ItemID) | Delete item by id. |
| GetItems | [GetItemsRequest](#mruv.items.GetItemsRequest) | [GetItemsResponse](#mruv.items.GetItemsResponse) | Gets all items. |
| CreateItemType | [ItemType](#mruv.items.ItemType) | [ItemTypeID](#mruv.items.ItemTypeID) | Create item type. |
| GetItemType | [ItemTypeID](#mruv.items.ItemTypeID) | [ItemType](#mruv.items.ItemType) | Get item type by id. |
| DeleteItemType | [ItemTypeID](#mruv.items.ItemTypeID) | [ItemTypeID](#mruv.items.ItemTypeID) | Delete item type by id. |
| GetItemTypes | [GetItemTypesRequest](#mruv.items.GetItemTypesRequest) | [GetItemTypesResponse](#mruv.items.GetItemTypesResponse) | Gets all item types. |
| CreateContainer | [Container](#mruv.items.Container) | [ContainerID](#mruv.items.ContainerID) | Create container. |
| GetContainer | [ContainerID](#mruv.items.ContainerID) | [Container](#mruv.items.Container) | Get container by id. |
| DeleteContainer | [ContainerID](#mruv.items.ContainerID) | [ContainerID](#mruv.items.ContainerID) | Delete container by id. |
| GetContainers | [GetContainersRequest](#mruv.items.GetContainersRequest) | [GetContainersResponse](#mruv.items.GetContainersResponse) | Get all containers. |
| CreateContainerType | [ContainerType](#mruv.items.ContainerType) | [ContainerTypeID](#mruv.items.ContainerTypeID) | Create a container type. |
| GetContainerType | [ContainerTypeID](#mruv.items.ContainerTypeID) | [ContainerType](#mruv.items.ContainerType) | Get a container type by id. |
| DeleteContainerType | [ContainerTypeID](#mruv.items.ContainerTypeID) | [ContainerTypeID](#mruv.items.ContainerTypeID) | Delete a container type by id. |
| GetContainerTypes | [GetContainerTypesRequest](#mruv.items.GetContainerTypesRequest) | [GetContainerTypesResponse](#mruv.items.GetContainerTypesResponse) | Get all container types. |
| GetContainerItems | [GetContainerItemsRequest](#mruv.items.GetContainerItemsRequest) | [GetContainerItemsResponse](#mruv.items.GetContainerItemsResponse) | Get items inside a container. |
| PullItem | [PullItemRequest](#mruv.items.PullItemRequest) | [Item](#mruv.items.Item) | Pull an item from container. |
| PutItem | [PutItemRequest](#mruv.items.PutItemRequest) | [PutItemResponse](#mruv.items.PutItemResponse) | Put an item into container. |
| SortItems | [SortItemsRequest](#mruv.items.SortItemsRequest) | [SortItemsResponse](#mruv.items.SortItemsResponse) | Sort items inside container. This procedure change order of items inside container. |
| GetNearestItems | [GetNearestItemsRequest](#mruv.items.GetNearestItemsRequest) | [GetNearestItemsResponse](#mruv.items.GetNearestItemsResponse) | Retrieves from the container the list of items nearest to the given position. |
| UseItem | [UseItemRequest](#mruv.items.UseItemRequest) | [UseItemResponse](#mruv.items.UseItemResponse) | Trigger action associated with the item usage. |
| GetServiceStatus | [.mruv.common.ServiceStatusRequest](#mruv.common.ServiceStatusRequest) | [.mruv.common.ServiceStatusResponse](#mruv.common.ServiceStatusResponse) | Get service health status. |
| GetServiceVersion | [.mruv.common.VersionRequest](#mruv.common.VersionRequest) | [.mruv.common.VersionResponse](#mruv.common.VersionResponse) | Get service current version. |

 



<a name="items/items_model.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## items/items_model.proto



<a name="mruv.items.Container"></a>

### Container
Container data structure.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| type_id | [uint32](#uint32) |  | ID of an container type. |
| item_id | [uint32](#uint32) |  | ID of container item representing container. |
| items_inside | [uint32](#uint32) |  | Number of items inside container. |
| items | [InsideItem](#mruv.items.InsideItem) | repeated | List of items inside container. |






<a name="mruv.items.ContainerID"></a>

### ContainerID
Container ID.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.items.ContainerType"></a>

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






<a name="mruv.items.ContainerTypeID"></a>

### ContainerTypeID
Container type ID.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.items.InsideItem"></a>

### InsideItem
Item inside container data structure.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| container_id | [uint32](#uint32) |  | ID of container containing the item. |
| item_id | [uint32](#uint32) |  |  |
| item | [Item](#mruv.items.Item) |  |  |
| position | [int32](#int32) |  | Position representing order in container. In ascending manner. |






<a name="mruv.items.Item"></a>

### Item
Item data structure.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| item_type_id | [uint32](#uint32) |  | ID of an item type. |
| weight | [float](#float) |  | Current weight of the item. |
| volume | [float](#float) |  | Current volume of the item. |






<a name="mruv.items.ItemID"></a>

### ItemID
Item ID.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.items.ItemType"></a>

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






<a name="mruv.items.ItemTypeID"></a>

### ItemTypeID
Item type ID.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |





 


<a name="mruv.items.SortingMode"></a>

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

 



<a name="objects/models.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## objects/models.proto



<a name="mruv.objects.CreateObjectModelRequest"></a>

### CreateObjectModelRequest
Request message for rpc `CreateObjectModel`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| object_type | [ObjectModel](#mruv.objects.ObjectModel) |  |  |






<a name="mruv.objects.CreateObjectModelResponse"></a>

### CreateObjectModelResponse
Response message for rpc `CreateObjectModel`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.objects.DeleteObjectModelRequest"></a>

### DeleteObjectModelRequest
Request message for rpc `DeleteObjectModel`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| model | [int32](#int32) |  |  |






<a name="mruv.objects.DeleteObjectModelResponse"></a>

### DeleteObjectModelResponse
Response message for rpc `DeleteObjectModel`.






<a name="mruv.objects.FetchAllModelsRequest"></a>

### FetchAllModelsRequest
Request message for rpc `FetchAll`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| chunk_size | [uint32](#uint32) |  |  |






<a name="mruv.objects.FetchAllModelsResponse"></a>

### FetchAllModelsResponse
Response message for rpc `FetchAll`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| models | [FetchAllModelsResponse.ModelsEntry](#mruv.objects.FetchAllModelsResponse.ModelsEntry) | repeated |  |






<a name="mruv.objects.FetchAllModelsResponse.ModelsEntry"></a>

### FetchAllModelsResponse.ModelsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [ObjectModel](#mruv.objects.ObjectModel) |  |  |






<a name="mruv.objects.GetObjectModelRequest"></a>

### GetObjectModelRequest
Request message for rpc `GetObjectModel`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| model | [int32](#int32) |  |  |






<a name="mruv.objects.GetObjectModelResponse"></a>

### GetObjectModelResponse
Response message for rpc `GetObjectModel`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| object_type | [ObjectModel](#mruv.objects.ObjectModel) |  |  |






<a name="mruv.objects.ObjectModel"></a>

### ObjectModel
SA-MP Object type data structure.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| model | [int32](#int32) |  |  |
| model_name | [string](#string) |  |  |
| name | [string](#string) |  |  |
| category | [string](#string) |  |  |
| length | [double](#double) |  |  |
| width | [double](#double) |  |  |
| height | [double](#double) |  |  |
| size | [double](#double) |  | if no size specified, it will be calculated based on length, width and height |
| tags | [string](#string) | repeated |  |
| has_collision | [bool](#bool) |  |  |
| breaks_on_hit | [bool](#bool) |  |  |
| has_animation | [bool](#bool) |  |  |
| visible_by_time | [bool](#bool) |  |  |
| visible_from | [uint32](#uint32) |  |  |
| visible_to | [uint32](#uint32) |  |  |






<a name="mruv.objects.UpdateObjectModelRequest"></a>

### UpdateObjectModelRequest
Request message for rpc `UpdateObjectModel`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| object_type | [ObjectModel](#mruv.objects.ObjectModel) |  |  |






<a name="mruv.objects.UpdateObjectModelResponse"></a>

### UpdateObjectModelResponse
Response message for rpc `UpdateObjectModel`.





 

 

 


<a name="mruv.objects.MruVObjectModelsService"></a>

### MruVObjectModelsService
The MruV objects service provides procedures for game object models.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateObjectModel | [CreateObjectModelRequest](#mruv.objects.CreateObjectModelRequest) | [CreateObjectModelResponse](#mruv.objects.CreateObjectModelResponse) | Create an object model. |
| GetObjectModel | [GetObjectModelRequest](#mruv.objects.GetObjectModelRequest) | [GetObjectModelResponse](#mruv.objects.GetObjectModelResponse) | Get an object model. |
| UpdateObjectModel | [UpdateObjectModelRequest](#mruv.objects.UpdateObjectModelRequest) | [UpdateObjectModelResponse](#mruv.objects.UpdateObjectModelResponse) | Update an object model. |
| DeleteObjectModel | [DeleteObjectModelRequest](#mruv.objects.DeleteObjectModelRequest) | [DeleteObjectModelResponse](#mruv.objects.DeleteObjectModelResponse) | Delete an object model. |
| FetchAllModels | [FetchAllModelsRequest](#mruv.objects.FetchAllModelsRequest) | [FetchAllModelsResponse](#mruv.objects.FetchAllModelsResponse) stream | Get all models. |

 



<a name="objects/movable.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## objects/movable.proto



<a name="mruv.objects.CreateMovableObjectRequest"></a>

### CreateMovableObjectRequest
Request message for rpc `CreateMovableObject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| object | [Object](#mruv.objects.Object) |  |  |
| states | [State](#mruv.objects.State) | repeated | List of states that an object can take. |






<a name="mruv.objects.CreateMovableObjectResponse"></a>

### CreateMovableObjectResponse
Response message for rpc `CreateMovableObject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.objects.DeleteMovableObjectRequest"></a>

### DeleteMovableObjectRequest
Request message for rpc `DeleteMovableObject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.objects.DeleteMovableObjectResponse"></a>

### DeleteMovableObjectResponse
Response message for rpc `DeleteMovableObject`.






<a name="mruv.objects.FetchAllMovableObjectsRequest"></a>

### FetchAllMovableObjectsRequest
Request message for rpc `FetchAllMovableObjects`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| chunk_size | [uint32](#uint32) |  |  |






<a name="mruv.objects.FetchAllMovableObjectsResponse"></a>

### FetchAllMovableObjectsResponse
Response message for rpc `FetchAllMovableObjects`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| movable_objects | [FetchAllMovableObjectsResponse.MovableObjectsEntry](#mruv.objects.FetchAllMovableObjectsResponse.MovableObjectsEntry) | repeated |  |






<a name="mruv.objects.FetchAllMovableObjectsResponse.MovableObjectsEntry"></a>

### FetchAllMovableObjectsResponse.MovableObjectsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [MovableObject](#mruv.objects.MovableObject) |  |  |






<a name="mruv.objects.GetMovableObjectRequest"></a>

### GetMovableObjectRequest
Request message for rpc `GetMovableObject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.objects.GetMovableObjectResponse"></a>

### GetMovableObjectResponse
Response message for rpc `GetMovableObject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| object | [Object](#mruv.objects.Object) |  |  |
| states | [State](#mruv.objects.State) | repeated |  |
| current_state_id | [uint32](#uint32) |  |  |
| current_state_name | [string](#string) |  |  |






<a name="mruv.objects.MovableObject"></a>

### MovableObject
A movable object.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| object | [Object](#mruv.objects.Object) |  |  |
| states | [State](#mruv.objects.State) | repeated | List of states that an object can take. |






<a name="mruv.objects.MoveObjectNextRequest"></a>

### MoveObjectNextRequest
Request message for rpc `MoveObjectNext`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.objects.MoveObjectNextResponse"></a>

### MoveObjectNextResponse
Response message for rpc `MoveObjectNext`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| state_id | [uint32](#uint32) |  |  |
| state_name | [string](#string) |  |  |






<a name="mruv.objects.MoveObjectPreviousRequest"></a>

### MoveObjectPreviousRequest
Request message for rpc `MoveObjectPrevious`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.objects.MoveObjectPreviousResponse"></a>

### MoveObjectPreviousResponse
Response message for rpc `MoveObjectPrevious`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| state_id | [uint32](#uint32) |  |  |
| state_name | [string](#string) |  |  |






<a name="mruv.objects.MoveObjectRequest"></a>

### MoveObjectRequest
Request message for rpc `MoveObject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| state | [uint32](#uint32) |  |  |






<a name="mruv.objects.MoveObjectResponse"></a>

### MoveObjectResponse
Response message for rpc `MoveObject`.






<a name="mruv.objects.State"></a>

### State
Position and rotation state of moving object.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| x | [float](#float) |  |  |
| y | [float](#float) |  |  |
| z | [float](#float) |  |  |
| rx | [float](#float) |  |  |
| ry | [float](#float) |  |  |
| rz | [float](#float) |  |  |
| transition_speed | [float](#float) |  |  |






<a name="mruv.objects.UpdateMovableObjectRequest"></a>

### UpdateMovableObjectRequest
Request message for rpc `UpdateMovableObject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| object_id | [uint32](#uint32) |  | 0 for no changes. |
| states | [State](#mruv.objects.State) | repeated |  |






<a name="mruv.objects.UpdateMovableObjectResponse"></a>

### UpdateMovableObjectResponse
Response message for rpc `UpdateMovableObject`.





 

 

 


<a name="mruv.objects.MruVMovableObjectsService"></a>

### MruVMovableObjectsService
The MruV objects service provides procedures for movable game objects.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateMovableObject | [CreateMovableObjectRequest](#mruv.objects.CreateMovableObjectRequest) | [CreateMovableObjectResponse](#mruv.objects.CreateMovableObjectResponse) | Create a movable object. |
| GetMovableObject | [GetMovableObjectRequest](#mruv.objects.GetMovableObjectRequest) | [GetMovableObjectResponse](#mruv.objects.GetMovableObjectResponse) | Get a movable object. |
| UpdateMovableObject | [UpdateMovableObjectRequest](#mruv.objects.UpdateMovableObjectRequest) | [UpdateMovableObjectResponse](#mruv.objects.UpdateMovableObjectResponse) | Update a movable object. |
| DeleteMovableObject | [DeleteMovableObjectRequest](#mruv.objects.DeleteMovableObjectRequest) | [DeleteMovableObjectResponse](#mruv.objects.DeleteMovableObjectResponse) | Delete a movable object. |
| MoveObject | [MoveObjectRequest](#mruv.objects.MoveObjectRequest) | [MoveObjectResponse](#mruv.objects.MoveObjectResponse) | Move an object to other state. |
| MoveObjectNext | [MoveObjectNextRequest](#mruv.objects.MoveObjectNextRequest) | [MoveObjectNextResponse](#mruv.objects.MoveObjectNextResponse) | Move an object to next state. |
| MoveObjectPrevious | [MoveObjectPreviousRequest](#mruv.objects.MoveObjectPreviousRequest) | [MoveObjectPreviousResponse](#mruv.objects.MoveObjectPreviousResponse) | Move an object to previous state. |
| FetchAllMovableObjects | [FetchAllMovableObjectsRequest](#mruv.objects.FetchAllMovableObjectsRequest) | [FetchAllMovableObjectsResponse](#mruv.objects.FetchAllMovableObjectsResponse) stream |  |

 



<a name="objects/objects.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## objects/objects.proto



<a name="mruv.objects.AddObjectMaterialRequest"></a>

### AddObjectMaterialRequest
Request message for rpc `AddObjectMaterial`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| object_id | [uint32](#uint32) |  |  |
| index | [uint32](#uint32) |  | The material index on the object to change (0 to 15) |
| material | [Material](#mruv.objects.Material) |  |  |






<a name="mruv.objects.AddObjectMaterialResponse"></a>

### AddObjectMaterialResponse
Response message for rpc `AddObjectMaterial`.






<a name="mruv.objects.AddObjectMaterialTextRequest"></a>

### AddObjectMaterialTextRequest
Request message for rpc `AddObjectMaterialText`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| object_id | [uint32](#uint32) |  |  |
| index | [uint32](#uint32) |  | The object&#39;s material index to replace with text (0 to 15). |
| material_text | [MaterialText](#mruv.objects.MaterialText) |  |  |






<a name="mruv.objects.AddObjectMaterialTextResponse"></a>

### AddObjectMaterialTextResponse
Response message for rpc `AddObjectMaterialText`.






<a name="mruv.objects.AddRemoveBuildingRequest"></a>

### AddRemoveBuildingRequest
Request message for rpc `AddRemoveBuilding`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| removed_building | [RemovedBuilding](#mruv.objects.RemovedBuilding) |  |  |






<a name="mruv.objects.AddRemoveBuildingResponse"></a>

### AddRemoveBuildingResponse
Response message for rpc `AddRemoveBuilding`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.objects.CreateObjectRequest"></a>

### CreateObjectRequest
Request message for rpc `CreateObject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| object | [Object](#mruv.objects.Object) |  |  |






<a name="mruv.objects.CreateObjectResponse"></a>

### CreateObjectResponse
Response message for rpc `CreateObject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.objects.DeleteObjectMaterialRequest"></a>

### DeleteObjectMaterialRequest
Request message for rpc `DeleteObjectMaterial`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| object_id | [uint32](#uint32) |  |  |
| index | [uint32](#uint32) |  | The material index on the object to delete (0 to 15). |






<a name="mruv.objects.DeleteObjectMaterialResponse"></a>

### DeleteObjectMaterialResponse
Response message for rpc `DeleteObjectMaterial`.






<a name="mruv.objects.DeleteObjectMaterialTextRequest"></a>

### DeleteObjectMaterialTextRequest
Request message for rpc `DeleteObjectMaterialText`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| object_id | [uint32](#uint32) |  |  |
| index | [uint32](#uint32) |  | The object&#39;s material index to delete (0 to 15). |






<a name="mruv.objects.DeleteObjectMaterialTextResponse"></a>

### DeleteObjectMaterialTextResponse
Response message for rpc `DeleteObjectMaterialText`.






<a name="mruv.objects.DeleteObjectRequest"></a>

### DeleteObjectRequest
Request message for rpc `DeleteObject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.objects.DeleteObjectResponse"></a>

### DeleteObjectResponse
Response message for rpc `DeleteObject`.






<a name="mruv.objects.DeleteRemoveBuildingRequest"></a>

### DeleteRemoveBuildingRequest
Request message for rpc `DeleteRemoveBuilding`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.objects.DeleteRemoveBuildingResponse"></a>

### DeleteRemoveBuildingResponse
Response message for rpc `DeleteRemoveBuilding`.






<a name="mruv.objects.FetchAllObjectsRequest"></a>

### FetchAllObjectsRequest
Request message for rpc `FetchAll`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| chunk_size | [uint32](#uint32) |  |  |
| estate_id | [uint32](#uint32) |  | optional filter for estate id |






<a name="mruv.objects.FetchAllObjectsResponse"></a>

### FetchAllObjectsResponse
Response message for rpc `FetchAll`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| objects | [FetchAllObjectsResponse.ObjectsEntry](#mruv.objects.FetchAllObjectsResponse.ObjectsEntry) | repeated |  |






<a name="mruv.objects.FetchAllObjectsResponse.ObjectsEntry"></a>

### FetchAllObjectsResponse.ObjectsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [int32](#int32) |  |  |
| value | [Object](#mruv.objects.Object) |  |  |






<a name="mruv.objects.GetObjectMaterialTextsRequest"></a>

### GetObjectMaterialTextsRequest
Request message for rpc `GetObjectMaterialTexts`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| object_id | [uint32](#uint32) |  |  |






<a name="mruv.objects.GetObjectMaterialTextsResponse"></a>

### GetObjectMaterialTextsResponse
Response message for rpc `GetObjectMaterialTexts`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| material_texts | [GetObjectMaterialTextsResponse.MaterialTextsEntry](#mruv.objects.GetObjectMaterialTextsResponse.MaterialTextsEntry) | repeated | Map of material texts, key - material index (0-15). |






<a name="mruv.objects.GetObjectMaterialTextsResponse.MaterialTextsEntry"></a>

### GetObjectMaterialTextsResponse.MaterialTextsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [MaterialText](#mruv.objects.MaterialText) |  |  |






<a name="mruv.objects.GetObjectMaterialsRequest"></a>

### GetObjectMaterialsRequest
Request message for rpc `GetObjectMaterials`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| object_id | [uint32](#uint32) |  |  |






<a name="mruv.objects.GetObjectMaterialsResponse"></a>

### GetObjectMaterialsResponse
Response message for rpc `GetObjectMaterials`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| materials | [GetObjectMaterialsResponse.MaterialsEntry](#mruv.objects.GetObjectMaterialsResponse.MaterialsEntry) | repeated | Map of materials, key - material index (0-15) |






<a name="mruv.objects.GetObjectMaterialsResponse.MaterialsEntry"></a>

### GetObjectMaterialsResponse.MaterialsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [Material](#mruv.objects.Material) |  |  |






<a name="mruv.objects.GetObjectRequest"></a>

### GetObjectRequest
Request message for rpc `GetObject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.objects.GetObjectResponse"></a>

### GetObjectResponse
Response message for rpc `GetObject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| object | [Object](#mruv.objects.Object) |  |  |






<a name="mruv.objects.GetRemovedBuildingsRequest"></a>

### GetRemovedBuildingsRequest
Request message for rpc `GetRemovedBuildings`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| estate_id | [uint32](#uint32) |  | optional filter for estate id |






<a name="mruv.objects.GetRemovedBuildingsResponse"></a>

### GetRemovedBuildingsResponse
Response message for rpc `GetRemovedBuildings`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| removed_buildings | [RemovedBuilding](#mruv.objects.RemovedBuilding) | repeated |  |






<a name="mruv.objects.Material"></a>

### Material
Replace the texture of an object with the texture from another model in the game.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| model_id | [int32](#int32) |  | The modelid on which the replacement texture is located. Use 0 for alpha. Use -1 to change the material color without altering the texture. |
| txd_name | [string](#string) |  | The name of the txd file which contains the replacement texture (use &#34;none&#34; if not required) |
| texture_name | [string](#string) |  | The name of the texture to use as the replacement (use &#34;none&#34; if not required) |
| material_color | [int32](#int32) |  | The object color to set, as an integer or hex in ARGB color format. Using 0 keeps the existing material color. |






<a name="mruv.objects.MaterialText"></a>

### MaterialText
Replace the texture of an object with text.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| text | [string](#string) |  | The text to show on the object (MAX 2048 characters). |
| material_size | [MaterialSize](#mruv.objects.MaterialSize) |  | The size of the material (default: 256x128). |
| font_face | [string](#string) |  | The font to use (default: Arial). |
| font_size | [uint32](#uint32) |  | The size of the text (default: 24) (MAX 255). |
| bold | [bool](#bool) |  | Bold text. Set to 1 for bold, 0 for not (default: 1). |
| font_color | [int32](#int32) |  | The color of the text, in ARGB format (default: White). |
| back_color | [int32](#int32) |  | The background color, in ARGB format (default: None (transparent)). |
| text_alignment | [int32](#int32) |  | The alignment of the text (default: left). |






<a name="mruv.objects.Object"></a>

### Object
SA-MP Dynamic object data structure.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| model | [int32](#int32) |  |  |
| x | [float](#float) |  |  |
| y | [float](#float) |  |  |
| z | [float](#float) |  |  |
| rx | [float](#float) |  |  |
| ry | [float](#float) |  |  |
| rz | [float](#float) |  |  |
| world_id | [int32](#int32) |  | Virtual world id for which object will be visible. Set -1 to be visible for all. |
| interior_id | [int32](#int32) |  | Interior id for which object will be visible. Set -1 to be visible for all. |
| player_id | [int32](#int32) |  | SA-MP player id for which object will be visible. Set -1 to be visible for all. |
| area_id | [int32](#int32) |  | Dynamic area id for which object will be visible. Set -1 to be visible for all. |
| stream_distance | [float](#float) |  | Default streamer setting is 300.0 |
| draw_distance | [float](#float) |  | Default streamer setting is 0.0 = default game draw distance |
| priority | [int32](#int32) |  |  |
| estate_id | [uint32](#uint32) |  |  |
| materials | [Object.MaterialsEntry](#mruv.objects.Object.MaterialsEntry) | repeated |  |
| material_texts | [Object.MaterialTextsEntry](#mruv.objects.Object.MaterialTextsEntry) | repeated |  |






<a name="mruv.objects.Object.MaterialTextsEntry"></a>

### Object.MaterialTextsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [MaterialText](#mruv.objects.MaterialText) |  |  |






<a name="mruv.objects.Object.MaterialsEntry"></a>

### Object.MaterialsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [Material](#mruv.objects.Material) |  |  |






<a name="mruv.objects.RemovedBuilding"></a>

### RemovedBuilding
Removes a standard San Andreas model for a single player within a specified range.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| model | [uint32](#uint32) |  | The model to remove. |
| x | [float](#float) |  | The X coordinate around which the objects will be removed. |
| y | [float](#float) |  | The Y coordinate around which the objects will be removed. |
| z | [float](#float) |  | The Z coordinate around which the objects will be removed. |
| radius | [float](#float) |  | The radius around the specified point to remove objects with the specified model. |
| estate_id | [uint32](#uint32) |  | Estate to with removed object belong. |






<a name="mruv.objects.UpdateObjectRequest"></a>

### UpdateObjectRequest
Request message for rpc `UpdateObject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| object | [Object](#mruv.objects.Object) |  |  |






<a name="mruv.objects.UpdateObjectResponse"></a>

### UpdateObjectResponse
Response message for rpc `UpdateObject`.





 


<a name="mruv.objects.MaterialSize"></a>

### MaterialSize


| Name | Number | Description |
| ---- | ------ | ----------- |
| OBJECT_MATERIAL_SIZE_0 | 0 |  |
| OBJECT_MATERIAL_SIZE_32X32 | 10 |  |
| OBJECT_MATERIAL_SIZE_64X32 | 20 |  |
| OBJECT_MATERIAL_SIZE_64X64 | 30 |  |
| OBJECT_MATERIAL_SIZE_128X32 | 40 |  |
| OBJECT_MATERIAL_SIZE_128X64 | 50 |  |
| OBJECT_MATERIAL_SIZE_128X128 | 60 |  |
| OBJECT_MATERIAL_SIZE_256X32 | 70 |  |
| OBJECT_MATERIAL_SIZE_256X64 | 80 |  |
| OBJECT_MATERIAL_SIZE_256X128 | 90 |  |
| OBJECT_MATERIAL_SIZE_256X256 | 100 |  |
| OBJECT_MATERIAL_SIZE_512X64 | 110 |  |
| OBJECT_MATERIAL_SIZE_512X128 | 120 |  |
| OBJECT_MATERIAL_SIZE_512X256 | 130 |  |
| OBJECT_MATERIAL_SIZE_512X512 | 140 |  |


 

 


<a name="mruv.objects.MruVObjectsService"></a>

### MruVObjectsService
The MruV objects service provides procedures for game objects.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateObject | [CreateObjectRequest](#mruv.objects.CreateObjectRequest) | [CreateObjectResponse](#mruv.objects.CreateObjectResponse) | Create an object. |
| GetObject | [GetObjectRequest](#mruv.objects.GetObjectRequest) | [GetObjectResponse](#mruv.objects.GetObjectResponse) | Get an object. |
| UpdateObject | [UpdateObjectRequest](#mruv.objects.UpdateObjectRequest) | [UpdateObjectResponse](#mruv.objects.UpdateObjectResponse) | Update an object. |
| DeleteObject | [DeleteObjectRequest](#mruv.objects.DeleteObjectRequest) | [DeleteObjectResponse](#mruv.objects.DeleteObjectResponse) | Delete an object. |
| AddObjectMaterial | [AddObjectMaterialRequest](#mruv.objects.AddObjectMaterialRequest) | [AddObjectMaterialResponse](#mruv.objects.AddObjectMaterialResponse) | Add a material to existing object. |
| GetObjectMaterials | [GetObjectMaterialsRequest](#mruv.objects.GetObjectMaterialsRequest) | [GetObjectMaterialsResponse](#mruv.objects.GetObjectMaterialsResponse) | Get all object materials. |
| DeleteObjectMaterial | [DeleteObjectMaterialRequest](#mruv.objects.DeleteObjectMaterialRequest) | [DeleteObjectMaterialResponse](#mruv.objects.DeleteObjectMaterialResponse) | Delete a material assigned to an object. |
| AddObjectMaterialText | [AddObjectMaterialTextRequest](#mruv.objects.AddObjectMaterialTextRequest) | [AddObjectMaterialTextResponse](#mruv.objects.AddObjectMaterialTextResponse) | Add a material text to existing object. |
| GetObjectMaterialTexts | [GetObjectMaterialTextsRequest](#mruv.objects.GetObjectMaterialTextsRequest) | [GetObjectMaterialTextsResponse](#mruv.objects.GetObjectMaterialTextsResponse) | Get all object material texts. |
| DeleteObjectMaterialText | [DeleteObjectMaterialTextRequest](#mruv.objects.DeleteObjectMaterialTextRequest) | [DeleteObjectMaterialTextResponse](#mruv.objects.DeleteObjectMaterialTextResponse) | Delete a material text assigned to an object. |
| AddRemoveBuilding | [AddRemoveBuildingRequest](#mruv.objects.AddRemoveBuildingRequest) | [AddRemoveBuildingResponse](#mruv.objects.AddRemoveBuildingResponse) | Removes a object from GTA SA map. |
| GetRemovedBuildings | [GetRemovedBuildingsRequest](#mruv.objects.GetRemovedBuildingsRequest) | [GetRemovedBuildingsResponse](#mruv.objects.GetRemovedBuildingsResponse) | Get all removed objects. |
| DeleteRemoveBuilding | [DeleteRemoveBuildingRequest](#mruv.objects.DeleteRemoveBuildingRequest) | [DeleteRemoveBuildingResponse](#mruv.objects.DeleteRemoveBuildingResponse) | Delete removed buildings. |
| FetchAllObjects | [FetchAllObjectsRequest](#mruv.objects.FetchAllObjectsRequest) | [FetchAllObjectsResponse](#mruv.objects.FetchAllObjectsResponse) stream | Fetch all existing objects. |

 



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

 



<a name="plots/plots.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## plots/plots.proto



<a name="mruv.plots.CreatePlotRequest"></a>

### CreatePlotRequest
Request message for rpc `CreatePlot`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |
| points | [mruv.common.Position](#mruv.common.Position) | repeated |  |






<a name="mruv.plots.CreatePlotResponse"></a>

### CreatePlotResponse
Response message for rpc `CreatePlot`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.plots.DeletePlotRequest"></a>

### DeletePlotRequest
Request message for rpc `DeletePlot`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.plots.DeletePlotResponse"></a>

### DeletePlotResponse
Response message for rpc `DeletePlot`.






<a name="mruv.plots.GetPlotRequest"></a>

### GetPlotRequest
Request message for rpc `GetPlot`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.plots.GetPlotResponse"></a>

### GetPlotResponse
Response message for rpc `GetPlot`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |
| points | [mruv.common.Position](#mruv.common.Position) | repeated |  |
| area | [double](#double) |  |  |






<a name="mruv.plots.Plot"></a>

### Plot



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |
| points | [mruv.common.Position](#mruv.common.Position) | repeated |  |






<a name="mruv.plots.UpdatePlotRequest"></a>

### UpdatePlotRequest
Request message for rpc `UpdatePlot`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |
| description | [string](#string) |  |  |






<a name="mruv.plots.UpdatePlotResponse"></a>

### UpdatePlotResponse
Response message for rpc `UpdatePlot`.





 

 

 


<a name="mruv.plots.MruVPlotsService"></a>

### MruVPlotsService
The MruV plots service provides procedures for managing buildings plots and other areas.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreatePlot | [CreatePlotRequest](#mruv.plots.CreatePlotRequest) | [CreatePlotResponse](#mruv.plots.CreatePlotResponse) | Create a plot. |
| GetPlot | [GetPlotRequest](#mruv.plots.GetPlotRequest) | [GetPlotResponse](#mruv.plots.GetPlotResponse) | Get a plot. |
| UpdatePlot | [UpdatePlotRequest](#mruv.plots.UpdatePlotRequest) | [UpdatePlotResponse](#mruv.plots.UpdatePlotResponse) | Update a plot. |
| DeletePlot | [DeletePlotRequest](#mruv.plots.DeletePlotRequest) | [DeletePlotResponse](#mruv.plots.DeletePlotResponse) | Delete a plot. |

 



<a name="punishments/punishments.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## punishments/punishments.proto



<a name="mruv.punishments.AdminJailMessage"></a>

### AdminJailMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  | A player, that owns a jailed character. |
| character | [uint32](#uint32) |  | Character that has been jailed. |
| reason | [string](#string) |  | An admin jail reason. |
| admin | [uint32](#uint32) |  | Admin that jail a player. 0 = system jail. |
| aj_date | [int64](#int64) |  | Date on which an admin jail was issued in Unix time. |
| jail_time | [uint32](#uint32) |  | Time of admin jail in seconds. |






<a name="mruv.punishments.AdminJailRequest"></a>

### AdminJailRequest
Request message for rpc `AdminJail`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [uint32](#uint32) |  |  |
| time | [uint32](#uint32) |  | Admin jail time. |
| reason | [string](#string) |  | Admin jail reason. |
| admin | [uint32](#uint32) |  | Admin that gave an admin jail to a player. |






<a name="mruv.punishments.AdminJailResponse"></a>

### AdminJailResponse
Response message for rpc `AdminJail`.






<a name="mruv.punishments.BanMessage"></a>

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






<a name="mruv.punishments.BanRequest"></a>

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






<a name="mruv.punishments.BanResponse"></a>

### BanResponse
Response message for rpc `Ban`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| ban_id | [uint32](#uint32) |  |  |






<a name="mruv.punishments.BlockMessage"></a>

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






<a name="mruv.punishments.BlockRequest"></a>

### BlockRequest
Request message for rpc `Block`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [uint32](#uint32) |  |  |
| reason | [string](#string) |  | Block reason. |
| admin | [uint32](#uint32) |  | Admin that blocked a player. 0 = system ban. |






<a name="mruv.punishments.BlockResponse"></a>

### BlockResponse
Response message for rpc `Block`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| block_id | [uint32](#uint32) |  |  |






<a name="mruv.punishments.GetBanRequest"></a>

### GetBanRequest
Request message for rpc `GetBan`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.punishments.GetBlockRequest"></a>

### GetBlockRequest
Request message for rpc `GetBlock`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.punishments.GetPlayerAdminJailRequest"></a>

### GetPlayerAdminJailRequest
Request message for rpc `GetPlayerAdminJail`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [uint32](#uint32) |  |  |






<a name="mruv.punishments.GetPlayerAdminJailResponse"></a>

### GetPlayerAdminJailResponse
Response message for rpc `GetPlayerAdminJail`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| jail_time | [uint32](#uint32) |  | Time of admin jail in seconds. |
| reason | [string](#string) |  | Admin jail reason. |
| admin | [uint32](#uint32) |  | An admin that put a player in the admin jail. |
| date | [int64](#int64) |  | Date when the player was thrown into admin jail in Unix time. |






<a name="mruv.punishments.GetPlayerBansRequest"></a>

### GetPlayerBansRequest
Request message for rpc `GetPlayerBans`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| ip | [string](#string) |  |  |






<a name="mruv.punishments.GetPlayerBansResponse"></a>

### GetPlayerBansResponse
Response message for rpc `GetPlayerBans`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| bans | [BanMessage](#mruv.punishments.BanMessage) | repeated |  |






<a name="mruv.punishments.GetPlayerWarnsRequest"></a>

### GetPlayerWarnsRequest
Request message for rpc `GetPlayerWarns`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |






<a name="mruv.punishments.GetPlayerWarnsResponse"></a>

### GetPlayerWarnsResponse
Response message for rpc `GetPlayerWarns`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| warns | [WarnMessage](#mruv.punishments.WarnMessage) | repeated |  |






<a name="mruv.punishments.GetWarnRequest"></a>

### GetWarnRequest
Request message for rpc `GetWarn`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.punishments.IsCharacterBlockedRequest"></a>

### IsCharacterBlockedRequest
Request message for rpc `IsCharacterBlocked`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [uint32](#uint32) |  |  |






<a name="mruv.punishments.IsCharacterBlockedResponse"></a>

### IsCharacterBlockedResponse
Response message for rpc `IsCharacterBlocked`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| blocked | [bool](#bool) |  |  |
| block_id | [uint32](#uint32) |  |  |






<a name="mruv.punishments.IsCharacterJailedRequest"></a>

### IsCharacterJailedRequest
Request message for rpc `IsCharacterJailed`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [uint32](#uint32) |  |  |






<a name="mruv.punishments.IsCharacterJailedResponse"></a>

### IsCharacterJailedResponse
Response message for rpc `IsCharacterJailed`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| jailed | [bool](#bool) |  |  |
| jail_time | [uint32](#uint32) |  |  |






<a name="mruv.punishments.IsPlayerBannedRequest"></a>

### IsPlayerBannedRequest
Request message for rpc `IsPlayerBanned`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| ip | [string](#string) |  |  |






<a name="mruv.punishments.IsPlayerBannedResponse"></a>

### IsPlayerBannedResponse
Response message for rpc `IsPlayerBanned`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| banned | [bool](#bool) |  |  |
| ban_id | [uint32](#uint32) |  |  |






<a name="mruv.punishments.MuteGlobalChatsRequest"></a>

### MuteGlobalChatsRequest
Request message for rpc `MuteGlobalChats`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| account | [uint32](#uint32) |  |  |






<a name="mruv.punishments.MuteGlobalChatsResponse"></a>

### MuteGlobalChatsResponse
Response message for rpc `MuteGlobalChats`.






<a name="mruv.punishments.UnAdminJailMessage"></a>

### UnAdminJailMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| character | [uint32](#uint32) |  |  |






<a name="mruv.punishments.UnAdminJailRequest"></a>

### UnAdminJailRequest
Request message for rpc `UnAdminJail`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| character | [uint32](#uint32) |  |  |






<a name="mruv.punishments.UnAdminJailResponse"></a>

### UnAdminJailResponse
Response message for rpc `UnAdminJail`.






<a name="mruv.punishments.UnBanMessage"></a>

### UnBanMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| ban_id | [uint32](#uint32) |  |  |






<a name="mruv.punishments.UnBanRequest"></a>

### UnBanRequest
Request message for rpc `UnBan`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| ban_id | [uint32](#uint32) |  |  |
| reason | [string](#string) |  |  |






<a name="mruv.punishments.UnBanResponse"></a>

### UnBanResponse
Response message for rpc `UnBan`.






<a name="mruv.punishments.UnBlockMessage"></a>

### UnBlockMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| block_id | [uint32](#uint32) |  |  |






<a name="mruv.punishments.UnBlockRequest"></a>

### UnBlockRequest
Request message for rpc `UnBlock`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| block_id | [uint32](#uint32) |  |  |
| reason | [string](#string) |  |  |






<a name="mruv.punishments.UnBlockResponse"></a>

### UnBlockResponse
Response message for rpc `UnBlock`.






<a name="mruv.punishments.UnMuteGlobalChatsRequest"></a>

### UnMuteGlobalChatsRequest
Request message for rpc `UnMuteGlobalChats`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| account | [uint32](#uint32) |  |  |






<a name="mruv.punishments.UnMuteGlobalChatsResponse"></a>

### UnMuteGlobalChatsResponse
Response message for rpc `UnMuteGlobalChats`.






<a name="mruv.punishments.UnWarnMessage"></a>

### UnWarnMessage



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| warn_id | [uint32](#uint32) |  |  |






<a name="mruv.punishments.UnWarnRequest"></a>

### UnWarnRequest
Request message for rpc `UnWarn`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| warn_id | [uint32](#uint32) |  |  |
| reason | [string](#string) |  |  |






<a name="mruv.punishments.UnWarnResponse"></a>

### UnWarnResponse
Response message for rpc `UnWarn`.






<a name="mruv.punishments.WarnMessage"></a>

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






<a name="mruv.punishments.WarnRequest"></a>

### WarnRequest
Request message for rpc `Warn`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| player | [uint32](#uint32) |  |  |
| character | [uint32](#uint32) |  | Player character that was accused. Optional. |
| time | [uint32](#uint32) |  | Warn expiration time in days. 0 = permanent warn. |
| reason | [string](#string) |  | Warn reason. |
| admin | [uint32](#uint32) |  | Admin that warned player. 0 = system warn. |






<a name="mruv.punishments.WarnResponse"></a>

### WarnResponse
Response message for rpc `Warn`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| warn_id | [uint32](#uint32) |  |  |






<a name="mruv.punishments.WatchAdminJailsRequest"></a>

### WatchAdminJailsRequest
Request message for rpc `WatchAdminJails`.






<a name="mruv.punishments.WatchBansRequest"></a>

### WatchBansRequest
Request message for rpc `WatchBans`.






<a name="mruv.punishments.WatchBlocksRequest"></a>

### WatchBlocksRequest
Request message for rpc `WatchBlocks`.






<a name="mruv.punishments.WatchPlayerAcquittalsRequest"></a>

### WatchPlayerAcquittalsRequest
Request message for rpc `WatchPlayerAcquittals`.






<a name="mruv.punishments.WatchPlayerAcquittalsResponse"></a>

### WatchPlayerAcquittalsResponse
Response message for rpc `WatchPlayerAcquittals`.






<a name="mruv.punishments.WatchPlayerPunishmentsRequest"></a>

### WatchPlayerPunishmentsRequest
Request message for rpc `WatchPlayerPunishments`.






<a name="mruv.punishments.WatchPlayerPunishmentsResponse"></a>

### WatchPlayerPunishmentsResponse
Response message for rpc `WatchPlayerPunishments`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| type | [PunishmentType](#mruv.punishments.PunishmentType) |  |  |
| punishment_id | [uint32](#uint32) |  |  |






<a name="mruv.punishments.WatchPunishmentsRequest"></a>

### WatchPunishmentsRequest
Request message for rpc `WatchPunishments`.






<a name="mruv.punishments.WatchPunishmentsResponse"></a>

### WatchPunishmentsResponse
Response message for rpc `WatchPunishments`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| type | [PunishmentType](#mruv.punishments.PunishmentType) |  |  |
| punishment_id | [uint32](#uint32) |  |  |
| player | [uint32](#uint32) |  |  |
| character | [uint32](#uint32) |  |  |






<a name="mruv.punishments.WatchUnAdminJailsRequest"></a>

### WatchUnAdminJailsRequest
Request message for rpc `WatchUnAdminJails`.






<a name="mruv.punishments.WatchUnBansRequest"></a>

### WatchUnBansRequest
Request message for rpc `WatchUnBans`.






<a name="mruv.punishments.WatchUnBlocksRequest"></a>

### WatchUnBlocksRequest
Request message for rpc `WatchUnBlocks`.






<a name="mruv.punishments.WatchUnWarnsRequest"></a>

### WatchUnWarnsRequest
Request message for rpc `WatchUnWarns`.






<a name="mruv.punishments.WatchWarnsRequest"></a>

### WatchWarnsRequest
Request message for rpc `WatchWarns`.





 


<a name="mruv.punishments.AcquittalsType"></a>

### AcquittalsType


| Name | Number | Description |
| ---- | ------ | ----------- |
| UNKNOWN_ACQUITAL | 0 |  |
| UNBAN | 1 |  |
| UNBLOCK | 2 |  |
| UNWARN | 3 |  |
| UN_ADMIN_JAIL | 4 |  |



<a name="mruv.punishments.PunishmentType"></a>

### PunishmentType


| Name | Number | Description |
| ---- | ------ | ----------- |
| UNKNOWN_PUNISHMENT | 0 |  |
| BAN | 1 |  |
| BLOCK | 2 |  |
| WARN | 3 |  |
| ADMIN_JAIL | 4 |  |


 

 


<a name="mruv.punishments.MruVPunishmentsService"></a>

### MruVPunishmentsService
This service provides interface for managing punishments for players.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| Ban | [BanRequest](#mruv.punishments.BanRequest) | [BanResponse](#mruv.punishments.BanResponse) | Ban player on account and/or ip. If ban_time is 0, ban will never expire. |
| Block | [BlockRequest](#mruv.punishments.BlockRequest) | [BlockResponse](#mruv.punishments.BlockResponse) | Block player character. |
| Warn | [WarnRequest](#mruv.punishments.WarnRequest) | [WarnResponse](#mruv.punishments.WarnResponse) | Warn player. If warn_time is 0, warn will never expire. |
| AdminJail | [AdminJailRequest](#mruv.punishments.AdminJailRequest) | [AdminJailResponse](#mruv.punishments.AdminJailResponse) | Put player in an admin jail. |
| MuteGlobalChats | [MuteGlobalChatsRequest](#mruv.punishments.MuteGlobalChatsRequest) | [MuteGlobalChatsResponse](#mruv.punishments.MuteGlobalChatsResponse) | Mute player global chats. |
| UnBan | [UnBanRequest](#mruv.punishments.UnBanRequest) | [UnBanResponse](#mruv.punishments.UnBanResponse) | Deactivate a specific player ban. |
| UnBlock | [UnBlockRequest](#mruv.punishments.UnBlockRequest) | [UnBlockResponse](#mruv.punishments.UnBlockResponse) | Deactivate a character block. |
| UnWarn | [UnWarnRequest](#mruv.punishments.UnWarnRequest) | [UnWarnResponse](#mruv.punishments.UnWarnResponse) | Deactivate a specific player warning. If a player was banned by reaching the warning limit, a player will be unbanned. |
| UnAdminJail | [UnAdminJailRequest](#mruv.punishments.UnAdminJailRequest) | [UnAdminJailResponse](#mruv.punishments.UnAdminJailResponse) | Remove player from admin jail. |
| UnMuteGlobalChats | [UnMuteGlobalChatsRequest](#mruv.punishments.UnMuteGlobalChatsRequest) | [UnMuteGlobalChatsResponse](#mruv.punishments.UnMuteGlobalChatsResponse) |  |
| GetPlayerBans | [GetPlayerBansRequest](#mruv.punishments.GetPlayerBansRequest) | [GetPlayerBansResponse](#mruv.punishments.GetPlayerBansResponse) | Get all player bans. |
| GetPlayerWarns | [GetPlayerWarnsRequest](#mruv.punishments.GetPlayerWarnsRequest) | [GetPlayerWarnsResponse](#mruv.punishments.GetPlayerWarnsResponse) | Get all player warns. |
| GetPlayerAdminJail | [GetPlayerAdminJailRequest](#mruv.punishments.GetPlayerAdminJailRequest) | [GetPlayerAdminJailResponse](#mruv.punishments.GetPlayerAdminJailResponse) | Get player admin jail time. |
| GetBan | [GetBanRequest](#mruv.punishments.GetBanRequest) | [BanMessage](#mruv.punishments.BanMessage) | Get ban info. |
| GetWarn | [GetWarnRequest](#mruv.punishments.GetWarnRequest) | [WarnMessage](#mruv.punishments.WarnMessage) | Get warn info. |
| GetBlock | [GetBlockRequest](#mruv.punishments.GetBlockRequest) | [BlockMessage](#mruv.punishments.BlockMessage) | Get block info. |
| IsPlayerBanned | [IsPlayerBannedRequest](#mruv.punishments.IsPlayerBannedRequest) | [IsPlayerBannedResponse](#mruv.punishments.IsPlayerBannedResponse) | Check is player or ip banned. |
| IsCharacterBlocked | [IsCharacterBlockedRequest](#mruv.punishments.IsCharacterBlockedRequest) | [IsCharacterBlockedResponse](#mruv.punishments.IsCharacterBlockedResponse) | Check is character is blocked. |
| IsCharacterJailed | [IsCharacterJailedRequest](#mruv.punishments.IsCharacterJailedRequest) | [IsCharacterJailedResponse](#mruv.punishments.IsCharacterJailedResponse) |  |
| WatchBans | [WatchBansRequest](#mruv.punishments.WatchBansRequest) | [BanMessage](#mruv.punishments.BanMessage) stream | Subscribe to ban events. |
| WatchBlocks | [WatchBlocksRequest](#mruv.punishments.WatchBlocksRequest) | [BlockMessage](#mruv.punishments.BlockMessage) stream | Subscribe to block events. |
| WatchWarns | [WatchWarnsRequest](#mruv.punishments.WatchWarnsRequest) | [WarnMessage](#mruv.punishments.WarnMessage) stream | Subscribe to warn events. |
| WatchAdminJails | [WatchAdminJailsRequest](#mruv.punishments.WatchAdminJailsRequest) | [AdminJailMessage](#mruv.punishments.AdminJailMessage) stream | Subscribe to admin jail events. |
| WatchUnBans | [WatchUnBansRequest](#mruv.punishments.WatchUnBansRequest) | [UnBanMessage](#mruv.punishments.UnBanMessage) stream | Subscribe to unban events. |
| WatchUnBlocks | [WatchUnBlocksRequest](#mruv.punishments.WatchUnBlocksRequest) | [UnBlockMessage](#mruv.punishments.UnBlockMessage) stream | Subscribe to unblock events. |
| WatchUnWarns | [WatchUnWarnsRequest](#mruv.punishments.WatchUnWarnsRequest) | [UnWarnMessage](#mruv.punishments.UnWarnMessage) stream | Subscribe to unwarn events. |
| WatchUnAdminJails | [WatchUnAdminJailsRequest](#mruv.punishments.WatchUnAdminJailsRequest) | [UnAdminJailMessage](#mruv.punishments.UnAdminJailMessage) stream | Subscribe to admin jail release events. |
| WatchPlayerPunishments | [WatchPlayerPunishmentsRequest](#mruv.punishments.WatchPlayerPunishmentsRequest) | [WatchPlayerPunishmentsResponse](#mruv.punishments.WatchPlayerPunishmentsResponse) stream | Subscribe to player punishments. |
| WatchPlayerAcquittals | [WatchPlayerAcquittalsRequest](#mruv.punishments.WatchPlayerAcquittalsRequest) | [WatchPlayerAcquittalsResponse](#mruv.punishments.WatchPlayerAcquittalsResponse) stream | Subscribe to player acquittals. |
| WatchPunishments | [WatchPunishmentsRequest](#mruv.punishments.WatchPunishmentsRequest) | [WatchPunishmentsResponse](#mruv.punishments.WatchPunishmentsResponse) stream | Subscribe to all punishments and acquittals events. |

 



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


 

 

 



<a name="spots/spots.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## spots/spots.proto



<a name="mruv.spots.CreateSpotRequest"></a>

### CreateSpotRequest
Request message for rpc `CreateSpot`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| spot | [Spot](#mruv.spots.Spot) |  |  |






<a name="mruv.spots.CreateSpotResponse"></a>

### CreateSpotResponse
Response message for rpc `CreateSpot`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.spots.DeleteSpotRequest"></a>

### DeleteSpotRequest
Request message for rpc `DeleteSpot`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.spots.DeleteSpotResponse"></a>

### DeleteSpotResponse
Response message for rpc `DeleteSpot`.






<a name="mruv.spots.FetchAllSpotsRequest"></a>

### FetchAllSpotsRequest
Request message for rpc `FetchAllSpots`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| chunk_size | [uint32](#uint32) |  |  |






<a name="mruv.spots.FetchAllSpotsResponse"></a>

### FetchAllSpotsResponse
Response message for rpc `FetchAllSpots`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| spots | [FetchAllSpotsResponse.SpotsEntry](#mruv.spots.FetchAllSpotsResponse.SpotsEntry) | repeated |  |






<a name="mruv.spots.FetchAllSpotsResponse.SpotsEntry"></a>

### FetchAllSpotsResponse.SpotsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [uint32](#uint32) |  |  |
| value | [Spot](#mruv.spots.Spot) |  |  |






<a name="mruv.spots.GetSpotRequest"></a>

### GetSpotRequest
Request message for rpc `GetSpot`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="mruv.spots.GetSpotResponse"></a>

### GetSpotResponse
Response message for rpc `GetSpot`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| spot | [Spot](#mruv.spots.Spot) |  |  |






<a name="mruv.spots.Spot"></a>

### Spot
Spot.


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






<a name="mruv.spots.UpdateSpotRequest"></a>

### UpdateSpotRequest
Request message for rpc `UpdateSpot`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| spot | [Spot](#mruv.spots.Spot) |  |  |






<a name="mruv.spots.UpdateSpotResponse"></a>

### UpdateSpotResponse
Response message for rpc `UpdateSpot`.





 

 

 


<a name="mruv.spots.MruVSpotsService"></a>

### MruVSpotsService
The MruV spots service provides procedures for managing spots.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateSpot | [CreateSpotRequest](#mruv.spots.CreateSpotRequest) | [CreateSpotResponse](#mruv.spots.CreateSpotResponse) | Create a spot. |
| GetSpot | [GetSpotRequest](#mruv.spots.GetSpotRequest) | [GetSpotResponse](#mruv.spots.GetSpotResponse) | Get a spot. |
| UpdateSpot | [UpdateSpotRequest](#mruv.spots.UpdateSpotRequest) | [UpdateSpotResponse](#mruv.spots.UpdateSpotResponse) | Update a spot. |
| DeleteSpot | [DeleteSpotRequest](#mruv.spots.DeleteSpotRequest) | [DeleteSpotResponse](#mruv.spots.DeleteSpotResponse) | Delete a spot. |
| FetchAll | [FetchAllSpotsRequest](#mruv.spots.FetchAllSpotsRequest) | [FetchAllSpotsResponse](#mruv.spots.FetchAllSpotsResponse) stream | Fetch all spots. |

 



<a name="texturestudio/texturestudio_manage.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## texturestudio/texturestudio_manage.proto



<a name="texture_studio.CreateServerRequest"></a>

### CreateServerRequest
Request message for rpc `CreateServer`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| owner_id | [uint32](#uint32) |  |  |






<a name="texture_studio.CreateServerResponse"></a>

### CreateServerResponse
Response message for rpc `CreateServer`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |
| port | [uint32](#uint32) |  |  |






<a name="texture_studio.DeleteServerRequest"></a>

### DeleteServerRequest
Request message for rpc `DeleteServer`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="texture_studio.DeleteServerResponse"></a>

### DeleteServerResponse
Response message for rpc `DeleteServer`.






<a name="texture_studio.GetServersRequest"></a>

### GetServersRequest
Request message for rpc `GetServers`.






<a name="texture_studio.GetServersResponse"></a>

### GetServersResponse
Response message for rpc `GetServers`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) | repeated |  |






<a name="texture_studio.MyServerRequest"></a>

### MyServerRequest
Request message for rpc `MyServer`.






<a name="texture_studio.MyServerResponse"></a>

### MyServerResponse
Response message for rpc `MyServer`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="texture_studio.TransferOwnershipRequest"></a>

### TransferOwnershipRequest
Request message for rpc `TransferOwnership`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| server_id | [uint32](#uint32) |  |  |
| owner_id | [uint32](#uint32) |  |  |






<a name="texture_studio.TransferOwnershipResponse"></a>

### TransferOwnershipResponse
Response message for rpc `TransferOwnership`.





 

 

 


<a name="texture_studio.TextureStudioManagerService"></a>

### TextureStudioManagerService
Service to manage texture studio servers cluster.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| CreateServer | [CreateServerRequest](#texture_studio.CreateServerRequest) | [CreateServerResponse](#texture_studio.CreateServerResponse) | Create a new texture studio server. |
| GetServers | [GetServersRequest](#texture_studio.GetServersRequest) | [GetServersResponse](#texture_studio.GetServersResponse) | Get all existing servers |
| MyServer | [MyServerRequest](#texture_studio.MyServerRequest) | [MyServerResponse](#texture_studio.MyServerResponse) | Get texture studio server id for current user. |
| TransferOwnership | [TransferOwnershipRequest](#texture_studio.TransferOwnershipRequest) | [TransferOwnershipResponse](#texture_studio.TransferOwnershipResponse) | Change owner of texture studio server. |
| DeleteServer | [DeleteServerRequest](#texture_studio.DeleteServerRequest) | [DeleteServerResponse](#texture_studio.DeleteServerResponse) | Delete a texture studio server. |

 



<a name="texturestudio/texturestudio_server.proto"></a>
<p align="right"><a href="#top">Top</a></p>

## texturestudio/texturestudio_server.proto



<a name="texture_studio.GetProjectRequest"></a>

### GetProjectRequest
Request message for rpc `GetProject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| server_id | [uint32](#uint32) |  |  |
| name | [string](#string) |  |  |






<a name="texture_studio.GetProjectResponse"></a>

### GetProjectResponse
Response message for rpc `GetProject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| code | [string](#string) |  |  |






<a name="texture_studio.GetProjectsRequest"></a>

### GetProjectsRequest
Request message for rpc `GetProjects`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| server_id | [uint32](#uint32) |  |  |






<a name="texture_studio.GetProjectsResponse"></a>

### GetProjectsResponse
Response message for rpc `GetProjects`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| names | [string](#string) | repeated |  |






<a name="texture_studio.RestartServerRequest"></a>

### RestartServerRequest
Request message for rpc `RestartServer`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="texture_studio.RestartServerResponse"></a>

### RestartServerResponse
Response message for rpc `RestartServer`.






<a name="texture_studio.ServerStatusRequest"></a>

### ServerStatusRequest
Request message for rpc `ServerStatus`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="texture_studio.ServerStatusResponse"></a>

### ServerStatusResponse
Response message for rpc `ServerStatus`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| port | [uint32](#uint32) |  |  |
| status | [ServerStatus](#texture_studio.ServerStatus) |  |  |






<a name="texture_studio.StartServerRequest"></a>

### StartServerRequest
Request message for rpc `StartServer`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="texture_studio.StartServerResponse"></a>

### StartServerResponse
Response message for rpc `StartServer`.






<a name="texture_studio.StopServerRequest"></a>

### StopServerRequest
Request message for rpc `StopServer`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [uint32](#uint32) |  |  |






<a name="texture_studio.StopServerResponse"></a>

### StopServerResponse
Response message for rpc `StopServer`.






<a name="texture_studio.SubscribeToProjectsChangesRequest"></a>

### SubscribeToProjectsChangesRequest
Request message for rpc `SubscribeToProjectsChanges`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| server_id | [uint32](#uint32) |  |  |






<a name="texture_studio.SubscribeToProjectsChangesResponse"></a>

### SubscribeToProjectsChangesResponse
Response message for rpc `SubscribeToProjectsChanges`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| name | [string](#string) |  |  |






<a name="texture_studio.UploadProjectRequest"></a>

### UploadProjectRequest
Request message for rpc `UploadProject`.


| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| server_id | [uint32](#uint32) |  |  |
| project_name | [string](#string) |  |  |
| code | [string](#string) |  |  |
| file | [bytes](#bytes) |  |  |






<a name="texture_studio.UploadProjectResponse"></a>

### UploadProjectResponse
Response message for rpc `UploadProject`.





 


<a name="texture_studio.ServerStatus"></a>

### ServerStatus


| Name | Number | Description |
| ---- | ------ | ----------- |
| UNKNOWN_STATUS | 0 |  |
| ON | 1 |  |
| OFF | 2 |  |


 

 


<a name="texture_studio.TextureStudioServerService"></a>

### TextureStudioServerService
Service to manage texture studio server.

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| StartServer | [StartServerRequest](#texture_studio.StartServerRequest) | [StartServerResponse](#texture_studio.StartServerResponse) | Start a texture studio server. |
| StopServer | [StopServerRequest](#texture_studio.StopServerRequest) | [StopServerResponse](#texture_studio.StopServerResponse) | Stop a texture studio server. |
| RestartServer | [RestartServerRequest](#texture_studio.RestartServerRequest) | [RestartServerResponse](#texture_studio.RestartServerResponse) | Restart a texture studio server. |
| ServerStatus | [ServerStatusRequest](#texture_studio.ServerStatusRequest) | [ServerStatusResponse](#texture_studio.ServerStatusResponse) | Get texture studio server status. |
| UploadProject | [UploadProjectRequest](#texture_studio.UploadProjectRequest) | [UploadProjectResponse](#texture_studio.UploadProjectResponse) | Upload project to texture studio. |
| GetProject | [GetProjectRequest](#texture_studio.GetProjectRequest) | [GetProjectResponse](#texture_studio.GetProjectResponse) | Get texture-studio objects project. |
| GetProjects | [GetProjectsRequest](#texture_studio.GetProjectsRequest) | [GetProjectsResponse](#texture_studio.GetProjectsResponse) | Get all projects. |
| SubscribeToProjectsChanges | [SubscribeToProjectsChangesRequest](#texture_studio.SubscribeToProjectsChangesRequest) | [SubscribeToProjectsChangesResponse](#texture_studio.SubscribeToProjectsChangesResponse) stream | Listen for project changes - if texture studio project has been created or modified, this will trigger an event. |

 



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

