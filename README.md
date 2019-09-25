<h1 align="center">
  <br>
  <img src="https://cdn3.imggmi.com/uploads/2019/9/25/342c9fcf023615025e4f760006661a63-full.png" alt="Markdownify" width="200"></a>
  <br>
  Stipop
  <br>
</h1>


<h4 align="center">Propel user engagement, retention, and conversion with stipop sticker API</h4>

<p align="center">
  <a href="#Intro">Intro</a> •
  <a href="#Key-Features">Key Features</a> •
  <a href="#get-started-rocket">Get Started</a> •
  <a href="#1-sticker-pack-api-default-best-100">Pack API</a> •
  <a href="#2-sticker-id-api">ID API</a> •
  <a href="#announcements-loudspeaker">Announcements</a> •
  <a href="#opening-issues-warning">Issues</a> •
  <a href="#opening-pull-requests">Pull</a> •
  <a href="#license">License</a>
</p>





## Intro

![Works with Android](https://img.shields.io/badge/Works_with-Android-green?style=flat-square)
![Works with iOS](https://img.shields.io/badge/Works_with-iOS-blue?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues/stipop-development/Stipop_Sticker_API?style=flat-square)

> Stipop provides a powerful and flexible sticker API that enables companies to add stickers onto their apps and websites with minimum effort and maximum effect.

Sticker is one of the most powerful visual contents you can find in the digital world. With more than 50 billion being sent everyday, it brings emotion into online communicaton. Unlike GIFs, because it has specific artist who created it with a purpose (for online communication, character etc.) it's very unique and usable. 

Seeing that sticker is a useful media, we as a team started a platform, where stickers and sticker lovers can play about. Our product began as an app for messenger users to download stickers for their personal use. Now that there is more than 2,000 sticker artists participating from 20 different countries and the total sticker accumulate to 100,000 we thought it best that other companies should be able to provide stickers to their own users.


## Key Features
* Sticker Package
  - 100,000 stickers uploaded by 2,000 artists from 20 different countries.
  - Every sticker has been through the approval process where stipop App users decide.
* Multi-language Contents
  - English/Spanish/Korean
* Regional Best
  - Top 100 download list provided in specified langauge speaking countries
* Daily Update
  - All sticker list updated in a daily basis with new stickers added in automatically
* Favorites (preparing)
  - API to provide list of stickers used the most by a specific end user


## Get started :rocket:

To get started, review sections below in the 'README' files in the [Stipop_Sticker_API](https://github.com/stipop-development/Stipop_Sticker_API) repository.



## 1) Sticker-Pack API (default: Best 100)

* **URL**

  /v1/package/best/:languageCode

* **Method:**

  `GET`
  
*  **Request Headers**

   **Required:**
 
   `apikey=[string]` Issued apikey value


* **Request Parameters**

  `languageCode=[string]` all:Common, en:English, es:Spanish, ko:Korean

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** <br />
    ```json
    {
      "status": "success",
      "code": "0000",
      "packages": [
      {
          "packageId": 0,
          "packageName": "sticker 1",
          "mainImgUrl": "https://....Z41sOfn7Z.png",
          "keywords": "keyword1, keyword2",
          "language": "korean",
          "animatedYn": "N"
      },
      {
          "packageId": 1,
          "packageName": "sticker 2",
          "mainImgUrl": "https://....eNSPZR3r2D.png",
          "keywords": "keyword1, keyword2",
          "language": "Spanish",
          "animatedYn": "N"
      }]
    }
    ```
 
* **Error Response:**

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** 
    ```json
    {
      "status": "fail",
      "message": "non exist apikey",
      "code": "9000"
    }
    ```
    OR

  * **Code:** 500 Internal Server error <br />
    **Content:** 
    ```json
    {
       "status" : "fail", 
       "message": "server error", 
       "code":"9010"
    }
    ```

* **Sample Call:**

  ```curl
  curl --location --request GET "https://bapi.stipop.io/v1/packages/best" \ --header "apikey: {YOUR_API_KEY}"
  ```

* **Notes:**

## 2) Sticker-ID API

* **URL**

  /v1/package/:packageId

* **Method:**

  `GET`
  
*  **Request Headers**

   **Required:**
 
   `apikey=[string]` Issued apikey value


* **Request Parameters**

  **Required:**
  `packageId=[integer]`

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** <br />
    ```json
    {
        "status": "success",
        "code": "0000",
        "stickers": [
        {
            "packageId": 1,
            "stickerId": 790,
            "stickerImgUrl": "https://...img1.png"
        },
        {
            "packageId": 1,
            "stickerId": 791,
            "stickerImgUrl": "https://...img2.png"
        }]
    }
    ```
 
* **Error Response:**

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** 
    ```json
    {
      "status": "fail",
      "message": "non exist apikey",
      "code": "9000"
    }
    ```
    OR

  * **Code:** 500 Internal Server error <br />
    **Content:** 
    ```json
    {
       "status" : "fail", 
       "message": "server error", 
       "code":"9010"
    }
    ```

* **Sample Call:**

  ```curl
  curl --location --request GET "https://bapi.stipop.io/v1/packages/{pakcageId}" \ --header "apikey: {YOUR_API_KEY}"
  ```

* **Notes:**

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
