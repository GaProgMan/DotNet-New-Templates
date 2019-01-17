# Podcast Templates - Newsletter

This templates is used to quickly generate an edition of the newsletter for [The .NET Core Podcast](https://dotnetcore.show/).

## Installation

This template can be used to generate an edition of The .NET Core Podcast newslettter with most of the formatting and standard information built up automaticallu.

To create a newsletter file, you will need to install the template. Do so by running the following command from within this directory:

`dotnet new --install ./`

You can confirm that the template is installed by running either of the following commmands:

- `dotnet new list`

This should list all of the installed templates and the following line should be found somewhere within that list:

``` shell
New .NET Core Show newsletter      newsletter          markdown
```

- `dotnet new newsletter --help`

This should list all of the cli switches that the new template supports, which should look similar to the following:

``` shell
New .NET Core Show newsletter
Author: Jamie Taylor
Description: Generates a markdown file to contain an edition of the newletter The .NET Core Podcast.
Options:
  -nt|--newsletter-title  The title of the newsletter
                          string - Optional
                          Default: NL_TITLE

  -en|--episode-number    The episode number
                          string - Optional
                          Default: EP_NUMBER

  -et|--episode-title     The title for the episode (minus the number), e.g. "Creating the .NET Core Podcast with Jamie Taylor"
                          string - Optional
                          Default: EP_TITLE

  -ept|--episode-topic    A brief synopsis of the episode - "In this episode of The .NET Core Podcast, we talk with the person about the thing"
                          string - Optional
                          Default: EP_SNIPPET

  -rd|--release-date      The planned release date for the episode (i.e. January 18, 2019)
                          string - Optional
                          Default: RELEASE_DATE
```

## Using the Template

Creating a new instance of a show notes file is a case of running the following command:

`dotnet new newsletter -en 99 -et "Creating the .NET Core Podcast with Jamie Taylor" -ept "talk with Jamie Taylor about creating the podcast" -rd "Grungltober 88th, 2255" -nt "Grungletober, 2255"`

This will create a file named `newsletter.md` with the following content:

``` markdown
# Grungletober, 2255

INTRO HERE

### Latest Episode

#### Episode 99 - Creating the .NET Core Podcast with Jamie Taylor

This episode will be published to [Patreon supporters](https://www.patreon.com/TheDotNetCorePodcast) a few days ahead of the "regular" RSS feed on Grungltober 88th, 2255.

In this episode of The .NET Core podcast we talk with Jamie Taylor about creating the podcast

On release day, you'll be able to check out the show notes at: [Episode 99 - Creating the .NET Core Podcast with Jamie Taylor](https://dotnetcore.show/episode-EPISODE_NO/)

### Subscribing To The Show

You can subscribe to the show in a number of ways, here are links to a number of podcasting services which have the show listed:

<a href="https://itunes.apple.com/gb/podcast/the-net-core-podcast/id1433496275" ><img alt="Subscribe to The .NET Core Podcast on Apple Podcasts" src="https://dotnetcore.show/content/images/Apple_Podcasts.png" style="width:300px;max-width:50%"/></a>
<a href="https://www.google.com/podcasts?feed=aHR0cHM6Ly90aGVkb3RuZXRjb3JlcG9kY2FzdC5saWJzeW4uY29tL3Jzcw%3D%3D" ><img alt="Subscribe to The .NET Core Podcast on Google Podcasts" src="https://dotnetcore.show/content/images/Google_Podcasts.png" style="width:300px;max-width:50%"/></a>
<a href="https://www.podchaser.com/TheDotNetCorePodcast?utm_source=The%20.NET%20Core%20Podcast%7C710798&utm_medium=badge&utm_content=TRCASP710798" target="__blank" style="text-decoration:none" ><img alt="Podchaser - The .NET Core Podcast" src="https://imagegen.podchaser.com/badge/TRCASP710798.png" style="width:300px;max-width:50%"/></a>

### Some Recent Discoveries in The Community

### Let's Connect

### Sponsoring The Show

Support for The .NET Core Podcast is provided, in part, by our Patreon supporters. To find out more about them, or to become a supporter of the show head over to our [Supporters](https://www.patreon.com/TheDotNetCorePodcast/). Did you know that Patreon supporters get early access to full versions of each episode?

We also have a [ko-fi page](https://ko-fi.com/jayandjaymedia). This is for listeners who may not want to support us on a monthly basis, but more of an ad-hoc one.

<a href="https://jayandjay.media/" target="__blank" style="text-decoration:none" ><img alt="Jay & Jay Media" src="https://dotnetcore.show/content/images/jayandjaymedia.png" style="width:300px;max-width:50%"/></a>

This edition of the mailing list is sponsored by [Jay & Jay Media](https://jayandjay.media/).

> Jay and Jay Media helps entreprenuers promote their brand so they can focus on building it

Would you like to sponsor the show? Then check out our [sponsor page](https://dotnetcore.show/sponsor/) for details on what we have on offer.
```