# Fork of [FeitCSI](https://github.com/KuskoSoft/FeitCSI)

This fork addresses several bugs of the original code. These incuding:

- The compilation error of `'NL80211_CHAN_WIDTH_320' was not declared in this scope`. As a workaround, the support for 320 MHz bandwidth is removed.
- The `timestamp` field of CSI from `measure` mode is always zero. To solve the problem, the function `WiFiCsiController::processListenToCsiHandler` from `src/WiFiCsiController.cpp` is patched.

