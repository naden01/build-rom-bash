#! /bin/bash

mf=(
device/xiaomi/clover
kernel/xiaomi/sdm660
vendor/xiaomi/clover
device/xiaomi/sdm660-common
vendor/xiaomi/sdm660-common
hardware/qcom-caf/sdm660/audio
hardware/qcom-caf/sdm660/media
hardware/qcom-caf/sdm660/display
hardware/xiaomi
)

rm -rf "${mf[@]}"

git clone https://github.com/pix106/android_device_xiaomi_clover.git  -b lineage-22.2-dynamic device/xiaomi/clover

git clone https://github.com/pix106/android_vendor_xiaomi_clover.git -b 15-qpr2 vendor/xiaomi/clover

git clone https://github.com/pix106/android_device_xiaomi_sdm660-common.git -b 15-qpr2-dynamic device/xiaomi/sdm660-common

git clone https://github.com/pix106/android_vendor_xiaomi_sdm660-common.git -b 15-qpr2 vendor/xiaomi/sdm660-common

git clone https://github.com/pix106/android_kernel_xiaomi_southwest-4.19.git -b main-dynamic-3.18.2 kernel/xiaomi/sdm660

git clone https://github.com/pix106/android_hardware_qcom-caf_audio.git -b lineage-22.2-caf-sdm660 hardware/qcom-caf/sdm660/audio

git clone https://github.com/pix106/android_hardware_qcom-caf_media.git -b lineage-22.2-caf-sdm660 hardware/qcom-caf/sdm660/media

git clone https://github.com/pix106/android_hardware_qcom-caf_display.git -b lineage-22.2-caf-sdm660 hardware/qcom-caf/sdm660/display

git clone https://github.com/LineageOS/android_hardware_xiaomi.git -b lineage-22.2 hardware/xiaomi

source build/envsetup.sh
brunch clover
