# Podcast Templates - Show Notes

This templates is used to quickly generate show notes for an episode of [The .NET Core Podcast](https://dotnetcore.show/).

## Installation

This template can be used to generate an almost empty show notes file for an episode of The .NET Core Podcast.

To create a show notes file, you will need to install the template. Do so by running the following command from within this directory:

`dotnet new --install ./`

You can confirm that the template is installed by running either of the following commmands:

- `dotnet new list`

This should list all of the installed templates and the following line should be found somewhere within that list:

``` shell
New .NET Core Show podcast episode show notes      podcast         markdown
```

- `dotnet new podcast --help`

This should list all of the cli switches that the new template supports, which should look similar to the following:

``` shell
New .NET Core Show podcast episode show notes
Author: Jamie Taylor
Description: Generates a markdown file to contain the show notes for The .NET Core Podcast.
Options:
  -en|--episode-number   The episode number
                         string - Optional
                         Default: EP_NUMBER

  -et|--episode-title    The title for the episode
                         string - Optional
                         Default: TITLE

  -ii|--is-interview     Whether this is an interview episode or not (monologue if false)
                         bool - Optional
                         Default: false / (*) true

  -pn|--persons-name     The name of the person being interviewed (optional)
                         string - Optional
                         Default: PERSONS_NAME

  -pt|--persons-twitter  The twitter handle (@) of the person being interviewed (optional)
                         string - Optional
                         Default: PERSONS_TWITTER


* Indicates the value used if the switch is provided without a value.
```

## Using the Template

Creating a new instance of a show notes file is a case of running the following command:

`dotnet new podcast -ii true -pn "Jamie Taylor" -en 0 -et "Jamie's New Podcast" -pt "dotnetcoreblog"`

This will create a file named `episode.md` with the following content:

``` markdown
### Embedded Player

### Episode Transcription

Hello everyone and welcome to THE .NET Core podcast - the only podcast which is devoted to:

- .NET Core
- ASP.NET Core
- EF Core
- SignalR

and not forgetting The .NET Core community, itself.

I am your host, Jamie "GaProgMan" Taylor, and this is episode 0: Jamie's New Podcast with Jamie Taylor. In this episode I interviewed Jamie Taylor about (Person's niche). Some of you may know Jamie Taylor from (Places that the Person has worked or contributed towards the community).

So lets site back, open up a terminal, type in `dotnet new podcast` and let the show begin.

### Jamie Taylor Introduction

### Wrapping Up

That was my interview with Jamie Taylor of (Company Name). Be sure to check out the show notes for a bunch of links to some of the stuff that we covered, and a collection of text snippets from the interview. The show notes, as always, can be found at [dotnetcore.show](https://dotnetcore.show/).

And don't forget to spread the word, leave me a rating or review on your podcatcher of choice, and to come back next time for more .NET Core goodness.

I will see you again real soon. See you later folks.

### Useful Links

- [YouTube version of this episode](https://www.youtube.com/watch?v=)
  - The YouTube version of this episode, if you'd prefer to listen there
- [Jamie Taylor on twitter](https://twitter.com/dotnetcoreblog)
```