#Requirements Specification

1. [Introduction] (#introduction)
  1. Purpose
  2. Scope
  3. References

2. [Description] (#description)
  1. Product perspective
  2. Product functions
  3. User characteristcs
  4. Constraints

3. [Specific Requirements] (#specific-requirements)
  1. External interface requirements
    1. User interfaces
    2. Hardware interfaces
    3. Communications interfaces
  2. System Features
    1. System feature
      1. Introduction / Purpose of feature
      2. Stimulus / Response sequence
      3. Associated functional requirements
  3. [Perfomance Requirements] (#perfomance-requirements)
  4. [Design Constraints] (#design-constraints)

## Introduction
DuckieTV was originally developed as a private project so [SchizoDuckie](https://github.com/SchizoDuckie) could learn AngularJS. Nowadays this project is used to organize and catalogue all the TV shows and movies that the user wants to watch in a calendar. It may also be used to download said movies by searching for torrents on multiple external websites.

No acronyms or abbreviation were used in the project.

The author states that DuckieTV,

> is built with Angular.js and Bootstrap.css. On top of that, [some] libraries are used.

## Description
As [DuckieTV](http://duckie.tv/) describes,

> DuckieTV is an application that takes care of TV-Show addicts by providing a personalized TV-Show calendar.

This tool may be integrated directly with local Torrent clients such as Deluge, uTorrent, qBittorrent, Tixati, Transmission and Vuze. This allows the user to keep an eye on the download progress of its torrents without switching to another application.

Another feature that is widely used by its users is the ability to automatically download shows that they have enjoyed as soon as they air and become available on any of the torrent sites supported.

Additionally the program is available in 14 different languages.

![Calendar](http://schizoduckie.github.io/DuckieTV/img/screenshots/full/calendar.jpg)
![Main Page](http://schizoduckie.github.io/DuckieTV/img/screenshots/full/trending.jpg)

The target market is composed by TV-Show addicts and can be separated into two distinct types of use.
- Users that just want to keep track of when their favorite TV shows are airing, regardless of network or country. It doesn't matter if a show airs on BBC2, or is a Netflix or Amazon or HBO exclusive, the user can put it on their personal TV calendar regardless of the user's home country. 
- Users that prefer to see TV Shows at home without being locked out by regional copyright and release-schedule restrictions, or don't want to subscribe to different on-demand TV providers to see their favorite shows.

- Previously there was no software that allowed users to organize their favorite shows and downloads in a calendar like DuckieTV does.

There are currently no constraints on using this program, except for countries where the program might be illegal because it uses torrents.

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
DuckieTV runs on all chromium browsers and any modern Operating System, requiring only that the user has internet access. It does not use custom server-side code but runs completely on the clientside. Some resources are cached on GitHub's infrastructure though.

DuckieTV itself uses only HTTP to communicate with external resources. Having said that, It can interface with the BitTorrent protocol if the user installs any of the supported third-party Torrent Clients via their Web API's. Other API's such as [Open Subtitles](http://api.opensubtitles.org), [TrackTV](https://api-v2launch.trakt.tv/), [IMDB](http://www.imdb.com/) and [Torrent Search Engines](https://github.com/SchizoDuckie/DuckieTV/tree/angular/js/services/TorrentSearchEngines) all run on HTTP.

### System Features
* Chrome

[DuckieTV](http://duckie.tv/) is a huge fan of Chrome, so DuckieTV can be installed as an extension for this same browser without the need of a standalone version. An **online demo** is available [here](http://duckietv.github.io/DuckieTV/)

* Calendar

The calendar is used to schedule TV-Shows and movies download. In order to be used, the client just has to have either or a browser like [Chrome](https://www.google.pt/chrome/browser/desktop/) and install the extension or download the standalone version for their platform. In both cases it also requires an Internet connection to populate the calendar, after that the program can run without an internet connection (but then it will not fetch updates, obviously).

* Proxy

It is possible to bypass Internet Service Providers (ISP) torrent censorship with DuckieTV. It works by finding mirrors for the target websites that are not currently blocked by them.

* Privacy

Because there is no server side data storage, the user's privacy is kept intact.

> The only statistics tracked for DuckieTV are the visits to the public GitHub site (by Google Analytics) and the installations in the Chrome Webstore.

> As soon you install DuckieTV it runs locally without sending statistics anywhere. There is no server to connect to, no infrastructure to bring down, and no logging from DuckieTV’s side of anything you do within the app, and there never will be.

> Everything runs locally. If you decide to execute a torrent search for an episode, a request goes from your computer to the search engine.

#### Use Case Diagram
![Use Case](http://i.imgur.com/s6eBXHM.png)

## Perfomance Requirements

## Design Constraints
DuckieTV was developed in order to fit different screen dimensions. While it can technically run on a (high-end) Android phone, however, the use of a Tablet is advised when you want to run it on the Android platform because there are no small-screen optimisations.

Since it is a JavaScript application, its design is only limited by modern CSS's limitations.

### Authors
* João Silva ([up201305892@fe.up.pt](mailto:up201305892@fe.up.pt))
* Luís Figueiredo ([up201304295@fe.up.pt](mailto:up201304295@fe.up.pt))
* Pedro Teles ([up201305101@fe.up.pt](mailto:up201305101@fe.up.pt))
* Tiago Figueiredo ([ei12069@fe.up.pt](mailto:ei12069@fe.up.pt))

**Faculdade de Engenharia da Universidade do Porto - MIEIC**
**2015-10-16**
