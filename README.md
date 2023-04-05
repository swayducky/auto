# SwayDucky's fork of Auto-GPT (Thing #21)
![GitHub Repo stars](https://img.shields.io/github/stars/swayducky/auto?style=social)
![Twitter Follow](https://img.shields.io/twitter/follow/swayducky?style=social)

Sway here. I forked [Auto-GPT](https://github.com/Torantulino/Auto-GPT) to see what I can learn.

Auto-GPT uses GPT-4 to autonomously search Google, discover information, and create content.

## Sway's notes to self

- Install requirements: `poetry add $( cat requirements.txt )`
- Configure Search API here: https://console.cloud.google.com/apis/api/customsearch.googleapis.com/metrics?project=flowhunt-1162
- Configure custom search engine: https://programmablesearchengine.google.com/controlpanel/overview?cx=b7c572c1419224b43
- Search Engine ID: b7c572c1419224b43

---

## 🔧 Usage

To run:
```
python scripts/main.py
```

Other ways of running:
```
python scripts/main.py --speak # with TTS (disabled in this forked repo)
python scripts/main.py --continuous # dangerous
```

## 🔍 Google API Keys Configuration

This section is optional, use the official google api if you are having issues with error 429 when running google search.
To use the `google_official_search` command, you need to set up your Google API keys in your environment variables.

1. Go to the [Google Cloud Console](https://console.cloud.google.com/).
2. If you don't already have an account, create one and log in.
3. Create a new project by clicking on the "Select a Project" dropdown at the top of the page and clicking "New Project". Give it a name and click "Create".
4. Go to the [APIs & Services Dashboard](https://console.cloud.google.com/apis/dashboard) and click "Enable APIs and Services". Search for "Custom Search API" and click on it, then click "Enable".
5. Go to the [Credentials](https://console.cloud.google.com/apis/credentials) page and click "Create Credentials". Choose "API Key".
6. Copy the API key and set it as an environment variable named `GOOGLE_API_KEY` on your machine. See setting up environment variables below.
7. Go to the [Custom Search Engine](https://cse.google.com/cse/all) page and click "Add".
8. Set up your search engine by following the prompts. You can choose to search the entire web or specific sites.
9.  Once you've created your search engine, click on "Control Panel" and then "Basics". Copy the "Search engine ID" and set it as an environment variable named `CUSTOM_SEARCH_ENGINE_ID` on your machine. See setting up environment variables below.


## Credits

- Follow me: https://twitter.com/swayducky
- Follow original author of Auto-GPT: https://twitter.com/siggravitas
