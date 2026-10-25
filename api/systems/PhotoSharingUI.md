# PhotoSharingUI

Namespace `C_PhotoSharing` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/photosharinguidocumentation.lua` (FileDataID 7792171)

## Functions

### BeginAuthorizationFlow

```lua
C_PhotoSharing.BeginAuthorizationFlow()
```

### ClearAuthorization

```lua
C_PhotoSharing.ClearAuthorization()
```

### CompleteAuthorizationFlow

```lua
C_PhotoSharing.CompleteAuthorizationFlow(callbackURL: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### GetCropRatio

```lua
C_PhotoSharing.GetCropRatio() -> cropRatio: number
```

### GetPhotoSharingAuthURL

```lua
C_PhotoSharing.GetPhotoSharingAuthURL() -> authUrl: cstring
```

### GetStatus

```lua
C_PhotoSharing.GetStatus() -> status: PhotoSharingStatus
```

### IsAuthorized

```lua
C_PhotoSharing.IsAuthorized() -> authorized: bool
```

### IsEnabled

```lua
C_PhotoSharing.IsEnabled() -> enabled: bool
```

### SetScreenshotPreviewTexture

```lua
C_PhotoSharing.SetScreenshotPreviewTexture(textureObject: SimpleTexture)
```

`SecretArguments=AllowedWhenUntainted`

### TakePhoto

```lua
C_PhotoSharing.TakePhoto()
```

### UploadPhotoToService

```lua
C_PhotoSharing.UploadPhotoToService(optionalTitle: cstring, optionalDescription: cstring)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `optionalTitle` | `cstring` | default `""` |
| `optionalDescription` | `cstring` | default `""` |

## Events

### PHOTO_SHARING_AUTHORIZATION_NEEDED

```lua
PHOTO_SHARING_AUTHORIZATION_NEEDED()
```

`SynchronousEvent`

### PHOTO_SHARING_AUTHORIZATION_UPDATED

```lua
PHOTO_SHARING_AUTHORIZATION_UPDATED(showNotification: bool)
```

`SynchronousEvent`

### PHOTO_SHARING_PHOTO_UPLOAD_STATUS

```lua
PHOTO_SHARING_PHOTO_UPLOAD_STATUS(uploadStatus: PhotoSharingUploadStatus)
```

`SynchronousEvent`

### PHOTO_SHARING_SCREENSHOT_READY

```lua
PHOTO_SHARING_SCREENSHOT_READY()
```

`SynchronousEvent`

### PHOTO_SHARING_THIRD_PARTY_AUTHORIZATION_NEEDED

```lua
PHOTO_SHARING_THIRD_PARTY_AUTHORIZATION_NEEDED(authUrl: string)
```

`SynchronousEvent`
