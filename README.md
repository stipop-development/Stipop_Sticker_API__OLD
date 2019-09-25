
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
  <a href="#how-to-use">How To Use</a> •
  <a href="#download">Download</a> •
  <a href="#credits">Credits</a> •
  <a href="#related">Related</a> •
  <a href="#license">License</a>
</p>

![screenshot](https://raw.githubusercontent.com/amitmerchant1990/electron-markdownify/master/app/img/markdownify.gif)



## Intro

![Works with Android](https://img.shields.io/badge/Works_with-Android-green?style=flat-square)
![Works with iOS](https://img.shields.io/badge/Works_with-iOS-blue?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues/stipop-development/Stipop_Sticker_API?style=flat-square)

> Stipop provides a powerful and flexible sticker API that enables companies to add stickers onto their apps and websites with minimum effort and maximum effect.

Sticker is one of the most powerful visual contents you can find in the digital world. With more than 50 billion being sent everyday, it brings emotion into online communicaton. Unlike GIFs, because it has specific artist who created it with a purpose (for online communication, character etc.) it's very unique and usable. 

Seeing that sticker is a useful media, we as a team started a platform, where stickers and sticker lovers can play about. Our product began as an app for messenger users to download stickers for their personal use. Now that there is more than 2,000 sticker artists participating from 20 different countries and the total sticker accumulate to 100,000 we thought it best that other companies should be able to provide stickers to their own users.

<_Additional information about your API call. Try to use verbs that match both request type (fetching vs modifying) and plurality (one vs multiple)._>

## Get started :rocket:

To get started, review the 'README' files in the [Stipop_Sticker_API](https://github.com/stipop-development/Stipop_Sticker_API) repository.



## 1) Best Sticker top 100 Api

* **URL**

  /v1/package/best

* **Method:**

  `GET`
  
*  **Request Headers**

   **Required:**
 
   `apikey=[string]` 발급받은 apikey 값


* **Request Parameters**

  `none`

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** <br />
    `{
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
        },
        .......
        ]`
 
* **Error Response:**

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** 
    `{
    "status": "fail",
    "message": "non exist apikey",
    "code": "9000"
}`

  OR

  * **Code:** 500 Internal Server error <br />
    **Content:** `{"status" : "fail", "message": 'server error', code:"9010"}`

* **Sample Call:**

  `curl --location --request GET "https://bapi.stipop.io/v1/packages/best" \ --header "apikey: {YOUR_API_KEY}"`

* **Notes:**

## 2) 패키지 상세조회 Api

* **URL**

  /v1/package/:packageId

* **Method:**

  `GET`
  
*  **Request Headers**

   **Required:**
 
   `apikey=[string]` 발급받은 apikey 값


* **Request Parameters**

  **Required:**
  `packageId=[integer]`

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** <br />
    `{
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
        },
        .......
        ]`
 
* **Error Response:**

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** 
    `{
    "status": "fail",
    "message": "non exist apikey",
    "code": "9000"
}`

  OR

  * **Code:** 500 Internal Server error <br />
    **Content:** `{"status" : "fail", "message": 'server error', code:"9010"}`

* **Sample Call:**

  `curl --location --request GET "https://bapi.stipop.io/v1/packages/{pakcageId}" \ --header "apikey: {YOUR_API_KEY}"`

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
