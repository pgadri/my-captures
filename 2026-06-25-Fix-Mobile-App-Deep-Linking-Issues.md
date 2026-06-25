# Fix Mobile App Deep Linking Issues
**Source:** https://www.facebook.com/share/v/17g75Me99S/?mibextid=wwXIfr
**Creator:** The Faction Group LLC
**Captured:** June 25, 2026

---

## Key Insights

• Apple Universal Links require an apple-app-site-association file on your domain
• Android app links need a digital assets link JSON file and intent filters
• Expo Linking Package handles Android app links configuration
• Expo Router handles fallback to website with app install prompt
• Universal links increase mobile web to app conversions

---

## Full Transcript

 Your mobile app exists, but when someone shares a link to your content, it opens in the browser, not the app like it was supposed to. The user hits a login wall, gets confused, and leaves. You lost them because of a missing configuration file. Here are the three things you can do right now to fix it. Number one, configure Apple Universal Links. Go create an apple.app site association file in your domain. Hosted at yourdomain.com This is a JSON file that tells iOS which URL pass should open your app. No redirects. The link opens directly in your app every time. Apple verifies this file when the user installs your app. Step 2. Configure Android app links. Similarly, create a digital assets link file. Hosted at yourdomain.com again. This JSON file tells Android which URLs open your app. Add intent filters to your Android manifest. Expo handles this with Expo Linking Package. Same URLs work on both platforms. Step 3. Handle the fallback. Not every user has your app installed on their phone. If the app is not installed, the link should go straight to your website. Your website shows the content plus a smart banner promoting the app install. Expo Router handles this with a single configuration. One URL, app installed, opens in app, not installed, opens in website with install prompt. Universal links convert mobile web visitors into app users. Without them, every shared link is a dead end. Do you have any deep linking setups? What tripped you up? Tell me about it.
