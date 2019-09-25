**Stipop Sticker API**
----

![Works with Android](https://img.shields.io/badge/Works_with-Android-green?style=flat-square)
![Works with iOS](https://img.shields.io/badge/Works_with-iOS-blue?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues/stipop-development/Stipop_Sticker_API?style=flat-square)

> Stipop provides a powerful and flexible sticker API that enables companies to add stickers onto their apps and websites with minimum effort and maximum effect.

Sticker is one of the most powerful visual contents you can find in the digital world. With more than 50 billion being sent everyday, it brings emotion into online communicaton. Unlike GIFs, because it has specific artist who created it with a purpose (for online communication, character etc.) it's very unique and usable. 

Seeing that sticker is a useful media, we as a team started a platform, where stickers and sticker lovers can play about. Our product began as an app for messenger users to download stickers for their personal use. Now that there is more than 2,000 sticker artists participating from 20 different countries and the total sticker accumulate to 100,000 we thought it best that other companies should be able to provide stickers to their own users.

<_Additional information about your API call. Try to use verbs that match both request type (fetching vs modifying) and plurality (one vs multiple)._>

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
