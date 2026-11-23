# Optional: connect your own Google Search Console

This is free, and it is the one source of real, measured search data you can wire up yourself, because it is your own data straight from Google. It is optional. The skill works without it.

When connected, keyword research can use your actual queries, impressions, clicks and average positions, which makes the scoring and the quick-win list much sharper.

This uses YOUR Google Cloud OAuth app and YOUR credentials. Nothing goes to The SEO Agent.

## One-time setup

1. **Create a Google Cloud project** at https://console.cloud.google.com and enable the **Search Console API**.
2. **Create an OAuth 2.0 Client ID** (type: Desktop app). Note the client ID and client secret.
3. **Authorize the `webmasters.readonly` scope** and complete the consent flow once to get a **refresh token**. (Google's OAuth Playground at https://developers.google.com/oauthplayground can mint a refresh token against your own client ID and secret.)
4. **Put the values in a `.env` file** in your project folder, and keep that file out of git:
   ```
   GSC_CLIENT_ID=...
   GSC_CLIENT_SECRET=...
   GSC_REFRESH_TOKEN=...
   GSC_PROPERTY_URL=https://your-verified-property.com/
   ```

## What the agent does with it

When these are set, the agent will:

- Refresh an access token from your refresh token (the access token is short-lived; the refresh token is long-lived, so keep it private).
- Call the Search Analytics API for the last 28 days, grouped by query.
- Surface your top queries and your **quick wins**: queries where you already sit at positions 5 to 20, where one better article may move you up.

## Security notes

- Your refresh token is a long-lived secret. Keep `.env` out of git and never paste it into a chat or a shared file.
- The scope is read-only (`webmasters.readonly`). The agent cannot change anything in your Search Console.
