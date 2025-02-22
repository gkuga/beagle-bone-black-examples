### Memo

```
ct-ng show-arm-cortex_a8-linux-gnueabi
ct-ng menuconfig
```

MacではCase Sensitiveボリュームを作成してそこでビルドする必要がある。

```diff
-CT_PREFIX_DIR="${CT_PREFIX:-${HOME}/x-tools}/${CT_HOST:+HOST-${CT_HOST}/}${CT_TARGET}"
+CT_PREFIX_DIR="${CT_PREFIX:-${HOME}/dev/ct-ng/x-tools}/${CT_HOST:+HOST-${CT_HOST}/}${CT_TARGET}"
```


