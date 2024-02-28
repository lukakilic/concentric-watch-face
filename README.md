# Concentric - Watch Face

<img src='https://play-lh.googleusercontent.com/yACgfLN9DZreXxiaCrfSL8wiFk0eSNa7ScC3n5vRK5ZUh0Fe2d8NlQUtB4Fb7T53bQw=w832-h470' style="width:600px;" ></img>

<a href='https://play.google.com/store/apps/details?id=com.watchfacedesigns.Concentric&utm_source=https%3A%2F%2Fgithub.com%2Flukakilic%2Fconcentric-watch-face%2Ftree%2Fmain&pcampaignid=pcampaignidMKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1' style="display:inline-block"><img alt='Get it on Google Play' src='https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png' style="width:200px;"/></a>

The Concentric design is originally from the Google Pixel Watch (1). This project recreates it using [Watch Face Format](https://developer.android.com/training/wearables/wff). 

## Modify the Watch Face

The XML code can be found in the `res/raw` folder. Watch Face Format is well [documented](https://developer.android.com/training/wearables/wff/watch-face) in case you wish to modify the watch face.


## Build the Watch Face
⚠️ For a detailed explanation, refer to [wear-os-samples/WatchFaceFormat](https://github.com/android/wear-os-samples/tree/main/WatchFaceFormat)

Here's a quick overview:

```sh
git clone https://github.com/lukakilic/concentric-watch-face.git
```

Create a `build-wff.sh` file and paste the contents of [this shell script](https://github.com/android/wear-os-samples/blob/main/WatchFaceFormat/build-wff.sh) into it. Adjust the paths of 
`ANDROID_HOME`, `AAPT2`, `ANDROID_JAR`, `BUNDLETOOL` to match your system. 

Your folder should look like this:

```
/example-folder
│___ build-wff.sh    
└─── concentric-watch-face/
```

Then execute:

```shell
./build-wff.sh concentric-watch-face
```

Finally, install the watch face with:

```sh
adb install concentric-watch-face/out/result_apks/universal.apk
```
 

## Validate the code

If you've made changes to the code, validate it using the [memory footprint evaluator](https://github.com/google/watchface/tree/main/play-validations). This will ensure the watch face runs efficiently and check for errors in the XML code using the [XSD validator](https://github.com/google/watchface/blob/main/third_party/wff/README.md).