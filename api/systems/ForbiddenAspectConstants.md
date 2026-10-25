# ForbiddenAspectConstants

source `interface/addons/blizzard_apidocumentationgenerated/forbiddenaspectconstantsdocumentation.lua` (FileDataID 8119707)

## Types

### ForbiddenAspect

*Enumeration* · 15 values, 1..16384

Access values as `Enum.ForbiddenAspect.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `SetToDefaults` | `ForbiddenAspect` | = 1; Restricts resetting this object to a default state. Implied automatically when any other forbidden aspect is set. |
| `ScriptBindings` | `ForbiddenAspect` | = 2; Restricts querying, replacement, or hooks of scripts on this object. |
| `UntrustedScriptExecution` | `ForbiddenAspect` | = 4; Restricts execution of all scripts for this object. Propagates to any children of this object. |
| `UntrustedLayoutScriptExecution` | `ForbiddenAspect` | = 8; Restricts execution of layout scripts (eg. OnSizeChanged) for this object. Propagates to any children of this object, and anything anchored to to this object. |
| `EventRegistrations` | `ForbiddenAspect` | = 16; Restricts querying or modifying registered script events for this object. |
| `AlwaysPropagateInput` | `ForbiddenAspect` | = 32; Forces propagation of mouse and keypress input for this object. Propagates to any children. |
| `ScriptedInput` | `ForbiddenAspect` | = 64; Restricts APIs that trigger synthetic input interactions on objects from Lua scripts. |
| `QueryFocus` | `ForbiddenAspect` | = 128; Restricts APIs that query input focus state. |
| `ChangeAnimationTarget` | `ForbiddenAspect` | = 256; Restricts APIs that can change the target object of an animation. |
| `RemoveSecretAspects` | `ForbiddenAspect` | = 512; Restricts APIs that clear secret aspects from objects. |
| `ChangeParent` | `ForbiddenAspect` | = 1024; Restricts APIs that change the parent of an object. |
| `SetTexture` | `ForbiddenAspect` | = 2048; Restricts APIs that set the texture on a texture object. |
| `QueryRotation` | `ForbiddenAspect` | = 4096; Restricts APIs that query texture rotation. |
| `QueryAnimationProgress` | `ForbiddenAspect` | = 8192; Restricts APIs that query the progress or state of animations. |
| `AddAnimations` | `ForbiddenAspect` | = 16384; Restricts APIs that add animations to animation groups. |
