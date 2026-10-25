# ImageSharingConstants

source `interface/addons/blizzard_apidocumentationgenerated/imagesharingconstantsdocumentation.lua` (FileDataID 7701853)

## Types

### ImageSharingResult

*Enumeration* · 15 values, 0..14

Access values as `Enum.ImageSharingResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Failure` | `ImageSharingResult` | = 0 |
| `Success` | `ImageSharingResult` | = 1 |
| `NotConfigured` | `ImageSharingResult` | = 2 |
| `RetrievedExisting` | `ImageSharingResult` | = 3 |
| `PlatformApiError` | `ImageSharingResult` | = 4 |
| `MissingFieldApiError` | `ImageSharingResult` | = 5 |
| `AccountDataRequestFailure` | `ImageSharingResult` | = 6 |
| `GetAccountDataRequestFailure` | `ImageSharingResult` | = 7 |
| `SetAccountDataRequestFailure` | `ImageSharingResult` | = 8 |
| `RefreshTokenExpired` | `ImageSharingResult` | = 9 |
| `FailedToCreateHeader` | `ImageSharingResult` | = 10 |
| `EncryptionFailure` | `ImageSharingResult` | = 11 |
| `InvalidOAuthExpiration` | `ImageSharingResult` | = 12 |
| `InvalidRefreshExpiration` | `ImageSharingResult` | = 13 |
| `EncryptionSecretNotSet` | `ImageSharingResult` | = 14 |

### PhotoSharingStatus

*Enumeration* · 9 values, 0..8

Access values as `Enum.PhotoSharingStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Disabled` | `PhotoSharingStatus` | = 0 |
| `NotConfigured` | `PhotoSharingStatus` | = 1 |
| `Configured` | `PhotoSharingStatus` | = 2 |
| `Expired` | `PhotoSharingStatus` | = 3 |
| `ParentalControl` | `PhotoSharingStatus` | = 4 |
| `TrialOrVeteran` | `PhotoSharingStatus` | = 5 |
| `AADCRestricted` | `PhotoSharingStatus` | = 6 |
| `Error` | `PhotoSharingStatus` | = 7 |
| `FailedToClear` | `PhotoSharingStatus` | = 8 |

### PhotoSharingUploadStatus

*Enumeration* · 30 values, 0..29

Access values as `Enum.PhotoSharingUploadStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Disabled` | `PhotoSharingUploadStatus` | = 0 |
| `Failed` | `PhotoSharingUploadStatus` | = 1 |
| `Success` | `PhotoSharingUploadStatus` | = 2 |
| `Locked` | `PhotoSharingUploadStatus` | = 3 |
| `ListPagesApiCallFailed` | `PhotoSharingUploadStatus` | = 4 |
| `ListPagesBadRequest` | `PhotoSharingUploadStatus` | = 5 |
| `ListPagesUnauthorized` | `PhotoSharingUploadStatus` | = 6 |
| `ListPagesForbidden` | `PhotoSharingUploadStatus` | = 7 |
| `ListPagesNotFound` | `PhotoSharingUploadStatus` | = 8 |
| `ListPagesTooManyRequests` | `PhotoSharingUploadStatus` | = 9 |
| `ListPagesGenericFailure` | `PhotoSharingUploadStatus` | = 10 |
| `ListPagesEmptyBoardID` | `PhotoSharingUploadStatus` | = 11 |
| `ListPagesInvalidBookmark` | `PhotoSharingUploadStatus` | = 12 |
| `CreatePageApiCallFailed` | `PhotoSharingUploadStatus` | = 13 |
| `CreatePageBadRequest` | `PhotoSharingUploadStatus` | = 14 |
| `CreatePageUnauthorized` | `PhotoSharingUploadStatus` | = 15 |
| `CreatePageForbidden` | `PhotoSharingUploadStatus` | = 16 |
| `CreatePageNotFound` | `PhotoSharingUploadStatus` | = 17 |
| `CreatePageTooManyRequests` | `PhotoSharingUploadStatus` | = 18 |
| `CreatePageGenericFailure` | `PhotoSharingUploadStatus` | = 19 |
| `CreatePageNoBoardIDFound` | `PhotoSharingUploadStatus` | = 20 |
| `CreatePostApiCallFailed` | `PhotoSharingUploadStatus` | = 21 |
| `CreatePostBadRequest` | `PhotoSharingUploadStatus` | = 22 |
| `CreatePostUnauthorized` | `PhotoSharingUploadStatus` | = 23 |
| `CreatePostForbidden` | `PhotoSharingUploadStatus` | = 24 |
| `CreatePostNotFound` | `PhotoSharingUploadStatus` | = 25 |
| `CreatePostTooManyRequests` | `PhotoSharingUploadStatus` | = 26 |
| `CreatePostGenericFailure` | `PhotoSharingUploadStatus` | = 27 |
| `CreatePostNoIDFound` | `PhotoSharingUploadStatus` | = 28 |
| `CreatePostThrottled` | `PhotoSharingUploadStatus` | = 29 |
