FROM nextcloudci/androidbase:androidBase-4

# Android 8.1 (API 27)
RUN sdkmanager --sdk_root=/opt/android-sdk-linux/ "platforms;android-27"
RUN sdkmanager --sdk_root=/opt/android-sdk-linux/ "system-images;android-27;google_apis;x86"
RUN (sleep 5; echo "no") | avdmanager create avd -n android -c 100M -k "system-images;android-27;google_apis;x86" --abi "google_apis/x86"
