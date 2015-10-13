#Requirements Specification

1. Introduction
  1. Purpose
  2. Scope
  3. Definitions
  4. Acronyms
  5. Abbreviations
  6. References
  7. Overview

2. Description
  1. Product perspective
  2. Product functions
  3. User characteristcs
  4. Constraints
  5. Assumptions and dependencies

3. Specific requirements
  1. External interface requirements
    1. User interfaces
    2. Hardware interfaces
    3. Communications interfaces
  2. System features
    1. System feature
      1. Introduction / Purpose of feature
      2. Stimulus / Response sequence
      3. Associated functional requirements
  3. Perfomance requirements
  4. Design constraints
  5. Software system attributes
  6. Other requirements

## Introduction
DuckieTV was originially developed as a private project so [SchizoDuckie](https://github.com/SchizoDuckie) could learn AngularJS. Nowadays this project is used to organize and catalogue all the TV shows and movies that the user wants to watch in a calendar. It may also be used to download said movies by indexing torrents from multiple websites.

No acronyms or abbreviation were used in the project.

The author states that [DuckieTV](http://schizoduckie.github.io/DuckieTV/?from=duckie.tv/),

> is build with Angular.js and Bootstrap.css. On top of that, [some] libraries are used.

## Description
As we can state from *DuckieTV*,

> DuckieTV is an application that takes care of TV-Show addicts by providing a personalized TV-Show calendar.

This tool may be integrated directly to local Torrent clients such as Deluge, uTorrent, qBittorrent, Tixati, Transmission and Vuze. This allows the user to keep an eye on the download progress of its torrents without switching to another application.

Another feature that is widely used by its users is the ability to automatically download shows that they have enjoyed as soon as they air.

Additionally the program is available in 14 different languages.

![Calendar](http://schizoduckie.github.io/DuckieTV/img/screenshots/full/calendar.jpg)
![Main Page](http://schizoduckie.github.io/DuckieTV/img/screenshots/full/trending.jpg)

The target market is composed by TV-Show addicts that prefer to see movies at home over buying expensive tickets in a cinema. Previously there was no software that allowed users to organize their favorite shows and downloads in a calendar like DuckieTV does.

There are currently no constraints on using this program, except for North Korea where the program is illegal.

Some libraries are being used in the development.
- CreateReadUpdateDelete.js - [Javascript Sqlite ORM](https://github.com/SchizoDuckie/CreateReadUpdateDelete.js/)
- Dialogs.js - [Modal dialogs for Angular.js](https://github.com/m-e-conroy/angular-dialog-service)
- UI-Bootstrap.js - [Bootstrap enhancements for angular.js](https://angular-ui.github.io/bootstrap/)
- Datepicker.js - [Somewhat modified, the basis for the calendar](https://github.com/g00fy-/angular-datepicker)
- angular-translate - [i18n translations](https://angular-translate.github.io)
- angular-translate-once - [translation one time bindings](https://github.com/ajwhite/angular-translate-once)
- angular-formly - [form presentation](https://github.com/formly-js/angular-formly)
- tmhDynamicLocale - [locale management](https://github.com/lgalfaso/angular-dynamic-locale)
- moment - [Parse, validate, manipulate, and display dates](https://momentjs.com)
- moment-timezone - [timezone support](https://github.com/moment/moment-timezone)
- AngularJS-Toaster - [customized version of "toastr" non-blocking notification library](https://github.com/jirikavi/AngularJS-Toaster)
- UI-router Extras - [enhancements for UI-Router](https://christopherthielen.github.io/ui-router-extras)
- angular-dialgauge - [dial gauge directive](https://cdjackson.github.io/angular-dialgauge/)

## Specific Requirements

DuckieTV runs on any browser and any modern Operating System, requiring only that the user has internet access. 
