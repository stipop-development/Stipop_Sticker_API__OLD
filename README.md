
<h1 align="center">
  <br>
  <img src="https://cdn3.imggmi.com/uploads/2019/9/25/342c9fcf023615025e4f760006661a63-full.png" alt="Markdownify" width="200"></a>
  <br>
  Stipop
  <br>
</h1>

<h4 align="center">A minimal Markdown Editor desktop app built on top of <a href="http://electron.atom.io" target="_blank">Electron</a>.</h4>

<p align="center">
  <a href="https://badge.fury.io/js/electron-markdownify">
    <img src="https://badge.fury.io/js/electron-markdownify.svg"
         alt="Gitter">
  </a>
  <a href="https://gitter.im/amitmerchant1990/electron-markdownify"><img src="https://badges.gitter.im/amitmerchant1990/electron-markdownify.svg"></a>
  <a href="https://saythanks.io/to/amitmerchant1990">
      <img src="https://img.shields.io/badge/SayThanks.io-%E2%98%BC-1EAEDB.svg">
  </a>
  <a href="https://www.paypal.me/AmitMerchant">
    <img src="https://img.shields.io/badge/$-donate-ff69b4.svg?maxAge=2592000&amp;style=flat">
  </a>
</p>

<p align="center">
  <a href="#key-features">Key Features</a> •
  <a href="#how-to-use">How To Use</a> •
  <a href="#download">Download</a> •
  <a href="#credits">Credits</a> •
  <a href="#related">Related</a> •
  <a href="#license">License</a>
</p>

![screenshot](https://raw.githubusercontent.com/amitmerchant1990/electron-markdownify/master/app/img/markdownify.gif)



**Stipop Sticker API**
----

![Works with Android](https://img.shields.io/badge/Works_with-Android-green?style=flat-square)
![Works with iOS](https://img.shields.io/badge/Works_with-iOS-blue?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues/stipop-development/Stipop_Sticker_API?style=flat-square)

> Stipop provides a powerful and flexible sticker API that enables companies to add stickers onto their apps and websites with minimum effort and maximum effect.

Sticker is one of the most powerful visual contents you can find in the digital world. With more than 50 billion being sent everyday, it brings emotion into online communicaton. Unlike GIFs, because it has specific artist who created it with a purpose (for online communication, character etc.) it's very unique and usable. 

Seeing that sticker is a useful media, we as a team started a platform, where stickers and sticker lovers can play about. Our product began as an app for messenger users to download stickers for their personal use. Now that there is more than 2,000 sticker artists participating from 20 different countries and the total sticker accumulate to 100,000 we thought it best that other companies should be able to provide stickers to their own users.

<_Additional information about your API call. Try to use verbs that match both request type (fetching vs modifying) and plurality (one vs multiple)._>

## Get started :rocket:

To get started, review the 'README' files in the [Stipop_Sticker_API](https://github.com/stipop-development/Stipop_Sticker_API) repository.

## Announcements :loudspeaker:
Please check out [Annoucements](https://github.com/stipop-development/Stipop_Sticker_API/wiki/Announcements) for recent changes.

## Opening Issues :warning:

> Only use the GitHub Issues section if you discovered **issues with the code itself**. Do not mistake the Issues page as a help desk. You can ask for help at [Stack Overflow](https://stackoverflow.com/).  
> For support, please contact <webmaster@stipop.io>.

- Create a [**general issue**](https://github.com/stipop-development/Stipop_Sticker_API/issues/new?template=general.md)

## Opening Pull Requests

> In order for us to accept pull requests, please complete the Contributor License Agreement by following instructions in [`CONTRIBUTING`](https://github.com/stipop-development/Stipop_Sticker_API/blob/master/CONTRIBUTING.md).

1. Please check that a similar pull request doesn't exist already [here](https://github.com/stipop-development/Stipop_Sticker_API/pulls)
2. [Open a new pull request](https://github.com/stipop-development/Stipop_Sticker_API/compare)
3. Wait for someone to look at it :watch:

## License

Stipop Sticker API is MIT licensed, as found in the [`LICENSE`](https://github.com/stipop-development/Stipop_Sticker_API/blob/master/LICENSE) file.

## API

* **URL**

  <_The URL Structure (path only, no root url)_>

* **Method:**
  
  <_The request type_>

  `GET` | `POST` | `DELETE` | `PUT`
  
*  **URL Params**

   <_If URL params exist, specify them in accordance with name mentioned in URL section. Separate into optional and required. Document data constraints._> 

   **Required:**
 
   `id=[integer]`

   **Optional:**
 
   `photo_id=[alphanumeric]`

* **Data Params**

  <_If making a post request, what should the body payload look like? URL Params rules apply here too._>

* **Success Response:**
  
  <_What should the status code be on success and is there any returned data? This is useful when people need to to know what their callbacks should expect!_>

  * **Code:** 200 <br />
    **Content:** `{ id : 12 }`
 
* **Error Response:**

  <_Most endpoints will have many ways they can fail. From unauthorized access, to wrongful parameters etc. All of those should be liste d here. It might seem repetitive, but it helps prevent assumptions from being made where they should be._>

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "Log in" }`

  OR

  * **Code:** 422 UNPROCESSABLE ENTRY <br />
    **Content:** `{ error : "Email Invalid" }`

* **Sample Call:**

  <_Just a sample call to your endpoint in a runnable format ($.ajax call or a curl request) - this makes life easier and more predictable._> 

* **Notes:**

  <_This is where all uncertainties, commentary, discussion etc. can go. I recommend timestamping and identifying oneself when leaving comments here._> 
