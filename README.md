Pico 1.14" LCD (Waveshare) Pinout to Wemos D1 Pinout:

    VCC (Power Input) - 3V3 (Wemos 3.3V pin)
    GND - GND (Wemos ground)
    DIN (SPI MOSI, Data input) - D7 (GPIO13, Wemos MOSI pin)
    CLK (SPI SCK, Clock) - D5 (GPIO14, Wemos SCK pin)
    CS (Chip select, Low active) - D2 (GPIO4)
    DC (Data/Command control) - D3 (GPIO0)
    RST (Reset, Low active) - D4 (GPIO2)
    BL (Backlight control) - D1 (GPIO5) or leave unconnected if the backlight is always on.
LED pin D8 (GPIO15)
LCD Setup: 
Display the Pico 1.14" LCD using the Adafruit ST7789 library. It’s initialized to 240x135 resolution.
Pin Definitions: Updated the pin mappings to reflect your connections with the Wemos D1 (e.g., TFT_CS, TFT_RST, TFT_DC, TFT_BL).
Distance Calculation: The distance is calculated using the Haversine formula, and the LED lights up if the ISS is within the threshold distance (1000 km).
