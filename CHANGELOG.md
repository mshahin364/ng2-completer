# Change Log
All notable changes to this project will be documented in this file.

## 1.2.0 (2017-02-26)

### Implemented enhancements
- Replaced the source URL of remote formatter because of Google API limits
- Replace `dataService` with `datasource` and accept Array or URL string as input for `datasource`. Note: `dataService` will be depreacated in future releases

### Fixed bugs
- Since last commit searchFields does not behave as stated in the docs #144
- Fixed ionic build
- Fix material design demo
- Fix demo of remote URL formatter

## 1.1.0 (2017-02-10)

### Implemented enhancements
- searchFields and titleField are mandatory #100

### Fixed bugs
- (selected) not called when text is highlighted and then deleted #121
- Clicking in a pre-filled ng2-completer with [overrideSuggested]="true", then immediately clicking another element clears the ngModel to a blank string #122
- required not working when intializing ngModel with a value #126
- First item is selected on enter #134

## 1.0.0 (2017-01-21)

### Implemented enhancements
- Input box doesn't have a type! #73
- new ctr-input property 'fillHighlighted' that controls setting of input value when item is highlighted #123 (by @mdudek)
- Cannot access entered text when not selected from list #72
- ng2-completer input autofocus? #125
- Set `max-height` of dropdown in demo

### Fixed bugs
- ngModelChange doesn't work #97
- Material design dropdown pushes everything down #115

### Breaking changes
- NgModel now reflects the vlue of the input. to get only selected values use `selected` event

## 0.4.0
### Implemented enhancements
- reorder of the folder structure
- Apply class to child input for styling purposes #40
- Annoying flickering when clearing data #82
- Open dropdown programmatically. #84

### Fixed bugs
- Problem with OnPush change detection strategy #69
- AutoMatch doesn't remove binded value if nothing match (angucomplete-alt does) #101

## 0.3.3
### Fixed bugs
- Why version 0.3.2 requires @angular/*@2.2.4? #103
- Build with @angular version 2.3.1 to fix issue with metadata version

## 0.3.2
### Fixed bugs
- Form is submitted when we select an option from dropdown using enter key #52

## 0.3.0
### Implemented enhancements
- Change deployment method now using ngc and rollup for the package and webpack for dev and demo
- AOT support #60

### Fixed bugs
- TS5023 Build:Unknown compiler option 'forceConsistentCasingInFileName' #74
- .completer-selected-row is missing in the description #78
- originalObject is null for CompleterService in version 0.2.3 #81

## 0.2.3
### Implemented enhancements
- Clear selection when search changes #45

### Fixed bugs:
- fix for overrideSuggested

## 0.2.2 
### Implemented enhancements
- Added support for async local data

### Fixed bugs
- Not able to capture blur event #50
- textSearching not display in first search #55

## 0.2.1 (2016-10-05)
### Implemented enhancements
- Added material2 component to demo

### Fixed bugs
- Mouse click doesn't select the item, Enter Key does! #46


## 0.2.0 (2016-10-04)
This is a rewrite of the completer component using directives that implement most of the functionality.
### Implemented enhancements
- Support for custom HTML and CSS #13 #21

### Fixed bugs
- Bump version dependency to angular 2.0.0 #39