# Concentric - Watch Face

<img src='https://play-lh.googleusercontent.com/Qp-fN1rU6bimstpohGY03DlDPMRdYapLK0CXH-utB6HJQhtCLxBERs47vjFP4rvVU-w=w832-h470' style="width:600px;" ></img>

<a href='https://play.google.com/store/apps/details?id=com.watchfacedesigns.Concentric&utm_source=https%3A%2F%2Fgithub.com%2Flukakilic%2Fconcentric-watch-face%2Ftree%2Fmain&pcampaignid=pcampaignidMKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1' style="display:inline-block"><img alt='Get it on Google Play' src='https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png' style="width:200px;"/></a>

The Concentric design is originally from the Google Pixel Watch (1). This project recreates it using [Watch Face Format](https://developer.android.com/training/wearables/wff). 

## Modify the Watch Face

The XML code can be found in the `res/raw` folder. Watch Face Format is well [documented](https://developer.android.com/training/wearables/wff/watch-face) in case you wish to modify the watch face.


## Build the Watch Face

> Google has transitioned to Gradle for compiling watch faces, but I still use the original build script provided when WFF first launched. For reference on building a watch face, see [wear-os-samples/WatchFaceFormat](https://github.com/android/wear-os-samples/tree/main/WatchFaceFormat).

To streamline the process, I’ve developed a small CLI tool that integrates this script, removing the need for Gradle. Once it's ready, I plan to publish it on GitHub.
