# Qt-android-openSSL-shared-libs

Building OpenSSL for Qt on Android is poorly documented and a real pain in the ass since there is no definitive list of what versions of everything you need. This Repo hopes to relieve some of that pain.

Here you will find prebuild OpenSSL shared libraries that have been tested with Qt on actual android devices that you can distribute with your android apps.

If you want to thank me for the time saved by this repo then feel free to buy me a beer https://www.paypal.me/aatwo

# How do I use these in my Qt Android project?

Using the libs is easy:
    - find the copy of libcrypto.so and libssl.so that you want to use
    - add the following to your .pro file

```
ANDROID_EXTRA_LIBS+=$$PWD/<relative-path-to-openssl-libs>/libcrypto.so
ANDROID_EXTRA_LIBS+=$$PWD/<relative-path-to-openssl-libs>/libssl.so
```
