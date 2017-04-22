# Version 1.0.24.41 (2017-04-15)
## Module Manifest
* Cleaned up white space at end of file

## Functions
### Import-GraphApplication
* Now provides its own error instead of Import-clixml

### Import-GraphOauthAccessToken
* Now provides its own error instead of Import-clixml

### Get-AADGroupMember
* Added ResultsPerPage Paramter to provide access to '$top' query filter.
* Addeed .LINK to Get-AADGroupById
* Addeed .LINK to Get-AADGroupByDisplayName
* Added .INPUTS MSGraphAPI.DirectoryObject.Group
* Added .OUTPUTS MSGraphAPI.DirectoryObject.User

### Get-AADGroupById
* Addeed .LINK to Get-AADGroupByDisplayName
* Addeed .LINK to Get-AADGroupMember

### Get-AADGroupByDisplayName
* Addeed .LINK to Get-AADGroupMember
* Addeed .LINK to Get-AADGroupById

### Get-GraphOauthAccessToken
* **Breaking Change**: Removed ```ResultVariable``` and related debugging code that should never have been in production
* Removed ```ResultVariable``` parameter help
* Improved error reporting
* Fixed ```Resource``` parameter documentation
* Imrpoved Example
* Removed dangling ```&``` from ```$Body``` creation

## Build Tools
### psake.ps1
* Block ```staging``` branch recommits so clean pull requests can be made
* Add ```!skiprecommit``` commit tag to block recommits

## Tests
### Get-AADGroupMember.Unit.Tests.ps1
* Created tests for Get-AADGroupMember

### Import-GraphApplication.Unit.Tests.ps1
* Created tests for Import-GraphApplication

### Import-GraphOauthAccessToken.Unit.Tests.ps1
* Created tests for Import-GraphOauthAccessToken

### Get-AADGroupById.Unit.Tests.ps1
* Created tests for Get-AADGroupById

### Get-AADGroupByDisplayName.Unit.Tests.ps1
* Created tests for Get-AADGroupByDisplayName

### Get-GraphOauthAccessToken.Unit.Tests.ps1
* Created tests for Get-GraphOauthAccessToken