
# Logseq

From their website:
> Logseq is a joyful, open-source outliner that works on top of local plain-text Markdown and Org-mode files. Use it to write, organize and share your thoughts, keep your to-do list, and build your own digital garden.

Logseq is the app that I use to write my notes. This repo contains almost all the scripts that I developed to make my life easier while using logseq.

## FAQ

#### What does the youtubeData script do?
- It simply parses the data from youtube using the Youtube Data API. It extracts metadata such as title, channel Name and Publish date. It then outputs the data in a nice format which youo can copy past into logseq.

#### Where to get the apiKey?
- You can get the api key from [Google Cloud Console](https://console.cloud.google.com "Google Cloud Console")
- From the navigation menu, go to **APIs and Services** > **Enabled APIs and Services**.
- Click on **ENABLE APIS AND SERVICES** at the top of the page.
- Search for **Youtube Data Api V3**.
- Click on **Enable**.
- Now again from the navigation menu, go to **APIs and Services** > **Credentials**.
- Click on **CREATE CREDENTIALS** at the top of the page and select Api key from the list.
- Configure the options and you should have the api key.
## Usage

#### youtubeData


| Parameter | Type     | Description                        |
| :-------- | :------- | :--------------------------------- |
| `url`     | `string` | **Required**. URL of youtube video |
| `apiKey`  | `string` | **Required**. Google api key       |

#### Command line

```bash
    chmod +x youtubeData.py
    ./youtubeData.py url apiKey
```


## Acknowledgements

 - [Florian Brucker](https://stackoverflow.com/a/50992575) For the module to make Ordinal number.
 - [Logseq](https://logseq.com/)


