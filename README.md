# Customizable web browser home screen

Customize your home screen in all browsers with a single file.

![imagen demo](/assets/demo.png)

When you open the page for the first time in the day, the system automatically loads a wallpaper <b>ONCE A DAY</b> from the [Unsplash](https://unsplash.com/) API.
The wallpaper url is saved in localStorage on your browser for next open and wallpaper upgrade is in the nex day.

## Requirements

- Unsplash account
- Any web browser

## Get Unsplash api credentials

You need the `apikey` and `topic_id` for load background wallpapers on the page.

|||
|-|-|
| APIKEY_UNSPLASH | Create app in Unsplash [here](https://unsplash.com/oauth/applications),after, open the app and scroll down to seccion `Keys` and copy `Access Key`.|
| TOPIC_UNSPLASH | For the topic id, go to [here](https://unsplash.com/t/) after you selected any, you watch the URL and copy the tag mark. |

![How to get topic id image](/assets/topics-unsplash.png)

## Installation

- Clone repository with `git clone git@github.com:Leonardo-Henao/BrowserHomeScreen.git` for SSH or `git clone https://github.com/Leonardo-Henao/BrowserHomeScreen.git` for HTTPS
- Open in your browser `file:///[FOLDER_PATH]/BrowserHomeScreen/index.html?unsplash_key=[APIKEY_UNSPLASH]&unsplash_topic=[TOPIC_UNSPLASH]`

## Browser settings

In your browser, go to the section settings and customize:

<b>Chrome</b>
|Section| Configuration |
|-|-|
| On startup | Set a specific page and paste the page that you open in browser. |
| Appearance | Enable `Show home button` and set page, paste the page that you open in browser. |

## Home screen settings

Open in your code editor, and go to script with following comment `// Script for configurations`

### Configure Google, Bing or Duckduckgo

| Variable name| Value |
|-|-|
| `useSearcher` | 1 : Google <br> 2 : Bing <br> 3 : Duckduckgo |

### Bookmarks

| Variable name| Value |
|-|-|
| `bookmarks` | `[{ name: 'NAME BOOKMARK', url: 'URL', img: getIconWebPage('URL_BOOKMARK'), }, ...]` |

The bookmarks variable requires a `json` element with the following keys:

- `name`: Any string
- `url`: Any url string
- `img`: you can use the function `getIconWebPage('URL_BOOKMARK')` or set you icon or image with an absolute path.

<br>
<br>
<hr>
<br>

<div align="center">

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)


</div>
