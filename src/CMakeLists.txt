set(BLE_SRCS
    ./BLE2902.cpp
    ./BLE2904.cpp
    ./BLEAddress.cpp
    ./BLEAdvertisedDevice.cpp
    ./BLEAdvertising.cpp
    ./BLEBeacon.cpp
    ./BLECharacteristic.cpp
    ./BLECharacteristicMap.cpp
    ./BLEClient.cpp
    ./BLEDescriptor.cpp
    ./BLEDescriptorMap.cpp
    ./BLEDevice.cpp
    ./BLEEddystoneTLM.cpp
    ./BLEEddystoneURL.cpp
    ./BLEExceptions.cpp
    ./BLEHIDDevice.cpp
    ./BLERemoteCharacteristic.cpp
    ./BLERemoteDescriptor.cpp
    ./BLERemoteService.cpp
    ./BLEScan.cpp
    ./BLESecurity.cpp
    ./BLEServer.cpp
    ./BLEService.cpp
    ./BLEServiceMap.cpp
    ./BLEUtils.cpp
    ./BLEUUID.cpp
    ./BLEValue.cpp
    ./FreeRTOS.cpp
    ./GeneralUtils.cpp
)


idf_component_register(
    SRCS ${BLE_SRCS} 
    INCLUDE_DIRS "." 
    REQUIRES "nvs_flash" "bt"
)
